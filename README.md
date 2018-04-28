# Semantic Segmentation

## Project Objectives
In this project, we label the pixels of a road in images using a Fully Convolutional Network (FCN).
The data set used for the model training is the [Kitti Road dataset](http://www.cvlibs.net/datasets/kitti/eval_road.php) accessible from [here](http://www.cvlibs.net/download.php?file=data_road.zip).

## Project Files

* Source code: [main.py](https://github.com/schambon77/CarND-Semantic-Segmentation/blob/master/main.py)
* [Read me](https://github.com/schambon77/CarND-Semantic-Segmentation/blob/master/README.md)

## Project Rubric Points

Project rubric points can be found [here](https://review.udacity.com/#!/rubrics/989/view)

### Build the Neural Network

The project loads the pretrained vgg model through the function `load_vgg`.

The project learns the correct features from the images through the function `layers`.

The project optimizes the neural network through the function `optimize`.

The project trains the neural network through the function `train_nn`.

![Loss printout][image1]
Printout of the loss value during training


### Neural Network Training

The project trains the model correctly. On average, the model decreases loss over time.

| Epoch 0            | Epoch 10      | Epoch 20  |  Epoch 30  | Epoch 39 |
| :------------------ |:-------------:| :---------:|:-----------:|:---------:|
| ![Epoch 0][image2] | ![Epoch 10][image3] | ![Epoch 20][image4] | ![Epoch 30][image5] | ![Epoch 39][image6] | 


The project uses reasonable hyperparameters
* epochs: 40
* batch size: 12
* learning rate: 1e-3

The project correctly labels the road.

![Test image][image7]

![Test image][image8]

![Test image][image9]

![Test image][image10]


[//]: # (Image References)

[image1]: ./loss_printout.jpg "Loss printout"
[image2]: ./epoch0.jpg "Epoch 0"
[image3]: ./epoch10.jpg "Epoch 10"
[image4]: ./epoch20.jpg "Epoch 20"
[image5]: ./epoch30.jpg "Epoch 30"
[image6]: ./epoch39.jpg "Epoch 39"
[image7]: ./runs/1524709708.7446492/um_000023.png "Test image"
[image8]: ./runs/1524709708.7446492/um_000082.png "Test image"
[image9]: ./runs/1524709708.7446492/umm_000041.png "Test image"
[image10]: ./runs/1524709708.7446492/uu_000091.png "Test image"

