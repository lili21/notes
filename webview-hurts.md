遇到的移动端兼容问题
================

Android(4.2.2)
-------

- 不支持`flex-wrap`
- FileReader只支持DOM 0 level的事件绑定形式 `reader.onloadend = () => {}`
- `flexbox`子元素使用`float`会导致元素隐藏
- 默认不支持多媒体自动播放，需要通过[配置开启](https://developer.android.com/reference/android/webkit/WebSettings.html#setMediaPlaybackRequiresUserGesture(boolean))
- 即使通过配置支持了多媒体自动播放，也不支持base64格式的资源自动播放

iOS
---

- 默认不支持多媒体自动播放，需要通过[配置开启](https://developer.apple.com/documentation/uikit/uiwebview/1617954-mediaplaybackrequiresuseraction?language=objc)
- [input in fixed container](https://hackernoon.com/how-to-fix-the-ios-11-input-element-in-fixed-modals-bug-aaf66c7ba3f8)