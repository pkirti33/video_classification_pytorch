# video_classification_pytorch
This repository features a Google Colab notebook where I explore multi-class video classification using the UCF11 video dataset. The dataset is available [here on Kaggle](https://www.kaggle.com/datasets/khanhvudo72/ucf11updated).

In this project, I built a mini 3D Convolutional Neural Network inspired by [Pytorch's 18-layer 3D Resnet Model](https://pytorch.org/vision/main/models/generated/torchvision.models.video.r3d_18.html) and trained it using two different methods:
1. **Custom Dimensions Transformation**: All videos were resized to 100x100 pixels. This approach achieved a 32% test accuracy over 10 epochs, taking approximately 1 hour.
2. **Inward Cropping Transformation**: Videos were cropped inward by 10% of their original length to focus on the most crucial parts. This method resulted in a 54% test accuracy over 10 epochs, taking about 1.4 hours.

## Next Steps
Future steps include experimenting with other transformations, tuning hyperparameters, and training over more epochs.

## Graphs
![Accuracy and Loss](https://github.com/pkirti33/video_classification_pytorch/blob/main/pictures/acc_loss_graphs.png)
![Time](https://github.com/pkirti33/video_classification_pytorch/blob/main/pictures/time_barchart.png)
