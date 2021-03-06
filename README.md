# Automorphic Equivalence-aware Graph Neural Network

This repository holds an implementation of [Automorphic Equivalence-aware Graph Neural Network](https://arxiv.org/abs/2011.04218) NeurIPS 2021. 

![alt text](https://github.com/AutoML-Research/GRAPE/blob/main/main.png?raw=true)

## Dependencies

This implementation depends on the following enviornment and packages:

```setup
python == 2.7
pytorch == 1.4
numpy == 1.17.2
scipy == 1.6.3
sklearn ==0.24.1
h5py == 2.9.0
GPUtil ==1.4.0
setproctitle == 1.1.10
```

## Training and Evaluation

To train and evaluate the model(s) in the paper, run this command:

```train
python grape_model.py --data='cite|cora' --gpu='0' --lr=0.003 --wd=0.00003 --dropout=0.5 --hid=32 
```

## Results

Our model achieves the following classification accuracy:


|  | Hamilton | Lehigh | Rochester | JHU | Amherst | Cora | Citeseer | Amazon |
| ------------------ |---------------- | -------------- | ---------------- | -------------- | ---------------- | -------------- | ---------------- | -------------- |
|  GRAPE  | 28.1% | 27.3% | 25.0% | 34.6% | 32.6% | 87.1% | 74.6% | 58.6% |

