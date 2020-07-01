# HANDWRITING RECOGNITION AND REPLICATION
## Team Members

* Chandan Kumar
* Sannuta

## Mentors

* Aditya Jayan
* A Shrikant
* Alabhya
* Anirudh Athresh
* Naman

## Objectives

This project aims at recognizing a handwritten text and replicating the same in a different handwriting. The work was then devided to
* Segmentation of the text into individual characters.
* Design and train a machine learning model to recognize the handwritten characters.
* Design a system to recreate the text in adifferent handwriting.

Each of the objectives were specifically handled by both of the team members.

## Methodology

### Segmentation of the text to letters

The handwritten text was to be captured by a camera and made available for processing it digitally. The image obtained was then processed to obtain a 
low-noise binary thresholded image of the same text. The program ensured that all the characters are correctly segmented even if some lines are tilted.

The algorithm used for segmentation was called a 'Projection  Profile'. The whole image was converted to a column vector by taking its sum of values
along each row. The resultant array was plotted and using suitable thresholds, each line in the text was segmented out to give an array of images copntaining each line.
The same pocedure aling the columns of each image in the array, gave a final array of characters. This array of letters were passed to the machine learning model for further training.

### Designing and training of the Machine Learning Model

The segmented characters now, have to be classified into their classed of alphabets and digits. Identifying this classification problem, a deep learning model was 
proposed for efficient traini9ng and to get accurate results. A Convolutional Neural Network (CNN) model was designed and was decided to use for the model.

The dataset for training the model was available as the [EMNIST](https://www.nist.gov/itl/products-and-services/emnist-dataset)
dataset of handwritten letters and digits. 

The CNN was trained on the dataset and the model was saved as a json file for further importing.

### Replacing each letter in a different handwriting

The set of letters for the seconfd handwriting was created as a single image. The set was again segmented into a set of reference characters
using the same algorithm as above. The set was then labelled and stored.

The recognized labels of the handwritten letters were matched with the new letters and the letters were concatenated to from a new image
 of new handwriting.
 
 ## Results
 
 * The segmentaion using projection profle was carried out with a fairly high accuracy.
 * The CNN model presented a validation accuracy of 
