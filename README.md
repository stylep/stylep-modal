# stylep-modal
<img src=https://avatars1.githubusercontent.com/u/16121328?v=3&s=200 title=stylep-button align=right height=95>

Everything you need to get started making a new style pattern.

## Install
You can install using the [spm](https://github.com/stylep/stylep) command or install using npm and the project name.

``` shell
spm install modal
```

## Usage
``` css
/* modal.css */

@import “stylep-modal”;

.modal {

  /* Modal Design Pattern */
  @extend %modal-inline;

  /* Customize your modal */
  @mixin modal-solid #444, #f7f7f7, #888, 4px, none, none;

  /* or roll your own */

  background-color: pink;
  color: white;
}
```

## Patterns
Placeholder selectors that contain common styles for structure and basic behavior.

#### `@extend %modal-inline;`
This draws a simple inline modal without style.

#### `@extend %modal-block;`
This draws a simple block modal without style.

## Styles
Customizable presets that give your pattern a specific style-set.

### modal-solid
A card-like solid style for a modal.

##### Options

* `$color-passive: #f7f7f7` Background color of the modal
* `$color-text: #444` Color of the text of the modal body
* `$radius-size: 0` Rounded corner value for the modal
* `$border: none` Style of border for the modal
* `$shadow: 0 2px 2px rgba(0, 0, 0, .4)` Basic shadow option for the modal

##### Example
```css
/* A solid modal with a light background, dark text, no radius, dark border and a dark shadow applied */
@mixin modal-solid #f7f7f7, #444, 0, 1px solid #444, 0 2px 2px #000;
```

### modal-hollow
A card-like hollow style for a modal.

##### Options

* `$color-passive: #444` Border color of the modal
* `$color-text: #444` Color of the text of the modal body
* `$color-background: #fff` Background color of the modal
* `$radius-size: 0` Rounded corner value for the modal
* `$border-width: 1px` Width of border for the modal
* `$shadow: none` Basic shadow option for the modal

##### Example
```css
/* A solid modal with a light background, dark text, no radius, dark border and a dark shadow applied */
@mixin modal-solid #f7f7f7, #444, 0, 1px solid #444, 0 2px 2px #000;
```

## License
This project is licensed under the MIT [license](LICENSE).
