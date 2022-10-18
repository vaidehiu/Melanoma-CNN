# Melanoma Skin Cancer Detection - CNN 
> There are many types of cancers focused on skin/derma in layman tongue upper layer of body. Some are benign some malignanant out of which Melanoma is most fatal malignant cancer type as it accounts for 75% of skin cancer death .


Why Melanoma is fatal ?
> Melanoma is needed to be detected at very early stage beacuse of manual process of doctor who check the scan and say if its melanoma or not which again induces human errors also it delays the treatment because of manual process involved. Patients miss the "GOLDEN" time and lose their life.
> This can fixed if and only if there was way to automate this process of detection and make the pipeline from doctor to patient easily.
> This project aims at detecting types of skin cancer given the dataset .To aid in better indentification if melanoma or any other cancer easily 

###### NOTE : Make a directory called CNN inside Mydrive .Add CNN_assignment.zip given in module inside this CNN folder.  As in multiple places the path defined is /content/gdrive/MyDrive/CNN/ . Also use colab to run as it takes more than 40 mins if run normally also this notebook is compatible only with colab if path folder not changed.
## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)

<!-- You can include any other section that is pertinent to your problem -->

## General Information
* Data Reading/Data Understanding → Defining the path for train and test images
* Dataset Creation→ Create train & validation dataset from the train directory with a batch size of 32. Also, make sure you resize your images to 180*180.
* Dataset visualisation → Create a code to visualize one instance of all the nine classes present in the dataset
* Model Building & training : Create a CNN model, which can accurately detect 9 classes present in the dataset. While building the model rescale images to normalize pixel values between (0,1).
* Choose an appropriate optimiser and loss function for model training
* Train the model for ~20 epochs
* model overfit or underfit?
* Choose an appropriate data augmentation strategy to resolve underfitting/overfitting Model Building & training on the augmented data :
* Create a CNN model, which can accurately detect 9 classes present in the dataset. While building the model rescale images to normalize pixel values between (0,1).
* Choose an appropriate optimiser and loss function for model training
* Train the model for ~20 epochs
* earlier issue is resolved or not?
* Examine the current class distribution in the training dataset
* Which class has the least number of samples?
* Which classes dominate the data in terms of the proportionate number of samples? Handling class imbalances:
* Rectify class imbalances present in the training dataset with Augmentor library. Model Building & training on the rectified class imbalance data:
* Create a CNN model, which can accurately detect 9 classes present in the dataset. While building the model rescale images to normalize pixel values between (0,1).
* Choose an appropriate optimiser and loss function for model training
* Train the model for ~30 epochs



<!-- You don't have to answer all the questions - just the ones relevant to your project. -->

## Conclusions
- This project has 3 models to investigate and get better model for prediction.
- Model 1 : Simple CNN model+scalling  without dropouts - Extreme overfitting
<img src="https://github.com/vaidehiu/Melanoma-CNN/blob/main/train.PNG" alt="drawing" style="width:150px;"/>

- Model 2: CNN +data augmentation layer+dropout .Overfitting reduced . But accuracy was very low even at 20 epochs it was 50% approx .Underfitted model 
<img src="https://github.com/vaidehiu/Melanoma-CNN/blob/main/train1.PNG" alt="drawing" style="width:150px;"/>

- Model 3 : Used Augmentor added 500 more augmented images and trained for 50 epoches. There is steady increasing in both validation accuracy and train accuracy with not much variations in both which is ideal case for model.
<img src="https://github.com/vaidehiu/Melanoma-CNN/blob/main/train2.PNG" alt="drawing" style="width:150px;"/>
<!-- You don't have to answer all the questions - just the ones relevant to your project. -->


## Technologies Used
* tensorflow- 2.9.2
* seaborn- 0.11.2
* Pillow - 7.1.2
* pathlib - 1.0.1
* pandas - 1.3.5
* numpy - 1.21.6
* matplotlib - 3.2.2
* keras - 2.9.0
* google - 2.0.3
* Augmentor - 0.2.10

<!-- As the libraries versions keep on changing, it is recommended to mention the version of library used in this project -->

## Acknowledgements
This project was created as a assignment required for Executive PG Programme in Machine Learning & AI - IIIT, Bangalore


## Contact
Reach out the creators on,
- Linkedin:
    - [Vaidehi Rao](https://www.linkedin.com/in/vaidehi-u-026a09150/)
- Github:
    - [Vaidehi Rao](https://github.com/vaidehiu)  
