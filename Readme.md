*This repository is a mirror of the [component](http://component.io) module [segmentio/sheet](http://github.com/segmentio/sheet). It has been modified to work with NPM+Browserify. You can install it using the command `npm install npmcomponent/segmentio-sheet`. Please do not open issues or send pull requests against this repo. If you have issues with this repo, report it to [npmcomponent](https://github.com/airportyh/npmcomponent).*
# sheet

  A special modal that slides out from the right or left side of the screen.

  ![example of a sheet](http://i.cloudup.com/HNkFjYOyCE.png)

## Installation

    $ component install segmentio/sheet

## Example

```js
var sheet = require('sheet');
sheet(el).show();
```

  To use it, pass in the `el` you want to "sheet-ize".

## API

```html
<div class="Modal" effect="sheet-left">
  <div class="Sheet">
    <a class="Sheet-close-button"></a>
    { Your element gets injected here. }
  </div>
</div>
<div class="Overlay"></div>
```

A [`segmentio/overlay`](https://github.com/segmentio/overlay) element (with an `.overlay` class) is used to create the mask above the screen, so if you've already themed it you've got no more work to do.


### Sheet(el)
  Create a new `Sheet` instance with the given `el`.

### #show(fn)
  Show the sheet, emitting `show`, optionally calling `fn`.

### #hide(fn)
  Hide the sheet, emitting `hide`, optionally calling `fn`.

### #addClass(name)
  Add a class `name` to the `.sheet` and `.sheet-overlay`.

### #removeClass(name)
  Remove a class `name` from the `.sheet` and `.sheet-overlay`.

## License

  MIT
