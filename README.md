# Sparser-Splat: Sparser Gaussian Splatting

## Installation Instructions

## The installation instructions assumes you have installed [Nerfstudio](https://docs.nerf.studio/quickstart/installation.html).

### 1. Clone this repo.
`git clone git@github.com:chengine/sparse_splat.git`

### 2. Install `sparse_splat` as a python package once you `cd` into the `sparse_splat` repository.
`python -m pip install -e .`

## 3. Register `sparse_splat` with Nerfstudio.
`ns-install-cli`

### Now, you can run `sparse_splat` like other models in Nerfstudio using the `ns-train sparse_splat` command.
### For example:
```python 
ns-train sparse_splat --data <path to the data> \
    --output-dir <path to the output directory> \
    --pipeline.model.camera-optimizer.mode SO3xR3 \
    --pipeline.model.rasterize-mode antialiased
```

