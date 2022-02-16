# fusibile

Modified fusibile version for [MVSNet](https://github.com/YoYo000/MVSNet) post-processing, which produces similar point cloud results to paper: 

[MVSNet: Depth Inference for Unstructured Multi-view Stereo](https://arxiv.org/abs/1804.02505), ECCV 2018

The original source code is for the paper:

[Massively Parallel Multiview Stereopsis by Surface Normal Diffusion](http://www.prs.igp.ethz.ch/content/dam/ethz/special-interest/baug/igp/photogrammetry-remote-sensing-dam/documents/pdf/galliani-lasinger-iccv15.pdf), ICCV 2015

## Compile Step For Ubunt 20.04 RTX 3080 CUDA 11.4

sudo apt-get install mesa-common-dev
sudo apt-get install libgl1-mesa-dev libglu1-mesa-dev

cmake -DCUDA_TOOLKIT_ROOT_DIR=/usr/local/cuda-11.5/ -DCMAKE_C_COMPILER=gcc-10 -DCMAKE_CXX_COMPILER=g++-10 .
make


