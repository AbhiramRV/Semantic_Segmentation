# Semantic_Segmentation

This is a Semantic Segmentation information for self driving car.
Task of semantic segmentation is to classify each and every pixel present in an object to predefined classes/labels.
This infromation is needed for self driving for effective lane line detection, improving object detection, drivable space estimation, occupancy grid generation and multi object tracking problems.
Effectively for scene understanding.

Semantic segmentation models generally have encoder-decoder architecture.
Encoder consists Convolution layers with RELU activation functions and max pooling layers.
Decoder has unpooling layers with deconvolution layers.
During encoding stage, high level features are extracted which is similar to the initial layers of object detection networks. Size of images keeps reducing while features information increases.
Decoder learns to classify these features at pixel level and will upscale the image.



Some popular DNN architectures for semantic segmentation are  FCN, U-Net, Mask R_CNN,SegNet, PSPNet,DeepLav3+,E_net etc
Open data sets available for this task are CamVid,KITTI, CityScape etc
Classes present in the data set are Road,SideWalk,Building,Wall,Fence,Pole,TrafficLight, TrafficSign, vegetation, Terrain,sky, person,rider,car,truck, bus, train,motorcycle,bicycle,unlabeled etc.

Training a model on an available data set contains following steps
 - Data loading,Data visualization, Data Augmentation, Data resizing and Train-val-Test splits
 - Building and compiling model
 - Training the model
 - testing and performace evaluation
 - If satisfied with the model performance, save model as model.h5 

If dataset is not available readily for the required problem,
  -collect a small set of data
  -Augement the data
  -Use transfer learning on pretrained models.
  
tf.keras can be used to build and train the networks


Resources
Lyft self driving car semantic segmentation dataset in Kaggle.

