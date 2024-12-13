---
title: antd simpleTable
date: 2024-12-12 19:54:00
type: "tags"
tags:
  - antd
categories: 前端组件
---

## 问题简述

andt 表格组件 Table 需要封装，样式还原原型，统一数据源接口，搜索，分页

## 方案详情

1.抽离 table 的状态和数据到控制器，暴露出 table 渲染数据，seachController 和 pagenationController 写为 hooks。

2.将控制器和数据传入 Search,Table,Pagination，简单封装为 SimpleSearch,SimpleTable,SimplePagination 等**纯逻辑组件**完成表单交互。

3.使用 styled-components 编写 Wrapper 组件包装**纯逻辑组件**完成与 UI 设计稿的一致性。

4.使用 React.Context 在 Wrapper 和**纯逻辑组件**之间传递 antd 组件 props 实现封装组件和 antd 组件 API 整合。

5.使用 Wrapper 和**纯逻辑组件**封装开箱即用 Table,以覆盖多数场景。

<!-- more-->

## 基本使用

````

import {
  SimpleSearchInstance,
  SimpleTableInstance,
  useTableController,
  GetTableData,
} from "@/components/SimpleTable";

  const dataFetcher: GetTableData<any> = async ({ page, size, params }) => {
    const resp = await request("/absc/v1/enterprise-accounts/list", "GET", {
      page,
      size,
      ...params,
    });

    const { totalElements, failed, content } = resp;

    if (failed) {
      return {total:0,data:[]};
    }
    return {
      data: content,
      total: totalElements,
    };
  };

  const { pagenationController, tableController, searchController } =
    useTableController(dataFetcher);

  const columns = [
    {
      title: "账号",
      dataIndex: "userId",
      key: "userId",
    },
    {
      title: "操作",
      dataIndex: "address",
      key: "address",
      render: () => (
        <a
          onClick={() => {
            navigate("/home/user-manage/edit/12");
          }}
        >
          编辑
        </a>
      ),
    },
  ];

      // 搜索
     <SimpleSearchInstance searchController={searchController}>
        <ProFormText placeholder='请输入' name='accountName' label='用户名' />
        <ProFormText placeholder='请输入' name='mobilePhone' label='手机号' />
        <ProFormText placeholder='请输入' name='email' label='邮箱' />
      </SimpleSearchInstance>

     // 表头
        <SimpleTableInstance
        columns={columns}
        tableController={tableController}
        pagenationController={pagenationController}
      />



```


## 进阶使用方式
自定义包装器，包装核心组件实现样式自定义，以及antd组件Table的API使用；具体写法参考 standardWrapper

## API

### useTableController

#### 参数

| 名称              | 类型       | 描述         | 是否必输 | 默认值 |
| ----------------- | ---------- | ------------ | -------- | ------ |
| tableDataFrom     | 函数或数组 | 数据源       | 是       |        |
| options.autoQuery | boolean    | 创建自动查询 | 否       | true   |
| options.size      | number     | 每页大小     | 否       | 5      |



#### 返回

```typescript

 {
  // pagination控制器
  paginationController: PaginationController;
  // 查询框控制器
  searchController: SearchController;
  // 表格数据
  tableController: TableController<T>;
  // 刷新数据
  refresh: () => Promise<void>;
  // 重置表格
  reset: (arg: {
    page?: number;
    size?: number;
    params?: Record<string, any>;
  }) => void;
 }

```







## 开箱即用组件

### 基本使用

```typescript
import {
  SimpleSearchInstance,
  SimpleTableInstance,
  useTableController,
  GetTableData,
} from "@/components/SimpleTable";
import { ProFormText } from "@ant-design/pro-form";

const Component:React.FC<PropsType> = ()=>{

    // 声明数据源
  const dataFetcher: GetTableData<any> = async ({ page, size, params }) => {
    const resp = await request("/absc/v1/enterprise-accounts/list", "GET", {
       // pagination 和后端的page相差1
      page:page-1,
      size,
      ...params,
    });

    const { totalElements, failed, content } = resp;

    if (failed) {
      return {
        data: [],
        total: 0,
      };
    }
    return {
      data: content,
      total: totalElements,
    };
  };


  const { paginationController, tableController, searchController ,refresh,reset} =
    useTableController(dataFetcher);


  return <>
       <SimpleSearchInstance searchController={searchController}>
        <ProFormText placeholder='请输入' name='accountName' label='用户名' />
        <ProFormText placeholder='请输入' name='mobilePhone' label='手机号' />
        <ProFormText placeholder='请输入' name='email' label='邮箱' />
      </SimpleSearchInstance>
     <SimpleTableInstance
          columns={generateColumns()}
          tableController={tableController}
          paginationController={paginationController}
        />
      </>

}


```



### SimpleTableInstance



| 参数                 | 类型                    | 描述                                                         | 是否必输 | 默认值 |
| -------------------- | ----------------------- | ------------------------------------------------------------ | -------- | ------ |
| columns              | 数组                    | antd的Table组件的columns                                     | 是       | 无     |
| tableController            | tableController                | antd的Table组件的dataSource 和 loading                                 | 是       | 无     |
| paginationController | PaginationController    | SimplePagination的参数，简单封装了pagination的逻辑           | 是       | 无     |
| tableExtraProps      | antd的Table的props      | antd的Table的props，使用table功能时传入对应的参数            | 否       | 无     |
| paginationExtraProps | antd的Pagination的props | antd的Pagination的props,使用Props的功能时，可以传入对应的参数 | 否       | 无     |

### SimpleSearchInstance



| 参数             | 类型                                               | 描述                                            | 是否必输 | 默认值 |
| ---------------- | -------------------------------------------------- | ----------------------------------------------- | -------- | ------ |
| searchController | SearchController                                   | SimpleSearch的参数，简单封装了QueryFilter的逻辑 | 是       | 无     |
| searchExtraProps | @ant-design/pro-components的组件QueryFilter的props | 使用QueryFilter的功能时可以传入对应的参数       | 否       | 无     |
|                  |                                                    |                                                 |          |        |

````
