## 高级特性
- 函数组件
- 非受控组件
- Portals
- context
- 异步组件
- 性能优化
- 高阶组件HOC
- render props
  
## 函数组件
- 混函数，输入props，输出jsx
- 没有实例，没有生命周期，没有state
- 不能扩展其他的方法

## 非受控组件
- ref
- defalutValue defaultChecked
- 手动操作Dom元素
- 使用场景：
  - 必须手动操作dom元素，setState实现不了
  - 文件上传<input type="file">
  - 某些富文本编辑器，需要传入dom元素
  - 触发强制动画
- 具体选择
  - 优先使用受控组件，符合React设计原则
  - 必须操作dom时，再使用非受控组件

## React Portals
- 默认按照层级渲染，如何让组件渲染到父组件以外
- 使用场景
  - overflow：hidden
  - 父组件z-index值太小
  - fixed需要放在body第一层级
  - 比如modal，对话框等

## React context
- 公共信息（语言，主题）如何传递到每个组件
- 用props太繁琐
- 用redux小题大作
- 面试时的问题
  - 什么时候需要用到
  - 怎么创建，怎么消费

## 异步加载组件
- import
- React.lazy React16.6
- React.Suspense
- 什么时候需要异步组件？
  - 组件比较大，需要懒加载的时候

## 性能优化
- 性能优化对React更加重要
- shouldComponentUpdate
- PureComponent和React.memo
- 不可变值 immutable

## SCU
- 默认返回什么 true
- React默认父组件有更新，子组件就会更新
- SCU一定要每次都用吗？
  - 需要的时候才用，页面卡顿的时候才用

## PureComponent和React.memo
- PureComponent在SCU中实现了浅比较 React 16中已经实现了
- memo, 函数组件中的PureComponent React 16.6

## immutable.js
- 不可变值
- 基于共享数据的技术（不是深拷贝），速度较好
- 有一定学习和迁移成本

## 组件公共逻辑的抽离
- mixin, 已经被React废弃
- 高阶组件 HOC
- Render Props

## 高阶组件
- redux connect就是高阶组件

## render props
