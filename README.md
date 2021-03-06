# Domain-Adaptation-Using-Convolutional-AutoEncoder
In this repository, I implemented the domain Adaptation problem in Manet Dataset using Convolutional Autoencoder.

## Table of contents
* [Task Description](#TaskDescription)
* [Requirements](#Requirements)
* [Instruction](#Instruction)
* [Acknowledgement](#Acknowledgement)


## Task Description
The dataset consist of Paired landscape and Monet-Stylized image from kaggle-set A(https://bit.ly/3l33Wiy) training image pairs.
The image pairs consists of image and the landscape paintings
The task is to adapt images from one domain to another.

Hyperparameter Optimisation was done using Optuna(https://optuna.org/)

Folder structure
--------------
```
Monet-styled-dataset
├──  Original_A       - this folder contains landscapes images.
│   ├── image1.jpeg
│   └── --------------------
│
├── Original_B      - this folder contains monet styled painting images.
│   ├── image2.jpeg
│   └── --------------------  
│   
│── Autoencoder-Baseline-mit-optuna.ipynb - this notebook contains  python scripts with visualisation
│   
├──  autoencoder_best_model.h5       - this model can be used directly for converting landscape image to paintings.
│
├── model.py
│
└── app.py 
│
├──datasets
│
├──static
└── templates



```

## Requirements
1. Flask
2. Python
3. Keras
4. Optuna


```bash
pip install requirements.txt
```

## Instruction
```bash
python app.py
```
## Acknowledgment

The basline borrows heavily from the following Github Link(https://bit.ly/3evvN9U) and youtube page(https://bit.ly/3bzUvEn).
