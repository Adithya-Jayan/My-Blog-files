# HANDWRITING RECOGNITION AND REPLICATION
## Team Members

* Chandan Kumar
* Sannuta

## Mentors

* Adithya Jayan
* A Shrikant
* Alabhya
* Anirudh Athresh
* Naman

## Objectives

This project aims at recognizing a handwritten text and replicating the same in a different handwriting. The work was then devided into three parts:
* Segmentation of the text into individual characters.
* Design and train a machine learning model to recognize the handwritten characters.
* Design a system to recreate the text in a different handwriting.

Each of the objectives were specifically handled by both of the team members.

## Methodology

### Segmentation of the text to letters


The handwritten text is captured by a camera and made available for digital processing. The image obtained is then processed to obtain a 
low-noise binary thresholded image of the same text. The program ensured that all the characters are correctly segmented even if some lines are tilted.

The algorithm used for segmentation is called a 'Projection  Profile'. The whole image is converted to a column vector by taking its sum of values
along each row. The resultant array is then plotted and using suitable thresholds, each line in the text is segmented out to give an array of images containing one line each.
The same pocedure along the columns of each image in the array, gave a final array of characters. This array of letters can then be passed to the machine learning model for further training.

### Designing and training of the Machine Learning Model

The segmented characters now, have to be classified into their classes of alphabets and digits. Identifying this classification problem, a deep learning model was 
proposed for efficient training and to get accurate results. A Convolutional Neural Network (CNN) model was designed and used as the model.

The dataset used for training the model is the [EMNIST](https://www.nist.gov/itl/products-and-services/emnist-dataset)
dataset of handwritten letters and digits. 

The CNN was trained on the dataset and the model was saved as a json file for further importing.

### Replacing each letter with a different handwriting

The set of letters for the second handwriting is read as a single image. The set is again segmented into a set of reference characters
using the same algorithm as above. The set is then labelled and stored. These can now be used to construct text in this handwriting.

The recognized labels of the handwritten letters are matched with the new letters and the letters are concatenated to from a new image
of the new handwriting.
 
 ## Results
 
 * The segmentaion using projection profle was carried out with a fairly high accuracy.
 * The CNN model presented a validation accuracy of about 88%.
 * The image with new handwriting was generated with few feeble errors and a fair accuracy.
 
 ### Application
 
 The project results can be used to discretize and recognize various aspects of recognition of handwritten text and proves to be of great work to study
 for further improvements to the project like a mechanical arm or a setup for copying the output onto a paper. The study in this field still remains quite interesting and open.

### Acknowledgements

We acknowledge and specially thank for the support and technical guidance given by our seniors Alabhya, Anirudh Athresh and Naman. We also thank IEEE-NITK for supporting
this project.

### References

Projection Profile - 
