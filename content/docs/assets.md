---
title: "Assets"
---


## Functions

::list

::method-info
#method
loadImage
#overridings
(url: [string]{.ts-base}, options?: [SurfaceCreateOptions]{.ts-type-intf}) ⇨ [Promise]{.ts-class}<[Surface]{.ts-class}>
#description
Loads an image by url and create instance of a the surface object
#example
<br>Example:
```ts
async function loadAssets () {
  const image = await loadImage('https://example.com/image.jpg', { useAlpha: false })
  ...
}
```
::

::method-info
#method
loadBlob
#overridings
(blob: [Blob]{.ts-class}, options?: [SurfaceCreateOptions]{.ts-type-intf}) ⇨ [Promise]{.ts-class}<[Surface]{.ts-class}>
#description
Loads an image from BLOB and create instance of the surface object
#example
<br>Example:
```ts
async function onFileUpload (ev: Event) {
  const files = ev.target.files
  if (!files || !files[0]) return
  
  const image = await loadBlob(files[0])
  ...
}
```
```html
...
<input type="file" onchange="onFileUpload">
...
```
::

::method-info
#method
loadTileMap
#overridings
(tileWidth: [number]{.ts-base}, titleHight: [number]{.ts-base}, url: [string]{.ts-base}, options?: [TileMapInitOptions]{.ts-type-intf}) ⇨ [Promise]{.ts-class}<[TileMap]{.ts-class}>
#description
Loads an tilemap by url and create instance of the TileMap object
::

::method-info
#method
createTileMap
#overridings
(tileWidth: [number]{.ts-base}, titleHight: [number]{.ts-base}, urls: [string]{.ts-base}\[], rows: [number]{.ts-base}, cols: [number]{.ts-base}, options?: [TileMapInitOptions]{.ts-type-intf}) ⇨ [Promise]{.ts-class}<[TileMap]{.ts-class}>
#description
Creates an tilemap from image files and create instance of the TileMap object
::

::