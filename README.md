## Configure .yaml file 
Put path to input/output folders. Input folder contains dataset with labels,path to pretrained models, weights

```shell
input_dir = "/home/yeldar/Documents/yolov5-face/config/"
output_dir = "/home/yeldar/Documents/yolov5-face/output/"
```
<!-- 
country = 'kg'
doc_version = '1'
doc_side = 'front' -->

batch_size = 0

output_shape_h_min = 300
output_shape_h_max = 822
output_shape_h_coef = 1.5


## Data preparation

1. Upload dataset with labels into data folder

## Training

```shell
cd data
python3 train.py /path/to/dataset/train 
python3 val2yolo.py  /path/to/dataset/val 
```

```shell
CUDA_VISIBLE_DEVICES="0,1,2,3" python3 train.py --data data/dataset.yaml --cfg models/yolov5s.yaml --weights 'pretrained models'
```
