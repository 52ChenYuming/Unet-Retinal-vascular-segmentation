
## 环境配置：
* Python 3.8.19
* Pytorch 1.13.1
* CUDA 11.7
* GPU 3050Ti 4GB显存

## 文件结构：
```
  ├── src: 搭建U-Net模型代码
  ├── train_utils: 训练、验证以及多GPU训练相关模块
  ├── my_dataset.py: 自定义dataset用于读取DRIVE数据集(视网膜血管分割)
  ├── train.py: 训练脚本
  ├── predict.py: 预测脚本(需要先进行训练获得权重)
  └── compute_mean_std.py: 统计数据集各通道的均值和标准差
```

## DRIVE数据集下载地址：
* 官网地址： [https://drive.grand-challenge.org/](https://drive.grand-challenge.org/)


## 训练方法
* 运行train.py

## 预测方法
* 运行predict.py

## 本项目U-Net使用双线性插值做为上采样
