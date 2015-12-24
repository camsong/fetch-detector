## Fetch Detector

有些浏览器虽然支持 Fetch API 但不完整，如 Chrome 45 和 Firefox 33 版本 response
中的[中文会乱码](https://code.google.com/p/chromium/issues/detail?id=511289)[2](https://code.google.com/p/chromium/issues/detail?id=516931)。本库的作用是只在 Chrome >= 46，Firefox >= 39 时才开启原生
Fetch，否则使用 XHR polyfill。

## Install

```
npm install 'fetch-detector'
```

## Usage

一定要与 fetch-ie8 一起使用， 并且放到 fetch-ie8 前引用。

```js
import 'fetch-detector'
import 'fetch-ie8'
```

## License
MIT
