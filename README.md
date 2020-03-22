# particles.js-es

[![npm version][npm-version-src]][npm-version-href]
[![npm downloads][npm-downloads-src]][npm-downloads-href]
[![Circle CI][circle-ci-src]][circle-ci-href]
[![Codecov][codecov-src]][codecov-href]
[![License][license-src]][license-href]


[📖 **Release Notes**](./CHANGELOG.md)

## Setup

1. Add `particles.js-es` dependency to your project

```bash
yarn add particles.js-es # or npm install particles.js-es
```

## Usage

```js
import PJS from 'particles.js-es'
import options from 'your/options/file.json' // json file
// or
import options from 'your/options/file' // js file
// or
const options = {
  particles: {
    number: {
      value: 20,
      density: {
        enable: true,
        value_area: 200
      }
    }
  }
  // ...
}

// Init
PJS.init('#myElement', options)
// Refresh
PJS.refresh('#myElement', options)
// Destroy
PJS.destroy('#myElement')
```

## options

You can generate usage ready options object with a cool WYSIWYG tool on @VincentGarreau's website: [https://vincentgarreau.com/particles.js/](https://vincentgarreau.com/particles.js/)

```js
{
  "particles": {
    "number": {
      "value": 80,
      "density": {
        "enable": true,
        "value_area": 800
      }
    },
    "color": {
      "value": "#ffffff"
    },
    "shape": {
      "type": "circle",
      "stroke": {
        "width": 0,
        "color": "#000000"
      },
      "polygon": {
        "nb_sides": 5
      },
      "image": {
        "src": "img/github.svg",
        "width": 100,
        "height": 100
      }
    },
    "opacity": {
      "value": 0.5,
      "random": false,
      "anim": {
        "enable": false,
        "speed": 1,
        "opacity_min": 0.1,
        "sync": false
      }
    },
    "size": {
      "value": 10,
      "random": true,
      "anim": {
        "enable": false,
        "speed": 80,
        "size_min": 0.1,
        "sync": false
      }
    },
    "line_linked": {
      "enable": true,
      "distance": 300,
      "color": "#ffffff",
      "opacity": 0.4,
      "width": 2
    },
    "move": {
      "enable": true,
      "speed": 12,
      "direction": "none",
      "random": false,
      "straight": false,
      "out_mode": "out",
      "bounce": false,
      "attract": {
        "enable": false,
        "rotateX": 600,
        "rotateY": 1200
      }
    }
  },
  "interactivity": {
    "detect_on": "canvas",
    "events": {
      "onhover": {
        "enable": false,
        "mode": "repulse"
      },
      "onclick": {
        "enable": true,
        "mode": "push"
      },
      "resize": true
    },
    "modes": {
      "grab": {
        "distance": 800,
        "line_linked": {
          "opacity": 1
        }
      },
      "bubble": {
        "distance": 800,
        "size": 80,
        "duration": 2,
        "opacity": 0.8,
        "speed": 3
      },
      "repulse": {
        "distance": 400,
        "duration": 0.4
      },
      "push": {
        "particles_nb": 4
      },
      "remove": {
        "particles_nb": 2
      }
    }
  },
  "retina_detect": true
}
```

[MIT License](./LICENSE)

Copyright (c) pirony <romainpouchol@gmail.com>

<!-- Badges -->
[npm-version-src]: https://img.shields.io/npm/v/particles.js-es/latest.svg?style=flat-square
[npm-version-href]: https://npmjs.com/package/particles.js-es

[npm-downloads-src]: https://img.shields.io/npm/dt/particles.js-es.svg?style=flat-square
[npm-downloads-href]: https://npmjs.com/package/particles.js-es

[circle-ci-src]: https://img.shields.io/circleci/project/github/pirony/particles.js-es.svg?style=flat-square
[circle-ci-href]: https://circleci.com/gh/pirony/particles.js-es

[codecov-src]: https://img.shields.io/codecov/c/github/pirony/particles.js-es.svg?style=flat-square
[codecov-href]: https://codecov.io/gh/pirony/particles.js-es

[license-src]: https://img.shields.io/npm/l/particles.js-es.svg?style=flat-square
[license-href]: https://npmjs.com/package/particles.js-es
