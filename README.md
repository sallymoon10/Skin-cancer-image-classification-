# Detect skin cancer based on dermatoscopic images of skin lesions 

### Highlights:
- Fine-tuned pre-trained image recognition model to classify dermatoscopic images and predict the presence of skin cancer 
- Achieved upto 0.81 AUC with DenseNet model fine-tuned to cancer classification task
- Tech: Python (Pytorch, Scipy, Numpy, Pandas, matplotlib)
- Work completed: Data processing (addressing class imbalance, data augmentation, normalization, custom Pytorch Datasets), model development (DenseNet, ResNet, VGG), and model iteration (train and validation pipeline)

![Alt text](/assets/results.png?raw=true=50x50  "AUC results on test dataset")


### Transfer learning image recognition model:
- Several deep convolutional models (eg. ResNet, DenseNet, Inception, etc) have been pre-trained on large corpuses of images and have been shown to have great performance on various image recognition tasks
- We can use transfer learning to use these top-performing pre-trained models to achieve good classification performance on other tasks, such as skin cancer recognition
- Transfer learning is process where a model trained on one problem is used in someway on another related problem. More specifically, the the weights of a pretrained model can be directly re-used or fine-tuned to work for another task. With this, we can obtain good performance with smaller datasets. 

### Dataset:
- Tschandl, P., Rosendahl, C. & Kittler, H. The HAM10000 dataset, a large collection of multi-source dermatoscopic images of common pigmented skin lesions. Sci. Data 5, 180161 doi:10.1038/sdata.2018.161 (2018).
- https://www.kaggle.com/kmader/skin-cancer-mnist-ham10000

### References:
- This notebook was inspired by the following resources:

- https://www.kaggle.com/xinruizhuang/skin-lesion-classification-acc-90-pytorch

- https://www.kaggle.com/kmader/dermatology-mnist-loading-and-processing
