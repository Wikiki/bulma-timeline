# bulma-timeline
Bulma's extension to display a timeline

Preview
---
![Timeline Component](https://img15.hostingpics.net/pics/440691ScreenShot20170719at120241.png)

Usage
---
This extension uses Bulma's color modifiers and have the following variables
             Name             |                                                Description                                               |     Default value    
----------------------------|--------------------------------------------------------------------------------------------------------|--------------------
 $timeline-icon-border-radius | Define the icon (on left) border radius. This allow you do create a square or rounded timeline item icon |         .5rem        
 $timeline-line-color         | Color of line in background of icons                                                                     |     $grey-lighter    
 $timeline-line-width         | Width of line in background of icons                                                                     |         .2rem        
 $timeline-content-padding    | Padding for item content                                                                                 | .2rem 0 .2rem 1.5rem

```html
<div class="timeline">
  <div class="timeline-item" id="timeline-example-1">
    <div class="timeline-left icon-lg">
      <a href="#timeline-example-1" class="timeline-icon"></a>
    </div>
    <div class="timeline-content">
      <div class="level">
        <div class="level-left">
          <div class="level-item">
            <div>
              <p class="heading">January 2017</p>
              <p>Timeline content - Can include any HTML element</p>
            </div>
          </div>
          <div class="level-right">
            <p class="level-item"><button class="button is-primary is-small">View</button></p>
          </div>
        </div>
      </div>
    </div>
  </div>
  <div class="timeline-item" id="timeline-example-2">
    <div class="timeline-left">
      <a href="#timeline-example-2" class="timeline-icon icon-lg">
          <i class="icon fa fa-check"></i>
        </a>
    </div>
    <div class="timeline-content">
      <div class="level">
        <div class="level-left">
          <div class="level-item">
            <div>
              <p class="heading">February 2017</p>
              <p>Timeline content - Can include any HTML element</p>
            </div>
          </div>
          <div class="level-right">
            <p class="level-item"><button class="button is-primary is-small">View</button></p>
          </div>
        </div>
      </div>
    </div>
  </div>
  <div class="timeline-item" id="timeline-example-3">
    <div class="timeline-left">
      <a href="#timeline-example-3" class="timeline-icon icon-lg">
          <i class="icon fa fa-check"></i>
        </a>
    </div>
    <div class="timeline-content">
      <div class="level">
        <div class="level-left">
          <div class="level-item">
            <div>
              <p class="heading">March 2017</p>
              <p>Timeline content - Can include any HTML element</p>
            </div>
          </div>
          <div class="level-right">
            <p class="level-item"><button class="button is-primary is-small">View</button></p>
          </div>
        </div>
      </div>
    </div>
  </div>
```

Demo
---
You can find a demo [here](https://codepen.io/anon/pen/MvJKrR)

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
