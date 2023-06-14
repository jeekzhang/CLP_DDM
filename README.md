# CLIP_DDM
——Distinguish duck or mouse with CLIP

## Usage
First, install PyTorch 1.7.1 (or later) and torchvision, as well as small additional dependencies, and then install this repo as a Python package. On a CUDA GPU machine, the following will do the trick:
```bash
$ conda install --yes -c pytorch pytorch=1.7.1 torchvision cudatoolkit=11.0
$ pip install ftfy regex tqdm
$ pip install git+https://github.com/openai/CLIP.git
```
Replace cudatoolkit=11.0 above with the appropriate CUDA version on your machine or cpuonly when installing on a machine without a GPU.

## Run
```bash
python main.py
```

## Output
```
It is a mouse
The probs of duck neck:  0.0012033392
The probs of a mouse:  0.9987966
```
