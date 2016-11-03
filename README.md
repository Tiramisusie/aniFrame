# aniFrame

get the compatible version of requestAnimationFrame

## how to use

```js
import { nextFrame, cancelFrame } from 'aniFrame'

var frame;

function step(timestamp) {
  element.style.left = timestamp + 'px';
  frame = nextFrame(step);
}

frame = nextFrame(step);

// cancel
cancelFrame(frame);
