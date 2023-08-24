# Brain-Tumor-Classification

During brain tumor diagnosis, different segments or sections of the brain are scanned by an MRI 
machine. One reason could be to obtain multiple scans to help medical experts arrive at an accurate 
diagnosis such as the type, position, size of the brain tumor etc. As a result, MRI machines usually scans 
for a prolonged period, capturing different areas of the brain. For an increased scan quality, MRI 
machines with higher magnetic index are used during brain scans and these machines are quite 
expensive to run.
To obtain multiple brain scans, patients are also required to remain still in the MRI machine for long 
periods pending when scans are completed. This makes the process discomforting to patients.

## Objectives
The main aim of this project to propose a deep learning algorithm that can effectively identify and 
classify MRI scans to determine the presence or absence of brain tumour and compare the performance 
of proposed algorithm with other methods. The objectives are further defined as follows:
- To evaluate and analyze the effectiveness of transfer learning technique using pre-trained VGG16 model in classifying brain MRI scans to determine the presence or absence of tumour.
- To compare the performance of CNN with pre-trained VGG-16 model with basic CNN network 
and machine learning algorithm like support vector classifier (SVC)
- Further validate proposed model performance by testing on a new dataset from Kaggle 
https://www.kaggle.com/datasets/abhranta/brain-tumor-detection-mri.

To obtain the best CNN model, data augmentation and hyperparameter tuning will also be implemented 
and evaluated for effectiveness.

## Data Soure:
The image dataset used for this work can be found via Kaggle –
https://www.kaggle.com/datasets/preetviradiya/brian-tumor-dataset. It contains 4,600 MRI scans 
(brain tumour – 2513 & healthy – 2087). To aid training and evaluation, the dataset will be splitted 
into training and testing dataset.

## Jupyter notebook file for Pyrhon codes used:
https://github.com/giftomoba/Brain-Tumor-Classification/blob/main/Final%20Ai%20code%20-%20main-Copy1.ipynb

## Best Performing Model:
The CNN model enhanced with pre-trained VGG-16 model performed best with training and validation accuracies of 100% and 99% respectively.
The model performance analysis is given below:

![vgg 1](https://github.com/giftomoba/Brain-Tumor-Classification/assets/124467481/a1ad7a8e-f634-452d-9c99-8652c71cb312) ![vgg 2](https://github.com/giftomoba/Brain-Tumor-Classification/assets/124467481/0e394e99-0829-4e45-8a5a-cb0606328810)

![vgg Tr](https://github.com/giftomoba/Brain-Tumor-Classification/assets/124467481/499625f7-4728-451f-a95f-1a24c54be588)

-
![vgg Te](https://github.com/giftomoba/Brain-Tumor-Classification/assets/124467481/0446c496-b808-44d5-9210-c732ac612bdc)

-
![vgg conf](https://github.com/giftomoba/Brain-Tumor-Classification/assets/124467481/189f8e69-5806-4ac2-948a-34b002611140)

-
## Applying model to predict a new 'Unseen' data:
![new](https://github.com/giftomoba/Brain-Tumor-Classification/assets/124467481/067e0abf-bcf7-4a4a-a91a-8954e1d02f4f)

## Conclusion:
In this project, both deep learning (CNN) and machine learning (SVC) algorithms were implemented 
and evaluated for determining the presence or absence of tumours in MRI scans. Different 
experiments were implemented with the CNN architecture to find optimal performance. Pre-trained
weights from VGG-16 model was used to finetune the CNN while hyperparameter tuning was also 
done. The CNN enhanced with VGG-16 performed best with training and validation accuracies of 
100% and 99%, outperforming the baseline models. Although SVC had training accuracy of 97%, for 
future work, I would recommend implementing GridSearchCV to select best hyperparameter to 
optimize the results.


