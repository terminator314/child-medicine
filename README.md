# child-medicine
基于儿童医学影像做图像识别、目标检测为医生提供诊断依据

---------------------------------------------------------------------------
## 基于PaddleDetection的医疗图像-病灶位置识别

 20231106 、尝试使用PP-yolov2检测痰液中的结合杆菌，从而实现异常检测。
## 一、项目背景
儿童影像主要是由X射线，分辨率较低，CT较高但数据较少。此项目主要预研目标检测病灶。

## 数据
数据说明
  该数据集全部与xx有关，取自xx样本。它包含yy个xx图像以及yy个细菌的边界框。XML文件包含图像的边界框详细信息。

## 算法

代码实现
python tools/train.py -c configs/yolov3/yolov3_mobilenet_v1_roadsign.yml

python tools/eval.py -c configs/yolov3/yolov3_mobilenet_v1_roadsign.yml -o weights=output/yolov3_mobilenet_v1_roadsign/model_final use_gpu=False

python tools/infer.py -c configs/yolov3/yolov3_mobilenet_v1_roadsign.yml -o weights=output/yolov3_mobilenet_v1_roadsign/model_final use_gpu=False


## 实现



## 结果



## 对比




## 【参考资料】



[Fracture Detection in Wrist X-ray Images Using Deep.pdf](https://github.com/terminator314/child-medicine/files/13454460/Fracture.Detection.in.Wrist.X-ray.Images.Using.Deep.pdf)

[Convolutional Neural Networks for Automated .pdf](https://github.com/terminator314/child-medicine/files/13454465/Convolutional.Neural.Networks.for.Automated.pdf)
[Deep learning assisted diagnosis system.pdf](https://github.com/terminator314/child-medicine/files/13454478/Deep.learning.assisted.diagnosis.system.pdf)


