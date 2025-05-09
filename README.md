# Gateway To React
[尚硅谷React教程](https://www.bilibili.com/video/BV1wy4y1D7JT/?spm_id_from=333.788.recommend_more_video.0&vd_source=6d423245acce785b947bbbe5fe626aac)
## 原生JavaScript痛点
- 操作DOM，繁琐，效率低（DOM-API操作UI）
- 直接操作真实DOM，浏览器会进行大量重排重绘（消耗浏览器资源，影响性能）
- 没有组件化代码模块，代码复用率低（重复代码多，可读性差）

### JSX语法规则：
1. 样式不能使用class, 而是className
2. 内联样式使用Style，需传入一个对象，style = {{}}属性名驼峰命名法
3. 标签中混入js表达式，使用{}包裹
    - js的一个表达式会产生一个值
    - js语句：if、for、while、switch、try...catch等，不能直接放在{}
    - js表达式：变量(a)、函数(demo(1))、对象、数组、字符串, 方法(function test) 等，能直接放在{}中
4. 虚拟DOM，必须只能有一个根元素，不能有多个根元素, 单标签元素需要加上/
5. 标签首字母
   - 若是小写字母，自动转为html里边同名元素，如果找不到则报错
   - 若是大写字母，React就直接自动去渲染对应的组件

### 模块与组件
- js模块：把不同功能的代码放在不同的js文件里边，复用js代码，简化js编写，提高js运行效率
- 组件：结构，样式，交互，音视频，图片等资源的集合，（html, css, js, video/audio/image），复用代码，简化项目，提供执行效率
