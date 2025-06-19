# Vehicle Registration Plate Object Detection

### Project Summary:
This project creates a machine learning model to operate an object detection task on vehicle registration plates, using PyTorch.

---

### Dataset Description:

This dataset consists of `5308` training and `386` validation dataset. Each dataset has images in `.jpg` format and labels in `.txt` format with the `xmin, ymin, xmax, ymax` format. Below are sample images from some of the classes present in the dataset:

![](./visuals/reg_plate_dataset1.png?raw=true)
![](./visuals/reg_plate_dataset2.png?raw=true)
![](./visuals/reg_plate_dataset3.png?raw=true)

---

### Machine Learning Model Architecture:

I used pretrained model `yolov9c.pt` with the pretrained weight and and trained it to be able to detect the vehicle registration plates. 

---

### Training Hyperparameters:

* Epochs: `30`
  
* In put Image size: `640`

---

### COCO Detection Evaluation:

```
map  0.6881700304920099
map50  0.9184385705155789
map75  0.8086742052315866
maps50-95  [    0.68817]
```

---

### Inference on Images:

![](./visuals/reg_plate_inference1.png?raw=true)
![](./visuals/reg_plate_inference2.png?raw=true)
![](./visuals/reg_plate_inference3.png?raw=true)

---


### Inference on Video:

https://youtu.be/GcFTGHmGbmU
