# child-medicine
基于儿童医学影像做图像识别、目标检测为医生提供诊断依据

---------------------------------------------------------------------------
## 基于PaddleDetection的医疗显微图像-结核杆菌识别

 20231106 、尝试使用PP-yolov2检测痰液中的结合杆菌，从而实现异常检测。


## 一、项目背景
儿童影像主要是由X射线，分辨率较低，CT较高但数据较少，但是CT辐射量较X射线要大，患者家属不易接受，目前主流还是X射线方式。此项目主要利用大量X射线获得的数据去训练一个模型，然后去在CT数据集上测试。

## 数据

GRAZPEDWRI-DX Dataset (Download Link)

```bash
GRAZPEDWRI-DX_dataset
    └── data   
         ├── images
         │    ├── train
         │    │    ├── train_img1.png
         │    │    └── ...
         │    ├── valid
         │    │    ├── valid_img1.png
         │    │    └── ...
         │    └── test
         │         ├── test_img1.png
         │         └── ...
         └── labels
              ├── train
              │    ├── train_annotation1.txt
              │    └── ...
              ├── valid
              │    ├── valid_annotation1.txt
              │    └── ...
              └── test
                   ├── test_annotation1.txt
                   └── ...

```

儿童医院手腕数据集child_data

```bash
positive_wristdata
         ├── 1.jpg
         │── 1.xml
         ├── 2.jpg
         │── 2.xml 
         ├── 3.jpg
         │── 3.xml  
         ├── 4.jpg
         │── 4.xml   
         ├── 5.jpg
         │── 5.xml       
 .....

```

数据说明
  该数据集全部与xx有关，取自xx样本。它包含yy个xx图像以及yy个细菌的边界框。XML文件包含图像的边界框详细信息。
- 数据切分
  dataset.csv 构成train_data.csv
  child.csv 构成valid_data.csv和 test_data.csv

## 算法
ppyolo+att

![image](https://github.com/user-attachments/assets/34d1dc4e-e064-49e9-b5d1-13168ba26396)

### 环境要求

- Linux (Ubuntu)
- Python = 3.7
- PaddlePaddle = 2.3.2
- NVIDIA GPU RTX3080 + CUDA CuDNN 10

## 实现


## 结果


## 对比

