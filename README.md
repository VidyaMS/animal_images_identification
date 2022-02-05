# animal_images_identification. 

Data source :   https://www.kaggle.com/alessiocorrado99/animals10. 

Images :  26179 for training , validation and testing.  
Classes : 10.  

Due to Kaggle memory restrictions during run time when images are not processed in batches, only 1000 train images , 300 validation images and 200 test images are used in this repo.  This limitation can be overcome by using tensorflow's methods of reading images from a directory.  

## Approach :  

### Build your own classifier using CNN + Max Pooling layers.  

Using tensorflow, sequential model consisting of layers of CNN and Max Pooling is created and its performance is checked using the data subset as mentioned above.Its seen that after building an 8 layer CNN + Max Pooling model , performance tuning by changing the optimizer as well as filters in CNN layer, neurons in the dense layer, the maximum accuracy obtained is 0.46.  This is a very poor performance.  

### Using pretrained weights and transfer learning.  

Using tensor keras application , various pretrained models such as VGG16, VGG19, MobileNet, ResNet50 are used to check the performance of transfer learning using  its own pretrained weights for the purpose of 10 class animal image classification. 

VGG16 and ResNet50 could give an accuraccy of 0.9 which is way too good as compared to model building approach.  
