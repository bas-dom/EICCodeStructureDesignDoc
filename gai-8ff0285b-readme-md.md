# EIC 框架选型 {#om-框架选型}



### 1. 路由 {#1-路由}

方案：react-router + react-redux-router

### 2. 数据 {#2-数据}

方案：redux 特点： 1、轻量级库，解决 component -&gt; action -&gt; reducer -&gt; state 的单向数据流转问题。 2、可预测性（函数式编程方式，纯函数、纯对象使得应用程序行为可预测，有利于增强应用程序的稳定性），可扩展性（dispatch、reducer、store等均可扩展）

### 3. 数据模型 -&gt; 视图模型 {#3-数据模型---视图模型}

方案：reselect 特点： 1、将视图涉及到的一些业务逻辑提取出来，使 Component 保持功能专一 2、可组合性，selector 之间可以相互组合，提高逻辑复用性 3、缓存机制，更新时利用缓存检测视图模型是否变化，减少不必要的重绘

### 4. 视图的 CSS 方案 {#4-视图的-css-方案}

方案：css-module 特点： css 模块化，解决命名冲突，各个组件的 css 之间不会相互冲突

### 5. 业务逻辑 Action {#5-业务逻辑-action}

方案：redux-saga 特点： 消除异步请求给 redux 带来的副作用，统一业务逻辑

### 6. 请求数据 {#6-请求数据}

方案：fetch



##  {#桌面端}



