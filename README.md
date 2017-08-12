# bulma-timeline
Bulma's extension to display a timeline (find all my bulma's extensions [here](https://github.com/Wikiki/bulma-extensions))

<img src="https://img4.hostingpics.net/pics/887099ScreenShot20170812at150229.png" width="50%">

Usage
---

```html
<ul class="timeline">
  <li class="timeline-header">
    <span class="button is-primary">Start</span>
  </li>
  <li class="timeline-item is-warning">
    <div class="timeline-tag"></div>
    <div class="timeline-content">
      <p class="heading">January 2016</p>
      <p>Timeline content - Can include any HTML element</p>
    </div>
  </li>
  <li class="timeline-item is-danger">
    <div class="timeline-tag is-icon">
      <figure class="image is-32x32">
        <img src="http://bulma.io/images/placeholders/32x32.png">
      </figure>
    </div>
    <div class="timeline-content">
      <p class="heading">February 2016</p>
      <p>Timeline content - Can include any HTML element</p>
    </div>
  </li>
  <li class="timeline-header">
    <span class="button is-primary">2017</span>
  </li>
  <li class="timeline-item">
    <div class="timeline-content">
      <p class="heading">March 2017</p>
      <p>Timeline content - Can include any HTML element</p>
    </div>
  </li>
  <li class="timeline-header">
    <span class="button is-primary">End</span>
  </li>
</ul>
```

Variables
---
This extension uses Bulma's color modifiers and have the following variables

Name | Description | Default value    
-----|-------------|---------------
$timeline-tag-background-color | Background color of item tag | $white
$timeline-tag-border | Size and default color of item tag | .1em solid $grey-light
$timeline-line | Line style of the timeline | .1em solid $grey-light
$timeline-content-padding | Content padding for items spacing | 1em 0 0 2em

Demo
---
You can find a demo [here](https://codepen.io/wikiki/pen/zdwjqL)

Integration
---
- Clone the [bulma repo](https://github.com/jgthms/bulma)
- Under the `sass` folder, create a new folder called `extensions`
- In this new folder, create a new file `timeline.sass`
- Copy the code form the `bulma-timeline repo`'s [timeline.sass](https://github.com/Wikiki/bulma-timeline/blob/master/timeline.sass) file into your new file
- In the same folder create a new file `_all.sass` (this is not required, but will help when you add more extensions)
- In this file add this code:
```
@charset "utf-8"
@import "timeline.sass"
```
At the end of the `bulma.sass` file, add this line: `@import "sass/extensions/_all"`

Now, you can just build the bulma project with `npm run build`, and the output will be available in the `css folder`.
