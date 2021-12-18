# react-carousel-infinite

### Installation
**npm**

```bash
npm install react-carousel-infinite --save
```

**yarn**

```bash
yarn add react-carousel-infinite
```

### [Example](https://g787543.github.io/infinite-react-carousel/)
```js
import React from 'react';
import Slider from 'react-carousel-infinite';

const SimpleSlider = () => (
  <Slider dots>
    <div>
      <h3>1</h3>
    </div>
    <div>
      <h3>2</h3>
    </div>
    <div>
      <h3>3</h3>
    </div>
    <div>
      <h3>4</h3>
    </div>
    <div>
      <h3>5</h3>
    </div>
  </Slider>
);
```

### Props

| Prop | Description | Default | Type |
|------|-------------|---------|------|
| rows | Number of rows per slide in the slider, (enables grid mode) | 1 | Number |
| slidesPerRow | Number of slides to display in grid mode, this is useful with rows option | 1 | Number |
| slidesToShow | How many slides to show in one frame | 1 | Number |
| className |  | "" | String |
| centerMode | Center current slide | false | Boolean |
| swipe | Enable/disable swiping to change slides | true | Boolean |
| adaptiveHeight | Adjust the slide's height automatically | false | Boolean |
| centerPadding |  | 50 | String, Number |
| initialSlide | Index of first slide | false | Boolean, Number |
| pauseOnHover | Prevents autoplay while hovering on track | true | Boolean |
| autoplay | Enable/disable slider autoplay | false | Boolean |
| autoplayScroll | How many slides to scroll when autoplay is true | 1 | Number |
| autoplaySpeed | Delay between each auto scroll (in milliseconds) | 3000 | Number |
| beforeChange | Before Index change callback. `(oldIndex, newIndex) => ...` | null | Function |
| afterChange | Index change callback. `index => ...` | null | Function |
| duration | Transition duration in milliseconds | 200 | Number |
| shift | Set the spacing of the center item | 0 | Number |
| arrows | Enable/disable arrow button | true | Boolean |
| arrowsBlock |  | true | Boolean |
| arrowsScroll | How many slides to scroll when click arrows button | 1 | Number |
| prevArrow | Custom prev arrows button | null | Element |
| nextArrow | Custom next arrows button | null | Element |
| dots | Enable/disable dots | false | Boolean |
| dotsClass | CSS class for dots | "carousel-dots" | String |
| dotsScroll | How many slides to scroll on one page | 1 | Number |
| appendDots | Custom dots templates. Works same as customPaging | ```(dots) => <ul style={{ display: 'block' }}>{dots}</ul>``` | Function |
| customPaging | Custom paging templates | ```(i) => <button type="button">{i + 1}</button>``` | Function |
| onReszie | detect carousel resize | ```(e) => {}``` | Function |
| onSwipe | Callback after slide changes by swiping | ```(direction) => {}``` | Function |
| accessibility | Enable tabbing and arrow key navigation | true | Boolean |
| wheel | Enable mouse wheel to slide item | false | Boolean |
| wheelScroll | How many slides to scroll when wheel trigger | 1 | Number |
| virtualList |  | false | Boolean |
| overScan | Number of items to render before/after the visible slice of the carousel | 2 | Number |

### Methods

| Name | Description |
|------|-------------|
| slickNext | Go to the next slide |
| slickPrev | Go to the previous slide |
| slickGoTo | Go to any slide |
| slickPause | Pause the autoplay |
| slickPlay | Start the autoplay |

### Development

Want to run demos locally

***npm***
```bash
npm install
npm run dev
```

***yarn***
```bash
yarn
yarn dev
```
open http://localhost:8080


### LICENSE

The project is licensed under the terms of [MIT license](https://github.com/g787543/infinite-react-carousel/blob/master/LICENSE)
