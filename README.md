# DETR_VPA
The purpose of the project was to train DETR object detection model on a custom dataset VPA (Visual Privacy Advisor). The model was trained for almost 55 epoch on Google colab. I used the official facebook detr: End to end object detection with transformers https://github.com/facebookresearch/detr) and fine-tuned my own model on vpa. Another repository that helped me tuning the detr on my custom dataset is https://github.com/woctezuma/finetune-detr#data.
# DATA
You can download the dataset from https://tribhuvanesh.github.io/vpa/ if you want to retrain the model or use it for another use-case.
# Data Preperation
Inorder to train detr on vpa, I converted the vpa annotations into COCO format. The modify_vpa_coco.ipynb can be used for that purpose.
# Training
The model was fine-tunned using DETR R50 model. Others models can be downloaded from the catalogue of model zoo (https://github.com/facebookresearch/detr#model-zoo).
https://github.com/EhsanAlahi/DETR_VISPR/blob/main/Use-cases/plot.png
