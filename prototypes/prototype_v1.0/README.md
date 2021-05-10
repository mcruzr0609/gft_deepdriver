# Dataset
https://drive.google.com/file/d/14IdzPDxYQELlfCK48lPcuOWEX6Jm81Ej/view?usp=sharing

# Training
Notebook [train](https://github.com/mcruzr0609/gft_deepdriver/blob/master/prototypes/prototype_v1.0/train.ipynb)  
Before training, checking that the training set has a uniform distribution is very important to obtain good results.
![alt text](https://github.com/mcruzr0609/gft_deepdriver/blob/master/prototypes/prototype_v1.0/steer_distribution.png?raw=true)

The architecture of the neural network:
![alt text](https://github.com/mcruzr0609/gft_deepdriver/blob/master/prototypes/prototype_v1.0/nvidia.png?raw=true)

* Inputs
  * Image 200x66 (Segmentation)
  * Speed
* Outputs
  * Steer
  * Throttle
  * Brake
  * Speed 

# Agent
Notebook [carla-agent-cnn](https://github.com/mcruzr0609/gft_deepdriver/blob/master/prototypes/prototype_v1.0/carla-agent-cnn.ipynb)  
As a result the lateral control works but there are problems with the longitudinal control, a combination of a PID and network prediction is used.
