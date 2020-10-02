# Toward Understanding  Supervised Representation Learning with RKHS and GAN

This repository is the demo implementation of [novel supervised representation learning approach (NSRL)]. 

## Requirements

To install requirements:

```setup
pip install -r requirements.txt
```

## Training and evaluation

To train NSRL on toy examples to visualize learned features, run this command:

```train_toys
python simulation/demo.py --save 'simulation/Results/S_curve'
```

To train NSRL on MNIST and Kuzushiji-MNIST dataset and get the evaluation results , run this command:

```train_mnist
python classification/demo.py --save 'classification/Results/MNIST' --dataset 'mnist' --latent_dim 8
```
```train_kmnist
python classification/demo.py --save 'classification/Results/KMNIST' --dataset 'kmnist' --latent_dim 8
```

## Results

Our model NSRL achieves the following performance on :

### [Image Classification on MNIST and Kuzushiji-MNIST]

| Reduced Dimension|   8   |   16   |   32   |
| ---------------- |--------|--------|--------|
|        MNIST       | 99.67% | 99.66% | 99.62% |
|        Kuzushiji-MNIST       | 98.61% | 98.81% | 98.63% |

### [Trained models]

All results for classification on MNIST and Kuzushiji-MNIST are saved in 'classification/Results'.
