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

[antdTable](https://ant-design.antgroup.com/components/table-cn)

[antdProTable](https://procomponents.ant.design/components/table)

andtTable：单纯的渲染组件

antdProTable: 官方封装过重，难以还原UI设计，交互逻辑



## 设计思路



![image-20241213150840733](https://typora-huang-cong.oss-cn-shanghai.aliyuncs.com/image-20241213150840733.png)

<!-- more-->

## 结构图

简单的表格组件 `SimpleTable` 及其相关的功能模块，包括分页、搜索和数据控制。具体来说：

- **useTableController**：这是一个自定义 Hook，用于管理表格的数据、分页和搜索逻辑。它提供了以下功能：
  - **paginationController**：管理分页状态，包括当前页码、每页大小、总记录数等。
  - **searchController**：管理搜索参数和重置功能。
  - **tableController**：管理表格数据，包括加载状态、选中的行等。
  - **refresh**：刷新表格数据。
  - **reset**：重置分页和搜索参数。
- **SimpleTable**：这是一个表格组件，基于 Ant Design 的 `Table` 组件。它接收 `columns` 和 `tableController` 作为属性，并渲染表格数据。支持行选择功能。
- **SimplePagination**：这是一个分页组件，基于 Ant Design 的 `Pagination` 组件。它接收 `paginationController` 作为属性，并渲染分页控件。
- **SimpleSearch**：这是一个搜索组件，基于 `@ant-design/pro-components` 的 `QueryFilter` 组件。它接收 `searchController` 和子组件作为属性，并提供搜索表单的功能，支持表单提交和重置。



![image-20241213145040903](https://typora-huang-cong.oss-cn-shanghai.aliyuncs.com/image-20241213145040903.png)

![image-20241213143002501](https://typora-huang-cong.oss-cn-shanghai.aliyuncs.com/image-20241213143002501.png)

## UI样式及兼容处理

1. UI样式的实现
2. 交互逻辑，默认组件配置添加
3. 不要侵入基础组件

![image-20241213153951504](https://typora-huang-cong.oss-cn-shanghai.aliyuncs.com/image-20241213153951504.png)



![image-20241213155443550](https://typora-huang-cong.oss-cn-shanghai.aliyuncs.com/image-20241213155443550.png)



## 应用

提供当前UI，及交互逻辑标准实现，并添加实用组件

![image-20241213161440188](https://typora-huang-cong.oss-cn-shanghai.aliyuncs.com/image-20241213161440188.png)



## 目录结构

```
src/components/SimpleTable/
├── context.ts
├── index.ts
├── SimpleTableInstance.tsx
├── standardWrapper.tsx
├── style.module.less
└── types.ts
```

### 目录结构说明

1. **context.ts**:
   - 定义和导出 `SIMPLETABLE_CONTEXT` 和 `SIMPLETABLE_CONTEXT_TYPE`，用于在组件之间传递配置属性。
2. **index.ts**:
   - 导出 `SimpleTable` 组件及其相关组件，方便外部引用。
3. **SimpleTableInstance.tsx**:
   - 实现 `SimpleTable` 组件的实例化逻辑，包括 `Search`、`Table` 和 `Pagination` 子组件的配置和渲染。
4. **standardWrapper.tsx**:
   - 使用 `styled-components` 和 `React.Context` 对 `SimpleTable` 组件的各个部分（如 `Search`、`Table` 和 `Pagination`）进行样式修改，并传递配置属性。
5. **style.module.less**:
   - 定义 `SimpleTable` 组件的样式，使用 CSS 模块化的方式避免样式冲突。
6. **types.ts**:
   - 定义 `SimpleTable` 组件及其子组件的相关类型，确保类型安全。





## 方案详情

1.抽离 table 的状态和数据到控制器，暴露出 table 渲染数据，seachController 和 pagenationController 写为 hooks。

2.将控制器和数据传入 Search,Table,Pagination，简单封装为 SimpleSearch,SimpleTable,SimplePagination 等**纯逻辑组件**完成表单交互。

3.使用 styled-components 编写 Wrapper 组件包装**纯逻辑组件**完成与 UI 设计稿的一致性。

4.使用 React.Context 在 Wrapper 和**纯逻辑组件**之间传递 antd 组件 props 实现封装组件和 antd 组件 API 整合。

5.使用 Wrapper 和**纯逻辑组件**封装开箱即用 Table,以覆盖多数场景。



## 基本使用

``` tsx

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

``` ts

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

``` tsx
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

