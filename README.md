# Object-Detection

This is an implementation of Mask RCNN on another dataset -Beer Dataset- using the code from https://github.com/matterport/Mask_RCNN
 
# Dataset
100 Beer Images collected from google to detect 3 objects - O (any circle or oval ), F letter and Star ★. 

the dataset is under dataset folder with subfolders train (90 images) and val (10 images)

# Training 
python3 './ofstar.py' train --dataset='./dataset/' --weights=coco   (to train using pretrained coco model)
or, 
python3 './ofstar.py' train --dataset='./dataset/' --weights=last   (to start train model form last saved model)

#saved model will be found in ./logs folder created while start training.

# 
