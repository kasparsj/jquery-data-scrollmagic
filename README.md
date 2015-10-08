# jquery-ScrollMagic
ScrollMagic data attribute shortcuts

This plugin aims to make ScrollMagic development more agile, by providing ways of creating ScrollMagic scenes via data attributes.

#Usage

```html
<div data-sm='{"opacity":1,"triggerHook":0.7,"duration":"75vh"}'></div>
<div data-sm='[{"opacity":1,"triggerElement":"#screen-text-1","triggerHook":0.25,"duration":150},{"opacity":0,"triggerElement":"#screen-text-2","triggerHook":1,"duration":150}]'></div>
```
