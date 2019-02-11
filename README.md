# GrapesJS TOAST UI Image Editor


## Summary

* Plugin name: `grapesjs-tui-image-editor`
* Commands





## Options

|Option|Description|Default|
|-|-|-
|`option1`|Description option|`default value`|





## Download

* CDN
  * `https://unpkg.com/grapesjs-tui-image-editor`
* NPM
  * `npm i grapesjs-tui-image-editor`
* GIT
  * `git clone https://github.com/artf/grapesjs-tui-image-editor.git`





## Usage

Directly in the browser
```html
<link href="https://unpkg.com/grapesjs/dist/css/grapes.min.css" rel="stylesheet"/>
<script src="https://unpkg.com/grapesjs"></script>
<script src="path/to/grapesjs-tui-image-editor.min.js"></script>

<div id="gjs"></div>

<script type="text/javascript">
  var editor = grapesjs.init({
      container : '#gjs',
      // ...
      plugins: ['grapesjs-tui-image-editor'],
      pluginsOpts: {
        'grapesjs-tui-image-editor': { /* options */ }
      }
  });
</script>
```

Modern javascript
```js
import grapesjs from 'grapesjs';
import tUIImageEditor from 'grapesjs-tui-image-editor';

const editor = grapesjs.init({
  container : '#gjs',
  // ...
  plugins: [tUIImageEditor],
  pluginsOpts: {
    [tUIImageEditor]: { /* options */ }
  }
  // or
  plugins: [
    editor => tUIImageEditor(editor, { /* options */ }),
  ],
});
```





## Development

Clone the repository

```sh
$ git clone https://github.com/artf/grapesjs-tui-image-editor.git
$ cd grapesjs-tui-image-editor
```

Install dependencies

```sh
$ npm i
```

Start the dev server

```sh
$ npm start
```





## License

BSD 3-Clause
