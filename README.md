#taro-demo
taro-demo,附上一些简单的小效果
1. 分享
2. 左滑删除
3. 瀑布流
4. 骨架屏

##启动步骤：
1. npm i -g @tarojs/cli@1.3.0
2. npm i
3. 编译h5：npm run dev:h5

##参考链接
[taro](https://nervjs.github.io/taro/)
[taro-ui](https://taro-ui.aotu.io/#/) (目前没用到)
[nativeshare](https://www.npmjs.com/package/nativeshare)

##瀑布流效果
1. 直接读取本地mock数据，启动npm run dev:h5:mock

##骨架屏
注意后代选择器的兼容性问题。
1. 百度小程序目前不支持跨自定义组件的后代选择器: >>>。
2. 但是H5使用后代选择器(.the-ancestor .the-descendant)的时候，可以自动识别自定义组件内的后代。使用自定义组件时，外层是否有元素包裹，都可识别到自定义组件内部的指定类选择器。
3. 微信小程序支持跨自定义组件的后代选择器(.the-ancestor >>> .the-descendant)，但使用自定义组件时，外层不能嵌套元素，否则无法识别。