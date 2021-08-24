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
## Train & Evaluate
The model used in training is detectron's two implementation of ```faster RCNN```. Since we are only interested in object detection, we extract only the bounding box labels for each object (pixel wise annotation is not used).

To train a model you can run ```fruits_detection.ipynb```.

You can change the hyperparameters used in this project.
```bash
cfg.SOLVER.IMS_PER_BATCH = 2
cfg.SOLVER.BASE_LR = 0.00025 
cfg.SOLVER.MAX_ITER = 300 
cfg.TEST.EVAL_PERIOD = 100
cfg.MODEL.ROI_HEADS.BATCH_SIZE_PER_IMAGE = 4
```
---
## Results

Results are stored inside ```output``` folder.

