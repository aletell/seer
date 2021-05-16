# seer
Synthetic Energy & Environment Replicator

### Description
Seer is a conditional GAN that creates synthetic building performance profiles. Synthetic projections of building performance profiles are conditioned based on climate and operation constraints. The model requires three sets of inputs for training, i.e. "performance", "operation", and "weather":
* The "performance" input should be a tensor of size [x,24,y], where x is the number of samples and y is the number of building perfromance features.
* The "operation" input should be a Boolean array of size [x,z]: where z corresponds to the length of the one-hot-encoded operation constraints.
* The "weather" input should have a size of [x,w], where w is the length of the weather constraints.

The data for training seer is obtained from "https://github.com/intelligent-environments-lab/CityLearn".

### Architecture

![GAN_arch](https://user-images.githubusercontent.com/27851066/118397689-8c76bf80-b655-11eb-9639-9ece5efc1ede.png)



## Requirements
Seer has been tested using the following Python libraries:
* Numpy 1.18.5
* Scipy 1.4.1
* TensorFlow 2.3.0

## Contact
Fazel Khayatian, Urban Energy Systems Laboratory, Empa.
https://www.empa.ch/web/khfa
