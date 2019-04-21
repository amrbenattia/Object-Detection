# Object Detection from Beer Dataset

This is an implementation of Mask RCNN on another dataset -Beer Dataset- using the code from https://github.com/matterport/Mask_RCNN
 
# Dataset
100 Beer Images collected from google to detect 3 objects - O (any circle or oval ), F letter and Star ★. 

the dataset is under dataset folder with subfolders train (90 images) and val (10 images)

# Training 
python3 './ofstar.py' train --dataset='./dataset/' --weights=coco   (to train using pretrained coco model)
or, 
python3 './ofstar.py' train --dataset='./dataset/' --weights=last   (to start train model form last saved model)

#saved model will be found in ./logs folder created while start training.

# Models pretrained on COCO and Beer Datasets 
you could downlaod from this link below and save to your present working directory.
https://drive.google.com/drive/folders/1hW0V-X3W083hcPlCodAcS4uyjskgAqh-?usp=sharing

# Data inspection and Model inference 
inspect_ofstar_data.ipynb notebook is provided for visulation of tthe dataset.
inspect_ofstar_model.ipynb to use the trained model to detect objects of validation dataset.

# Results 
using Mask R-CNN without Masks (Only Bounding Boxes), Results folder has a 3 samples.

![](Results/004927.jpg) 
![](Results/004435.jpg)



