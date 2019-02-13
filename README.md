# GrapesJS TOAST UI Image Editor

TODO
* Another command id
* Add new toolbar icon to image components
* Option custom "edit image" icon (better callback for the toolbar)
* Update README

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
        'grapesjs-tui-image-editor': {
          config: {
            includeUI: {
              initMenu: 'filter',
              theme: {
                'menu.normalIcon.path': 'https://ui.toast.com/static/icon-d.4ef3abbd.svg',
                'menu.activeIcon.path': 'https://ui.toast.com/static/icon-b.d70663d0.svg',
                'menu.disabledIcon.path': 'https://ui.toast.com/static/icon-a.843c03ed.svg',
                'menu.hoverIcon.path': 'https://ui.toast.com/static/icon-c.6f440c0d.svg',
                'submenu.normalIcon.path': 'https://ui.toast.com/static/icon-d.4ef3abbd.svg',
                'submenu.activeIcon.path': 'https://ui.toast.com/static/icon-c.6f440c0d.svg',
              }
            },
          }
        }
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
