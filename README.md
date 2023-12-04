# DTSAM

Welcome to the GitHub repository for the implementation code of my Master's Thesis. This repository contains all the code and resources used in my thesis titled 'Adapting Segment Anything Model for Industrial Image Segmentation'.


## Usage

I organize the folder as follows.

````
DTSAM
|___data
|___pretrained_checkpoint
|___utils
|___segment_anything_DT
|___work_dirs
|___train.py
````

## Train

To Train DT-SAM 
```
python train.py --checkpoint <path/to/checkpoint> --model-type <model_type> --output <path/to/output>
```

## Evaludation

To evaluate DT-SAM

```
python train.py --checkpoint <path/to/checkpoint> --model-type <model_type> --output <path/to/output> --eval --restore-model <path/to/training_checkpoint>
```