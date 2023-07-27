# OωO

> Lovely Emoticon and Emoji Keyboard for textarea or input

## 运行环境

- Node：11.x（不能 >=12.0）

## Introduction

[Demo](http://diygod.github.io/OwO/demo)

Screenshot

![OwO](http://i.imgur.com/eRSh95i.jpg)

## Install

```js
$ npm install owo --save
```

## Usage

### HTML

```html
<link rel="stylesheet" href="OwO.min.css">
<!-- ... -->
<div class="OwO"></div>
<!-- ... -->
<script src="OwO.min.js"></script>
```

### JS

```js
var OwO_demo = new OwO({
    logo: 'OωO表情',
    container: document.getElementsByClassName('OwO')[0],
    target: document.getElementsByClassName('OwO-textarea')[0],
    api: './OwO.json',
    type: 'data-src',
    position: 'down',
    width: '100%',
    maxHeight: '250px'
});
```

#### Options

```js
{
    logo: 'OωO表情',                                               // OwO button text, default: `OωO表情`
    container: document.getElementsByClassName('OwO')[0],         // OwO container, default: `document.getElementsByClassName('OwO')[0]`
    target: document.getElementsByClassName('OwO-textarea')[0],   // OwO target input or textarea, default: `document.getElementsByTagName('textarea')[0]`
    api: './OwO.json',                                            // OwO Emoticon data api, default: `https://api.anotherhome.net/OwO/OwO.json`
    type: 'data-src',                                            // json image图片路径
    position: 'down',                                             // OwO body position, default: `down`
    width: '100%',                                                // OwO body width, default: `100%`
    maxHeight: '250px'                                            // OwO body max-height, default: `250px`
}
```

#### Work with module bundler

```js
var OwO = require('owo');
var OwO_demo = new OwO({
    // ...
});
```

### Data API

Provide emoticon data for OwO.

[Example](https://api.anotherhome.net/OwO/OwO.json)

## Run in development

```js
$ npm install
$ npm run dev
```

## Make a release

```js
$ npm install
$ npm run build
```

## LICENSE

MIT © [DIYgod](http://github.com/DIYgod)