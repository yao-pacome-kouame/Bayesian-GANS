# Bayesian Generative Adversarial Networks Project

This project proposes a Pytorch implementation of the [Bayesian GAN](https://arxiv.org/abs/1705.09558) presentend by Wilson et al. at NeurIPS 2017.

## Project tree
The code folder is organized as follows :

Bayesian-GANS:
- bgan.py
- download_dataset.py
- Opt.py
- Readme.md
- requirements.txt

## Prerequisite

To replicate the results you will need the following modules :
- pytorch
- numpy
- scikit-learn
- scipy
- opencv-python
- gdown

To install them we recommend you to use the file requirements.txt which is in this folder by doing from a Terminal or a Command Prompt:
cd BayesianProject_BGAN
pip install -r requirements.txt

## Run
To replicate the results run the script as follows from a Terminal or a Command Prompt:

- For execute Bayesian GAN : python bgan.py mnist normal SGHMC 1

- For execute classical Deep Convolutionnal GAN : python bgan.py mnist normal SGHMC 0

## Nota

It is important to keep in mind that the training takes a lot of time and that a computer with GPU-CUDA is required for time optimisation. Else, to make sure that the user can execute the code in a reasonable time on CPU, we have fixed the number of epochs to train the network to 30 while others say that it is from 350 epochs that the generation of images almost correct and not a noise. You can change this number in the script bgan.py at line 41.
