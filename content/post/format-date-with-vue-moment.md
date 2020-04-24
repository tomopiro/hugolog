+++
author = "tueda"
title = "vue-momentで日付をフォーマットする"
date = "2020-03-05"
description = "Vue.jsで日付をフォーマットする時の方法"
tags = [
    "Vue.js",
    "JavaScript",
]
categories = [
    "プログラミング",
]
series = ["Themes Guide"]
aliases = ["migrate-from-jekyl"]
+++

## インストール

```bash:
npm install vue-moment
```

#Vueプロジェクトにインポート
```javascript:main.js
Vue.use(require('vue-moment'));
```

## vueファイルで使う
or演算子｜の右辺でフォーマット形式を指定します。

```javascript:App.vue
{{ new Date() }}
// 05 2020 19:38:33 GMT+0900 (日本標準時)

{{ new Date() | moment("dddd, MMMM, Do, YYYY, h:mm:ss a") }}
// Thursday, March, 5th, 2020, 7:38:33 pm

{{ new Date() | moment("YYYY/MM/DD") }}
// 2020/03/05
```

## 参考にしたサイト

vue-moment  -  npm  
[https://www.npmjs.com/package/vue-moment](https://www.npmjs.com/package/vue-moment)

