---
title: Dropdown
description: Dropdown panes are little happy sprites which can be revealed on click or hover.
sass: scss/components/_dropdown.scss
js: js/foundation.dropdown.js
video: '0F68zptD_nQ'
---

<div class="primary callout">
  <p>You might be looking for <a href="dropdown-menu.html">dropdown menus</a>, which are a separate plugin.</p>
</div>

## Basics

To create a dropdown pane, add the class `.dropdown-pane` and the attribute `data-dropdown` to an element. Give the dropdown a unique ID as well.

To create the dropdown trigger, add `data-toggle` to a `<button>`. The value of `data-toggle` is the ID of the dropdown.

<p>
  <a class="" data-open-video="0:47"><img src="{{root}}assets/img/icons/watch-video-icon.svg" class="video-icon" height="30" width="30" alt=""> Watch this part in video</a>
</p>

<div class="docs-codepen-container">
  <a class="codepen-logo-link" href="https://codepen.io/IamManchanda/pen/NjzByp?editors=1000" target="_blank"><img src="{{root}}assets/img/logos/edit-in-browser.svg" class="" height="" width="" alt="edit on codepen button"></a>
</div>


```html_example
<button class="button" type="button" data-toggle="example-dropdown">Toggle Dropdown</button>
<div class="dropdown-pane" id="example-dropdown" data-dropdown data-auto-focus="true">
  Example form in a dropdown.
  <form>
    <div class="row">
      <div class="medium-6 columns">
        <label>Name
          <input type="text" placeholder="Kirk, James T.">
        </label>
      </div>
      <div class="medium-6 columns">
        <label>Rank
          <input type="text" placeholder="Captain">
        </label>
      </div>
    </div>
  </form>
</div>


<button class="button" type="button" data-toggle="example-dropdown-1">Hoverable Dropdown</button>
<div class="dropdown-pane" id="example-dropdown-1" data-dropdown data-hover="true" data-hover-pane="true">
  Just some junk that needs to be said. Or not. Your choice.
</div>
```

---

## Positioning

By default, a dropdown anchors below the button that opened it. Add the class `.top`, `.right`, or `.bottom` to the dropdown to change this.

<div class="docs-codepen-container">
  <a class="codepen-logo-link" href="https://codepen.io/IamManchanda/pen/YVvjvz?editors=1000" target="_blank"><img src="{{root}}assets/img/logos/edit-in-browser.svg" class="" height="" width="" alt="edit on codepen button"></a>
</div>

```html_example
<button class="button" type="button" data-toggle="example-dropdown2">Top Aligned</button>

<div class="dropdown-pane top" id="example-dropdown2" data-dropdown>
  Just some junk that needs to be said. Or not. Your choice.
</div>
```

<button class="button" type="button" data-toggle="example-dropdown3" style="float: right;">Left Aligned</button>
<div class="dropdown-pane left" id="example-dropdown3" data-dropdown>
  Just some junk that needs to be said. Or not. Your choice.
</div>

<button class="button" type="button" data-toggle="example-dropdown4">Right Aligned</button>
<div class="dropdown-pane right" id="example-dropdown4" data-dropdown>
  Just some junk that needs to be said. Or not. Your choice.
</div>


Adding `.float-right` or `.float-left` to the anchor will change the direction of the dropdown as well.

<button class="button float-right" type="button" data-toggle="example-dropdown5">Bottom-right Aligned</button>
<div class="dropdown-pane bottom" id="example-dropdown5" data-dropdown>
  Just some junk that needs to be said. Or not. Your choice.
</div>

<button class="button float-left" type="button" data-toggle="example-dropdown6">Bottom-left Aligned</button>
<div class="dropdown-pane bottom" id="example-dropdown6" data-dropdown>
  Just some junk that needs to be said. Or not. Your choice.
</div>
