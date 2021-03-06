
Markdown Editor
------------------------

A markdown editor integrate `write` and `preview` tabs like Github's flavored editor.

### Live Demo

- [Markdown-Editor Demo](http://weflex.github.io/markdown-editor-flavored/)
- [Screenshots](#screenshots)

### Install

```sh
$ npm install markdown-editor-flavored
$ bower install markdown-editor-flavored
```

### Usage

Define your `div` element as the editor replacement.

```html
<div id="markdown-editor-sample"></div>
```

And write JavaScript:

```js
var editor = new MarkdownEditor('#markdown-editor-sample', {
  // this is optional
  'width': '100%',
  'margin': '5px'
});
editor.render();
```

You can specify the width of editor by calling the `.render` function with an argument like:

```js
editor.render('auto');
// or
editor.render('500px');
```

### Environment Variables

`MARKDOWN_EDITOR_FLAVORED_STYLE_PATH`: to change the root path to search style, the usage:

```js
window.MARKDOWN_EDITOR_FLAVORED_STYLE_PATH = 'your_root_dir';
```

`MARKDOWN_EDITOR_DISABLE_AUTO_LOAD_STYLE`: to disable the auto load of styles(`markdown-editor.css`), the usage:

```js
window.MARKDOWN_EDITOR_DISABLE_AUTO_LOAD_STYLE = true;
```

(This is used for some custom tools to load the style in their working group, like `concat`).

### Screenshots

![Preview UI](resource/preview.png)
![Write UI](resource/write.png)

### License

MIT
