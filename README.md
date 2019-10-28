# bcom-dataset
Our data set is a RGB-D images dataset captured from one indoor scene at IRT b-com (https://b-com.com). It is used for evaluating camera relocalization methods.
We use multiple fiducial markers attached on the scene to define the ground truth camera poses. 
This dataset consists of four small sequences corresponding to absolutely different camera trajectories with the aim of evaluating generalization capability of camera relocalization methods.
To use this dataset, you can choose respectively each trajectory for training and then evaluate this model to estimate camera
pose for each frame of the other three trajectories.
