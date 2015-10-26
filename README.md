# Minimal setup
Link to jQuery and slider-responsive.min.js file. Use basic HTML markup written below, specify a few necessary styles and call plugin itself.
[Watch demo on codepen](http://codepen.io/docode/pen/NqyawK)
### Basic HTML
```html
<div class="slider">
    <ul class="slides-wrapper">
        <li>1st slide</li>
        <li>2nd slide</li>
              ...
        <li>n-th slide></li>
    </ul>
    <ul>
        <li class="sl-prev">&larr;</li>
        <li class="sl-next">&rarr;</li>
    </ul>
</div>
```
You can specify your own classes. Read **options** section
### Required styles
Most required styles are specified in the plugin itself. All you left to do is:
* specify `width` and `height` of the slider
* properly position controls (`sl-prev` and `sl-next`). Otherwise they will be hidden.

### Call plugin
```javascript
$('.slider').sliderResponsive();
```
### Options
Option | Defalut value | 
-------|---------------|----------
`anim` | 300|sets duration of sliding effect
`pause` | 3000|pause duration
`autoplay` | null|set to `on` to turn on autoplay
`ratio` | null|set to `keep` to keep aspect ratio when window resizes
`ulClass` | `slides-wrapper`|specifies class of the `ul` element
`nextClass` | `sl-next`|specifies class of the element showing next slide
`prevClass` | `sl-prev`|specifies class of the element showing previous slide