# Deep Dimension Reduction for Supervised Representation Learning

This repository is the official implementation of [Deep Dimension Reduction for Supervised Representation Learning]. 

## Requirements

To install requirements:

```setup
pip install -r requirements.txt
```

## Training

To train DDR on toy examples, run this command:

```train_toys
python demo_toys.py --save 'Results/toys' --dataset 3
```

To train DDR on MNIST dataset and get the evaluation results , run this command:

```train
python train.py --save 'Results/MNIST' --latent_dim 16
```

## Evaluation

To evaluate DDR on MNIST, run:

```eval
python eval.py --path 'Results/MNIST' --latent_dim 16
```


## Pre-trained Models

DDR does not adopt the pre-trained models. However, to save the time and expense of training, we provied the trained models that can aviod the afresh training. To evaluate DDR on MNIST with trained models, run:

```eval_trained
python eval.py --path 'Results/MNIST_trained_16' --latent_dim 16
```

## Results

Our model DDR achieves the following performance on :

### [Image Classification on MNIST]

| Reduced Dimension|   16   |   32   |   64   |
| ---------------- |--------|--------|--------|
|        DDR       | 99.63% | 99.63% | 99.63% |
