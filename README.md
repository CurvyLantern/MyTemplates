# MyTemplates
HERE I UPLOAD THING THAT I NEED 
you can use it like this :

```JS
import { OutCubeCam } from './OutCubeCam'

const cubeRenderTarget = new THREE.WebGLCubeRenderTarget(256, {
  encoding: THREE.sRGBEncoding,
})

// Parameters : width of the cube , near , renderTarget
const outCubeCam = new OutCubeCam(3, 0.01, cubeRenderTarget)
for (let i = 0; i < outCubeCam.children.length; i++) {
  const helper = new THREE.CameraHelper(outCubeCam.children[i])
  scene.add(helper)
}
console.log(outCubeCam)
console.log(outCubeCam.children)

outCubeCam.update(renderer, scene)
```
