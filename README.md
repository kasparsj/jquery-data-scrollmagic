# jquery-scrollmagic
ScrollMagic data attribute shortcuts

This plugin aims to make ScrollMagic development more agile, by providing ways of creating ScrollMagic scenes via data attributes.

## Availability

```bash
bower install jquery-scrollmagic
```

## Installation

Install ScrollMagic as per: https://github.com/janpaepke/ScrollMagic#installation

Then add the jquery-scrollmagic plugin:

```html
<script src="bower_components/jquery-scrollmagic/jquery.scrollmagic.min.js"></script>
```

## Usage

### Pinning feature

```html
<!-- pin element for the duration of viewport height -->
<div data-scrollmagic='{"pin":true,"triggerHook":0,"duration":"100vh"}'></div>

<!-- pin element, pushing all elements below -->
<div data-scrollmagic='{"pin":{pushFollowers:true},"triggerHook":0,"duration":"100vh"}'></div>
```

### Tweening feature

```html
<!-- fade in (single scene) -->
<div data-scrollmagic='{"tween":{"opacity":1},"triggerHook":0.7,"duration":"75vh"}'></div>

<!-- fade in and out (two scenes) -->
<div data-scrollmagic='[{"tween":{"opacity":1},"triggerElement":"#screen-text-1","triggerHook":0.25,"duration":150},{"tween":{"opacity":0},"triggerElement":"#screen-text-2","triggerHook":1,"duration":150}]'></div>
```

### Class-toggle feature

```html
<!-- add class "active, while the element is in the center of the viewport" -->
<div data-scrollmagic='{"class":"active","duration":"100%"}'></div>

<!-- toggle class "active", while the element is in the center of the viewport -->
<div class="active" data-scrollmagic='{"class":{"classes":"active","toggle":true},"duration":"100%"}'></div>
```

### Mixing features

```html
<!-- when the element reaches screen top, pin it, and tween background color to red, for the duration of viewport height -->
<div data-scrollmagic='{"pin":true,"tween":{"backgroundColor":"#ff0000"},"class":"pinned","triggerHook":0,"duration":"100vh"}'></div>
```

### Options

Same options as for ScrollMagic Scene.

#### duration
**Type:** number or string (percentage or viewport units)

#### offset
**Type:** number

#### triggerElement
**Type:** string or object

#### triggerHook
**Type:** string or number

#### reverse
**Type:** boolean

#### loglevel
**Type:** number
