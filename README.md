# Three.js渲染SketchUp开发web 3D

> English summary: a Three.js web viewer for SketchUp models. Export a model from SketchUp as `.dae` (Collada), load it with Three.js and `ColladaLoader.js`, or publish it through the Three.js online editor. The repo includes `index.html`, `js/`, `libs/`, and a `demo.dae` sample model.

## Run locally

Serve this folder with any static file server and open `index.html`:

```bash
python3 -m http.server
# then open http://localhost:8000
```

Opening the file directly can block model loading in some browsers, so a local server is recommended.


## 方法一

### 1. 用SketchUp制作模型，并导出为.dae文件

### 2.导入所需库文件

```
<script type="text/javascript" src="./libs/three.js"></script>
<script type="text/javascript" src="./libs/ColladaLoader.js"></script>
```

这里的ColladaLoader.js并不包含在three.js文件里面，需要单独应用。

​          

## 方法二

### 通过在线工具  https://threejs.org/editor/

导入3D模型文件，在线配置效果，效果满意后publish，会自动生成对应的工程包，直接部署即可。

推荐第二种方法。