# RRDPM：Relay Residual Diffusion Probabilistic Model for global typical land and seabed DEM super-resolution

This is a diffusion-based super-resolution model, RRDPM, which incorporates two distinct reverse process patterns: residual prediction pattern and noise prediction pattern. Furthermore, we discover a symmetry in their error propagation. Capitalizing on this discovery, we design a relay sampling mechanism. in which the sampling process is relayed by two different sampling formulas, and Figure 1  illustrates the schematic diagram of RRDPM. To ensure that the LR and HR dimensions are the same, the nearest interpolation process is pre-applied to the LR.
![Figure 1. Schematic diagram of RRDPM ](https://github.com/SuperChen100/RRDPM/blob/main/img/img.png)


This model consists of a total of three algorithms, corresponding to the three.ipynb files in this project, namely the model training algorithm based on noise prediction (Noise_prediction_training.ipynb), the model training algorithm based on residual prediction (Residual_prediction_training.ipynb), and the relay sampling algorithm (Relay_sampling.ipynb). Below are the pseudo-code diagrams of these three algorithms.

![输入图片说明](https://github.com/SuperChen100/RRDPM/blob/main/img/Algorithm1.png)

![输入图片说明](https://github.com/SuperChen100/RRDPM/blob/main/img/Algorithm2.png)

![输入图片说明](https://github.com/SuperChen100/RRDPM/blob/main/img/Algorithm3.png)

This project needs to be run in the paddlepaddle 3.0 environment.
