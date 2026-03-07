
# Pretrained Networks

## Lesson Goal:

Students run predictions using MobileNet.

## Time Frame:

90'

## Key Concepts:

- imagenet competition
- VGG-16

## Warmup:

- do a recap quiz of concepts around CNN.

## Content Delivery:

- introduce the ImageNet competition
- discuss the structure of VGG-16
- run a prediction on 2-3 images using MobileNet
- discuss the mechanics (what shapes come out of the layers, the flattening especially)
- run the model with `include_top=False` and see 
- compare models in https://keras.io/api/applications/
- discuss why pretraining is a good idea

If you feel comfortable to go for a deeper dive, create variations of the images and see whether the model can deal with them, including:

- change brightness
- add blur
- insert black square
- remove one half
- shift the image
- rotate
- flip upside-down
- flip left-right
- blend two images together

Observer the resulting probabilities

TODO: Shreya ask Kristian to prepare a set of images for this.

## Material:

- notes: https://www.academis.eu/machine_learning/deep_learning/convolutional_neural_networks/pretrained.html
- notebook: https://github.com/krother/machine_learning/blob/main/solutions/neural_networks/PretrainedNetworks.ipynb

## Comments:

This is a rather easy lesson.

The VGG-16 is an inefficient model compared to others in the competition, but it explains the core idea best.

The ImageNet models are historically important, there has been a lot of gradual improvement since then. Discuss what modern pretrained models (like Google Images) do better/differently.

