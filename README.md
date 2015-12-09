# stylep-modal

Everything you need to get started making a new style pattern.

## Install
``` shell
npm i --save-dev stylep-modal
```

## Usage
``` css
/* modal.css */

@import “stylep-modal”;

.class {

  /* Button Design Pattern */
  @extend %modal;

  /* Customize your button */
  @mixin modal param, param;

  /* or roll your own */

  /* add something custom in here */
}
```

## Patterns
Placeholder selectors that contain common styles for structure and basic behavior.

#### `@extend %modal-of-pattern;`
Describe what this pattern does.

## Styles
Customizable presets that give your pattern a specific style-set.

### modal
Describe the visual look and feel of this style.

##### Options

* `$param-modal: default-value` Describe what this does

##### Example
```css
/* describe in english what this following statement really means in detail */
@mixin modal default-value;
```

