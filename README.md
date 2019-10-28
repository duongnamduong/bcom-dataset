# bcom-dataset
Our data set is a RGB-D images dataset captured from one indoor scene at IRT b-com (https://b-com.com). It is used for evaluating camera relocalization methods.
We use multiple fiducial markers attached on the scene to define the ground truth camera poses. 
This dataset consists of four small sequences (seq-01, seq-02, seq-03, seq-04) corresponding to absolutely different camera trajectories with the aim of evaluating generalization capability of camera relocalization methods.
To use this dataset, you can choose respectively each trajectory for training and then evaluate this model to estimate camera
pose for each frame of the other three trajectories.

# How to use
Each sequence consists of RGB images (xxxxx-color.png), their corresponding aligned depth images (xxxxx-depth.png) and ground truth camera poses.
For ground truth files, each line includes:

[path_to_image] tx ty tz w p q r

Where [tx ty tz] is camera's translation. [w p q r] is camera's quaternion.

Camera's intrinsic parameters are:
cx: 319.5
cy: 239.5
fx=fy: 469.15
depth is distance in millimeter
