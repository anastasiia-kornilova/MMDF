# MMDF: Mobile Microscopy Deep Framework
The aim of our project is to apply deep learning techniques in the field of optical imaging to images taken from mobile microscope. We consider data that consists of z-stack images of specimen (more details in dataset description). In this work we would like to use the next techniques:

- In-focus/out-of-focus images classification. When automatically scanning specimen, it is necessary to choose only in-focus images. In comparison to classical focus measure operators DL techniques allow not to lose small focused parts of the image.
- Fast scanning image deblurring. Obtaining of the high quality images requires much more time while scanning. The idea is to reuse DL deblurring techniques for fast scanning when we can reconstruct original image from one obtained from fast movement.
- Focus-stacking (Multi-Focus fusion). Because of the main feature of optical microscopes is shallow depth of focus, therefore volume specimen can not be studied from one focal length -- user should change it mechanically to understand the structure of sample. The idea is to apply all-in-focus technique to construct the image where all the parts are sharp.

![2018, Pfeil et al
“Mobile Microscopy and Automated Image Analysis”
](https://github.com/anastasiia-kornilova/MMDF/blob/master/pics/mobile_microscopy.PNG)

The code was written by:

- Egor Sevriugov and Kirill Shcherbakov -  
- Maria Begicheva and Olga Novitskaya - 
- Mikhail Salnikov and Anastasiia Kornilova - 

**AEbyForest: [Project](https://github.com/Olga013/Skoltech-ML-2020-AutoEncoder-by-Forest) | [Paper](https://arxiv.org/pdf/1709.09018.pdf) | [Report](https://github.com/Olga013/Skoltech-ML-2020-AutoEncoder-by-Forest/blob/master/AutoEncoder_by_Forest.pdf) | [Presentation](https://github.com/Olga013/Skoltech-ML-2020-AutoEncoder-by-Forest/blob/master/presentation/Presentation_AutoEncoder_by_Forest.pdf) | [Video](https://www.dropbox.com/s/v0iiwld87gk658y/zoom_0.mp4?dl=0)**

Train MNIST/Test MNIST
![](https://github.com/Olga013/Skoltech-ML-2020-AutoEncoder-by-Forest/blob/master/images/Merged_MNIST.png)

Train CIFAR10/Test CIFAR10
![](https://github.com/Olga013/Skoltech-ML-2020-AutoEncoder-by-Forest/blob/master/images/Merged_CIFAR10.png)


## Colab Notebook
- Tree ensemble based AE (MNIST, CIFAR-10, Omniglot): [Google Colab](https://colab.research.google.com/github/Olga013/Skoltech-ML-2020-AutoEncoder-by-Forest/blob/master/eForest_models/eForest_ml%20.ipynb) | [Code](https://github.com/Olga013/Skoltech-ML-2020-AutoEncoder-by-Forest/tree/master/eForest_models)
- CNN based AE (MNIST, CIFAR-10, Omniglot): [Google Colab](https://colab.research.google.com/github/Olga013/Skoltech-ML-2020-AutoEncoder-by-Forest/blob/master/CNN_models/CNNs_models.ipynb) | [Code](https://github.com/Olga013/Skoltech-ML-2020-AutoEncoder-by-Forest/tree/master/CNN_models)
- MLP based AE (MNIST, Omniglot): [Google Colab](https://colab.research.google.com/github/Olga013/Skoltech-ML-2020-AutoEncoder-by-Forest/blob/master/MLP_models/MLP_MNIST.ipynb) | [Code](https://github.com/Olga013/Skoltech-ML-2020-AutoEncoder-by-Forest/blob/master/MLP_models/MLP_MNIST.ipynb)
- MLP based AE (CIFAR-10, Omniglot): [Google Colab](https://colab.research.google.com/github/Olga013/Skoltech-ML-2020-AutoEncoder-by-Forest/blob/master/MLP_models/MLP_CIFAR_10.ipynb) | [Code](https://github.com/Olga013/Skoltech-ML-2020-AutoEncoder-by-Forest/blob/master/MLP_models/MLP_CIFAR_10.ipynb)

## Prerequisites
- Python 3
- Google Colaboratory service
- PyTorch 1.4.0, Tensorflow 2.1.0, Keras 2.3.0

## Datasets info
The dataset contains the videos of z-stack scanning recorded by a smartphone microscope (150 specimen). Every scan is presented in 4 videos with different speed of scanning.


## Related Projects

- The official implementation for the paper "AutoEncoder by Forest" by Ji Feng and Zhi-Hua Zhou 2017:  [Paper](https://arxiv.org/pdf/1709.09018.pdf) | [Code](https://github.com/kingfengji/eForest)
- Non-official implementation of the paper "AutoEncoder by Forest" by Ji Feng and Zhi-Hua Zhou 2017 by Antoine Passemiers:  [Paper](https://arxiv.org/pdf/1709.09018.pdf) | [Code](https://github.com/AntoinePassemiers/Encoder-Forest)
