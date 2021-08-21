# Object detection using detectron2 Faster-RCNN
![Project Image](https://github.com/Ghailen-Ben-Achour/detectron2_detection/blob/main/images/result_1.png)
![Project Image](https://github.com/Ghailen-Ben-Achour/detectron2_detection/blob/main/images/result_2.png)
---

## Description
This project aims to perform object detection using detectron2 Faster-RCNN on a custom datasetf (fruits nuts).

---

## Dataset
The dataset can be used as stored in ```data/images``` folder. Otherwise, you can follow the steps below to download and extract it.

- The COCO format of the dataset as well as its labels can be downloaded by running the command below.
```bash
wget https://github.com/Tony607/detectron2_instance_segmentation_demo/releases/download/V0.1/data.zip
```
- After that, go to the dataset directory and unzip it using:
```bash
unzip data.zip
```
---
#### Train & Evaluate
The model used in training is detectron's two implementation of ```faster RCNN```.

