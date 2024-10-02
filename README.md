# Fast-DSAGCN

A PyTorch implementation of [Fast-DSACGN]


## Table of Contents
- <a href='#installation'>Installation</a>
- <a href='#datasets'>Datasets</a>
- <a href='#training-fast-dsagcn'>Train</a>
- <a href='#evaluation'>Evaluate</a>

## Installation
- Python 3.x. Recommended using [Anaconda3](https://www.anaconda.com/distribution/)
- [PyTorch 1.0](https://pytorch.org/get-started/locally/). Install PyTorch by selecting your environment on the website and running the appropriate command. Such as:
  ```
  conda install pytorch torchvision cudatoolkit=9.0 -c pytorch
  ```
- Clone this repository.
- Download the dataset by following the [instructions](#datasets) below.
- Note: For training, we currently support [cityscapes](https://www.cityscapes-dataset.com/)

## Datasets
- You can download [cityscapes](https://www.cityscapes-dataset.com/) from [here](https://www.cityscapes-dataset.com/downloads/). Note: please download [leftImg8bit_trainvaltest.zip(11GB)](https://www.cityscapes-dataset.com/file-handling/?packageID=4) and [gtFine_trainvaltest(241MB)](https://www.cityscapes-dataset.com/file-handling/?packageID=1).

## Training-Fast-DSAGCN
- By default, we assume you have downloaded the cityscapes dataset in the `./datasets/citys` dir.
- To train Fast-SCNN using the train script the parameters listed in `train.py` as a flag or manually change them.
```Shell
python train.py --model fast_dsagcn --dataset citys
```

## Evaluation
To evaluate a trained network:
```Shell
python eval.py
```
``



