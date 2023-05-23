## Configure .yaml file 

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
