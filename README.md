# Explore Different ConvNets Models

After learning Convolution Neural Network in the class, we think that maybe we could use CNNs with different models to work. That is the initial motivation of our project. In our project, we recreated four small ConvNets via reading some published papers. Then We calculated the error rate of validation to judge the models' performance and came out with the idea of **ensemble them together to reduce the error rate**. Our word comments are the Markdown in jupyter notebook.

<p align="center">
<img src="/Image/Instruction.png">
</p>


### Dataset

Each network (model) will be trained base on CIFAR-10 dataset.The CIFAR-10 dataset consists of 60000 32x32 colour images in 10 classes, with 6000 images per class. There are 50000 training images and 10000 test images.  

<p align="center">
<img src="/Image/CIFAR10.png">
</p>

### Results

<p align="center">
<img src="/Image/Results.png">
</p>

| Model  | Evaluate Error Rate <br> (20 epochs)  |
|---|---|
| Strided-CNN-C<!-- .element: style="text-align:center;" --> | 25.63%<!-- .element: style="text-align:center;" --> |
| ConvPool-CNN-C<!-- .element: style="text-align:center;" --> | 22.07%<!-- .element: style="text-align:center;" --> |
| ALL-CNN-C<!-- .element: style="text-align:center;" -->  | 26.08%<!-- .element: style="text-align:center;" --> |
| Network In Network CNN<!-- .element: style="text-align:center;" -->  |  35.43%<!-- .element: style="text-align:center;" --> |
| Ensemble<!-- .element: style="text-align:center;" --> | 19.15%<!-- .element: style="text-align:center;" --> |

### Requisites

- Anaconda Python 3.0
- Keras
- TensoFlow
- GPU for fast training


### References

- [Striving for Simplicity: The All Convolutional Net](https://arxiv.org/pdf/1412.6806)
- [Understanding and Improving Convolutional Neural Networks via Concatenated Rectified Linear Units](https://arxiv.org/pdf/1603.05201)
- [Network In Network](https://arxiv.org/abs/1312.4400)
