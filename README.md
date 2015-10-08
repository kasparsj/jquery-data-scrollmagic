# jquery-scrollmagic
ScrollMagic data attribute shortcuts

This plugin aims to make ScrollMagic development more agile, by providing ways of creating ScrollMagic scenes via data attributes.

##Usage

### Pinning

```html
<div data-scrollmagic='{"pin":true,"triggerHook":0,"duration":"100vh"}'></div>
<div data-scrollmagic='{"pin":{pushFollowers:true,classes:"pinned"},"triggerHook":0,"duration":"100vh"}'></div>
```

### Tweening

```html
<!-- fade-in single scene -->
<div data-scrollmagic='{"opacity":1,"triggerHook":0.7,"duration":"75vh"}'></div>

<!-- fade in and out - two scenes -->
<div data-scrollmagic='[{"opacity":1,"triggerElement":"#screen-text-1","triggerHook":0.25,"duration":150},{"opacity":0,"triggerElement":"#screen-text-2","triggerHook":1,"duration":150}]'></div>
```

### Class Toggle

```html
<div data-scrollmagic='{"class":"active","triggerHook":0,"duration":"100vh"}'></div>
<div data-scrollmagic='{"class":{"classes":"active","toggle":true},"triggerHook":0,"duration":"100vh"}'></div>
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
