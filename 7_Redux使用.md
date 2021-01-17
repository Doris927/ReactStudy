# Redux使用
- 基本概念
  - store state
  - action 
  - reducer
- 单项数据流
  - dispatch(action)
  - reducer -> new state
  - subscribe 触发通知
- react-redux
- 异步action
  - 同步action 返回一个action
  - return一个函数，需要，redux-thunk
- 中间件
  - redux thunk
  - redux promise
  - redux saga


## 基础
- provider
- connect

## redux 中间件
- button - callback -> dispatch - action -> reducer - state -> view
- button - callback -> (mid1 -> mid2 - action -> dispatch)(new dispatch) - action -> reducer

## react-router
- 路由模式
  - hash模式
  - history模式
  - 后者需要server支持
- 路由配置