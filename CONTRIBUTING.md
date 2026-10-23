# Contributing to threejs-sketchup-web-viewer

## Test locally

Serve this folder with any static file server and open `index.html`:

```bash
python3 -m http.server
# then open http://localhost:8000
```

Confirm the bundled `demo.dae` model loads and can be orbited. Browsers can block model loading from `file://`, so always test through the server.

## Adding a model

Export from SketchUp as `.dae` (Collada), or publish a configured scene through the Three.js editor as described in the README. Keep `libs/` loader changes minimal, since `ColladaLoader.js` is loaded separately from `three.js`.

## Pull requests

Create a branch from `master` and say which model and browser you tested with in the PR.
