# WeChatMiniParams(微信小程序)

命名规则：下划线后的字母必须小写
Naming Rule: When using underscores in names, the letter following the underscore must be lowercase.

微信小程序的 Base64 转换方法与标准 Web 不同
Base64 Conversion: Base64 conversion in WeChat Mini Programs is different from standard web methods.

Click 事件不能传参时使用 :data-*
Passing Parameters in Click: If you can’t pass parameters directly in a click event, use :data-*="parameter" instead.

Image 标签 width 或 height 为 auto 会直接不显示
Image Display: If width or height of an image is auto, the image won’t show at all. You must provide a concrete value (even 100% may not work).

微信小程序中 left 等属性 rpx 实际调试参数是 px
Positioning Units: In WeChat Mini Programs, properties like left may be written in rpx, but during debugging the actual value is in px.

动态绑定 class 时必须使用数组
Dynamic Class Binding: When dynamically binding classes, you must use an array, otherwise class names can randomly disappear for no apparent reason.

父组件传函数到子组件偶现失效
Passing Functions: Passing a function from parent to child via :xxx= sometimes fails and the child receives its own this. Solution: Use @ to pass the function.

避免在标签上直接使用 v-if
v-if Usage: Never put v-if directly on elements in WeChat Mini Programs, it can cause big, frustrating problems.

涉及页面更新的变量必须使用 $set
Updating Variables: Any variable related to page updates (especially in uniapp) must be updated using $set.

类切换顺序要注意
Class Switching: When switching classes, ensure the switching class is after the base class; otherwise, the new class may refuse to work for reasons only WeChat knows.

微信小程序的变量不能有多个不同的逻辑复用会导致页面无法正常渲染（哪怕是临时变量也不行
WeChat Mini Program variables cannot be reused with multiple different logics, which will cause the page to not render properly (even temporary variables are not allowed)

注意微信小程序的模拟器上部分状态下disply:flex和正常web的不会一致（具体场景正在进行验证）
Note that in some states of the WeChat applet simulator, the display:flex will not be consistent with the normal web (specific scenarios are being verified)

微信小程序的模拟器上的canvas是不会随着页面的滚动而滚动的（实机测试没有这个问题）
The canvas on the WeChat applet simulator does not scroll as the page scrolls (there is no such problem in the actual machine test)

注意uniapp转微信小程序最好不要使用click方法使用tap（否则会导致向父组件传参出现异常）
Note that it is best not to use the click method when transferring uniapp to WeChat applet, but tap (otherwise it will cause an exception when passing parameters to the parent component)
