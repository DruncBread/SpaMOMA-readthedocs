# Installation

## 1. Clone SpaMOMA from GitHub

You can download **SpaMOMA** using `git clone`:

``` bash
git clone https://github.com/XiangyuLi-Lab/SpaMOMA.git
cd SpaMOMA
```

------------------------------------------------------------------------

## 2. Create a Virtual Environment

``` bash
conda create -n spamoma python=3.9
conda activate spamoma
```

------------------------------------------------------------------------

## 3. Install Dependencies

``` bash
pip install -r requirements.txt
```
## Tutorial runtime

Start Jupyter with the repository root as the working directory. The omics clustering examples use R with the `mclust` package through `rpy2`. The MISAR-seq resolution-enhancement example reads torchvision's ImageNet ResNet-50 weights. For offline use, provide `resnet50-0676ba61.pth` in the Torch Hub checkpoints cache. The two official registration weights go in `SpaMOMA/check_points/` as described in the project README.

The demonstration notebooks read the raw data from `datasets/` and write derived data to `SpaMOMA_output/`. The `coarse_gpu` and `fine_gpu` options use the GPU indices visible to the notebook process.

On a host that shares one notebook kernel between TensorFlow 2.14 (CUDA 11.8) and a newer CUDA build of PyTorch, the PyTorch cuSOLVER directory must precede the TensorFlow CUDA libraries in the loader path. The server checkout provides an environment-local Jupyter kernel called **SpaMOMA C100/F120** with this ordering. From the repository root, launch it with:

```bash
JUPYTER_PATH="$PWD/.venv/share/jupyter" .venv/bin/python -m jupyterlab
```

Select **SpaMOMA C100/F120** when opening a tutorial. For a newly cloned checkout, use the Python environment in which you installed the project dependencies.
