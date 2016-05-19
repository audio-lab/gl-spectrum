# gl-spectrum [![unstable](http://badges.github.io/stability-badges/dist/unstable.svg)](http://github.com/badges/stability-badges)

Spectrum rendering component.

[![Spectrum](https://raw.githubusercontent.com/audio-lab/gl-spectrum/gh-pages/preview.png "Spectrum")](http://audio-lab.github.io/gl-spectrum/)

## Usage

[![npm install gl-spectrum](https://nodei.co/npm/gl-spectrum.png?mini=true)](https://npmjs.org/package/gl-spectrum/)

```js
var Spectrum = require('gl-spectrum');

var spectrum = new Spectrum({
	container: document.body,
	canvas: canvas,
	context: 'webgl',

	frequencies: frequenciesData,

	maxDecibels: 0,
	minDecibels: -100,

	maxFrequency: 20000,
	minFrequency: 20,

	sampleRate: 44100,
	logarithmic: true,

	smoothing: 0.5,

	grid: true,
	gridAxes: false,

	colormap: 'jet',

	//WIP shadow frequencies
	shadow: [],

	//WIP
	style: 'line'
});

spectrum.setFrequencies(frequencies);
```

## Related

* [colormap](https://github.com/bpostlethwaite/colormap) — list of js color maps.
* [cli-visualizer](https://github.com/dpayne/cli-visualizer) — C++ spectrum visualizer.