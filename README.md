# DETR_VPA
The purpose of the project was to train DETR object detection model on a custom dataset VPA (Visual Privacy Advisor). The model was trained for almost 55 epoch on Google colab. I used the official facebook detr: End to end object detection with transformers (https://github.com/facebookresearch/detr) and fine-tunned my own model on vpa. Another repository that helped me tuning the detr on my custom dataset is https://github.com/woctezuma/finetune-detr#data.
# DATASET
You can download the dataset from https://tribhuvanesh.github.io/vpa/ if you want to retrain the model or use it for another use-case.In total, dataset contains 29 classes mostly related to text documnets.

      "face_all"
      "address_current_all", 
      "address_home_all", 
      "a108_license_plate_all", 
      "person_body", 
      "nudity_all", 
      "name_all", 
      "ethnic_clothing", 
      "birth_date", 
      "handwriting", 
      "ausweis", 
      "credit_card", 
      "passport", 
      "drivers_license", 
      "student_id", 
      "amail", 
      "receipt", 
      "ticket", 
      "disability_physical", 
      "medicine", 
      "phone", 
      "education_history", 
      "landmark", 
      "fingerprint", 
      "date_time", 
      "username", 
      "signature", 
      "email"
# Data Preperation
Inorder to train detr on vpa, I converted the vpa annotations into COCO format. The modify_vpa_coco.ipynb can be used for that purpose.
# Training
The model was fine-tunned using DETR R50 model. Others models can be downloaded from the catalogue of model zoo (https://github.com/facebookresearch/detr#model-zoo).
![alt text](https://github.com/EhsanAlahi/DETR_VISPR/blob/main/Use-cases/plot.png)
# Inferences
You can use the inferences.ipynb file to generate inferences on anyother images. Download the wights file from this drive link (https://drive.google.com/file/d/1-tcalfc-AjF1GezjqMvPLLGs4nr4R5p9/view?usp=sharing)
# Use-Cases
VPA dataset contain 29 different classes and our model was trained on all of them. Model perform differently for each class.Below are the results for different classes.
# Face, Body and Nudity
![alt text](https://github.com/EhsanAlahi/DETR_VISPR/blob/main/Use-cases/Face_Body.png)
![alt_text](https://github.com/EhsanAlahi/DETR_VISPR/blob/main/Use-cases/0.8.png)
![alt_text](https://github.com/EhsanAlahi/DETR_VISPR/blob/main/Use-cases/Face_Body_Nudity.png)
![alt_text](https://github.com/EhsanAlahi/DETR_VISPR/blob/main/Use-cases/download%20(21).png)
# Handwritten, Mail and Ticket
![alt_text](https://github.com/EhsanAlahi/DETR_VISPR/blob/main/Use-cases/Mail_Handwritten.png)
![alt_text](https://github.com/EhsanAlahi/DETR_VISPR/blob/main/Use-cases/ticket.png)
![alt_text](https://github.com/EhsanAlahi/DETR_VISPR/blob/main/Use-cases/ticket(2).png)
# Receipt
![alt_text](https://github.com/EhsanAlahi/DETR_VISPR/blob/main/Use-cases/receipt.png)
![alt_text](https://github.com/EhsanAlahi/DETR_VISPR/blob/main/Use-cases/receipt2.png)
# Passport
![alt_text](https://github.com/EhsanAlahi/DETR_VISPR/blob/main/Use-cases/Passport2.png)
![alt_text](https://github.com/EhsanAlahi/DETR_VISPR/blob/main/Use-cases/Passport.png)
# license plate number
![alt_text](https://github.com/EhsanAlahi/DETR_VISPR/blob/main/Use-cases/download%20(3).png)
# Redact Information
We can aslo it to redact information on student-id cards or other documents like Pictute, User-name, Date of birth or other information.
![alt_text](https://github.com/EhsanAlahi/DETR_VISPR/blob/main/Use-cases/redact.png)
![alt_text](https://github.com/EhsanAlahi/DETR_VISPR/blob/main/Use-cases/download%20(7).png)
# References 
Official DETR repository (https://github.com/facebookresearch/detr)
Fine-tunne DETR ( https://github.com/woctezuma/finetune-detr )
A Github issue regarding training detr on custom data (https://github.com/facebookresearch/detr/issues/9)
