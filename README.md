# DT-SAM

Welcome to the GitHub repository for the implementation code of my Master's Thesis. This repository contains all the code and resources used in my thesis titled 'DT-SAM: Optimizing SAM for Specialized Domains and Tasks'.


                                            

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
You should download the SAM checkpoints from [hugging face link]([hugging face link](https://huggingface.co/sam-hq-team/sam-hq-training/tree/main/pretrained_checkpoint))

## Train

To Train DT-SAM 
```
python train.py --checkpoint <path/to/sam_checkpoint> --model-type <model_type> --output <path/to/output>
```

## Evaluation

To evaluate DT-SAM

```
python train.py --checkpoint <path/to/sam_checkpoint> --model-type <model_type> --output <path/to/output> --eval --restore-model <path/to/dtsam_checkpoint>
```
