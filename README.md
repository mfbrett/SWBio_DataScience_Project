# README FILE
# Using CNN analysis for use in Species ID in Ecological Datasets

This is a script written in Google CoLab using neural network theory, to produce a file capable of differentiating between different species of flowers in the TensorFlow dataset ‘tf_flowers’. It is trained on 2,569 and tested on 1101 different images of flowers, of 5 classes: Sunflower, Rose, Daisy, Tulip and Dandelion.
Scaling this principle up to allow identification of multiple species of flower in the same image would be of great use in collecting ecological data, and could drastically reduce the time spent manually identifying plants during fieldwork. For example, by using a CNN script to analyse standardized quadrat photos in a wildflower meadow.

**To run:**

1.	Go to the script 'CNN_Flowers_SwBio.ipynb' in this repository, and open using Google Colab. Alternatively, download the file and then upload to Google Colab Manually: https://colab.research.google.com/

2.	The code for accessing and downloading the training and test dataset is provided in the script, however if you wish to also download it to your computer, it is available from this link: https://www.tensorflow.org/datasets/catalog/tf_flowers

3.	Run through the script to load the data, resize and prepare the images for use in training and testing the model. For a faster run time, you can reduce the size of the images by reducing the ‘IMAGE_RES =’ value.

4.	The unmodified model runs using 5 epochs. To improve the model accuracy, increase the number of epochs. NB this will also increase the run time.

5.	The last part of the script produces a graph that shows how well the model has improved accuracy over time, and a sample of images with identifications predicted by the model.

**Possible improvements:** The provided model in this script is able to identify flowers in images to around 63% accuracy. This could be improved by increasing the number of epochs run, and by removing erroneous images in the dataset which do not contain flowers.
