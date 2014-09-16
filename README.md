# Vocoder

This is a port of Chris Wilson's [Vocoder](https://github.com/cwilso/Vocoder)
project with all the UI stripped out and modified to work with Browserify.

Basically, you can control the pitch of a vocal track. `(ﾉ◕ヮ◕)ﾉ*:･ﾟ✧ M A G I C AL (ಥ﹏ಥ)`


## Installation

```bash
npm install --save vocoder
```

## Usage

###`function vocoder(audioContext, carrierBuffer, modulatorBuffer)`

Start the vocoder playing the `modulatorBuffer` mixed in with the `carrierBuffer`.
These are both AudioBuffers.

## Example
```javascript
var vocoder = require('vocoder');
var load = require('webaudio-buffer-loader');

var ctx = new AudioContext();

load(['/carrier.ogg', '/modulator.ogg'], ctx, function(err, buffers) {
});
```
