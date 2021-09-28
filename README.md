# Cleaning_Grimy_Docs

From E-books to online government records, the need for digitizing is exponentially
increasing. However, some documents cannot be digitized easily as they may
contain some strains, heavy foldings, etc. We used Autoencoders and conventional
image enhancement techniques to clean the grimy documents and make them easy
for digitization. Also, we stacked all our models (methods) by using CNN
stacker to generate a better document than any individual model, with the aid of
thinking about all models.

<br>

### Dataset - [Link](https://www.kaggle.com/c/denoising-dirty-documents/overview)

<br>

## Models 

### Traditional Image processing Techniques

1. Adaptive Thresholding
2. Median Filter

### Neural Networks

1. Convolutional Autoencoders
    
    Architecture :
    ![Autoencoder Architecture](https://github.com/OVSRIKANTH/Cleaning_Grimy_Docs/blob/main/Images/autoencoder.png)

2. Stacked CNN 
    
    Architecture :
    ![Stacked CNN Architecture](https://github.com/OVSRIKANTH/Cleaning_Grimy_Docs/blob/main/Images/stackedcnn.png)


All details about models and their hyperparameters are mentioned in [report](Report.pdf).


## Results 

| Model        | RMSE           |
| ------------- |:-------------:| 
| Raw Data     | 0.14974 | 
| Adaptive Thresholding     | 0.07516      |   
| Median Filter | 0.05197      |   
| Convolutional Autoencoder | 0.02319 |
| CNN Stacker | **0.01948** |


