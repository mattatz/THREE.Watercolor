THREE.Watercolor
=====================

Watercolor effects for three.js.

![sample](https://raw.githubusercontent.com/mattatz/THREE.Watercolor/master/Captures/watercolored.png)

## Usage

This effect relies on THREE.EffectComposer and you need to pass a paper texture.

```javascript
var composer = new THREE.EffectComposer();
composer.addPass(new THREE.RenderPass(scene, camera));

var paper = new THREE.ImageUtils.loadTexture(pathToPaperTexture);
var watercolorPass = new THREE.WatercolorPass(paper);
composer.addPass(watercolorPass);

composer.render();
```

## Example

Origin.
![origin](https://raw.githubusercontent.com/mattatz/THREE.Watercolor/master/Captures/origin.png)

Toon shaded.
![toon](https://raw.githubusercontent.com/mattatz/THREE.Watercolor/master/Captures/toonshaded.png)

Watercolored.
![result](https://raw.githubusercontent.com/mattatz/THREE.Watercolor/master/Captures/watercolored.png)

## Demo

[Demo](https://mattatz.github.io/THREE.Watercolor)

## Sources

- Real-Time rendering of watercolor effects for virtual environments - http://dl.acm.org/citation.cfm?id=2131253

- Charlotte Hoare MSc Project : http://nccastaff.bournemouth.ac.uk/jmacey/MastersProjects/MSc12/Hoare/index.html 

