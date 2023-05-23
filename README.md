## Data preparation

1. Upload dataset with labels into data folder

```shell
cd data
python3 train.py /path/to/dataset/train 
python3 val2yolo.py  /path/to/dataset/val 
```



## Training

```shell
CUDA_VISIBLE_DEVICES="0,1,2,3" python3 train.py --data data/dataset.yaml --cfg models/yolov5s.yaml --weights 'pretrained models'
```


#### Test

![](data/images/result.jpg)

#### Landmark Visulization 

![](data/images/landmark.png)
First row: RetinaFace, 2nd row: YOLOv5m-Face 
**YOLO5Face was used in the 3rd place standard face recogntion track of the [ICCV2021 Masked Face Recognition Challenge](https://www.face-benchmark.org/challenge.html).** 


#### AXera demo

https://github.com/AXERA-TECH/ax-samples/blob/main/examples/ax_yolov5s_face_steps.cc

#### Android demo

https://github.com/FeiGeChuanShu/ncnn_Android_face/tree/main/ncnn-android-yolov5_face

#### OpenCV DNN demo

https://github.com/hpc203/yolov5-face-landmarks-opencv-v2

#### ONNXRuntime/MNN/TNN/NCNN C++ demo

https://github.com/DefTruth/lite.ai.toolkit/blob/main/lite/ort/cv/yolo5face.cpp

https://github.com/DefTruth/lite.ai.toolkit/blob/main/lite/mnn/cv/mnn_yolo5face.cpp

https://github.com/DefTruth/lite.ai.toolkit/blob/main/lite/tnn/cv/tnn_yolo5face.cpp

https://github.com/DefTruth/lite.ai.toolkit/blob/main/lite/ncnn/cv/ncnn_yolo5face.cpp

#### References

https://github.com/ultralytics/yolov5

https://github.com/DayBreak-u/yolo-face-with-landmark

https://github.com/xialuxi/yolov5_face_landmark

https://github.com/biubug6/Pytorch_Retinaface

https://github.com/deepinsight/insightface


#### Citation 
- If you think this work is useful for you, please cite 

      @article{YOLO5Face,
      title = {YOLO5Face: Why Reinventing a Face Detector},
      author = {Delong Qi and Weijun Tan and Qi Yao and Jingfeng Liu},
      booktitle = {ArXiv preprint ArXiv:2105.12931},
      year = {2021}
      }

