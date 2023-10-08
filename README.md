# CRNN文本识别

论文： 
[An End-to-End Trainable Neural Network for Image-based Sequence Recognition and Its Application to Scene Text Recognition](http://arxiv.org/abs/1507.05717)

## 数据集

数据集使用[trdg](https://github.com/Belval/TextRecognitionDataGenerator)生成。

分别生成训练集和测试集，并将其放在两个不同的文件夹即可。

## 效果

| Five Words with Noise   | Single Word with Noise (trained with same Size 100x32) | Three Words with Background |
| ----------------------- | ------------------------------------------------------ | --------------------------- |
| ![](./img/5-words.png)  | ![](./img/1-word.png)                                  | ![](./img/3-words.png)      |
| Test Accuracy: 92.5%    | Test Accuracy: 93.5%                                   | Test Accuracy: 40.4%        |
| batch_size=16, epoch=30 | batch_size=32, epoch=30                                | batch_size=16, epoch=30     |

## 说明

`crnn_str_simple.ipynb`是一个简单的CRNN实现，可用于**一个单词**的数据集，并有着良好的效果。

`crnn_str.ipynb`可以用于识别不同长度的文本图像，也可修改参数来选择单通道（灰度图片）还是三通道（RGB彩色图像）训练和测试。

## 参考

[https://github.com/bgshih/crnn](https://github.com/meijieru/crnn.pytorch
)

[https://github.com/meijieru/crnn.pytorch](https://github.com/meijieru/crnn.pytorch
)
