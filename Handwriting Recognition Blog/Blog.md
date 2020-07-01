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
low-noise binary thresholded image of the same text. The program ensured that all the lines of the text to be aligned horizontally even if some lines are tilted.

The algorithm used for segmentation was called a 'Projection  Profile'. The whole image was converted to a column vector by taking its sum of values
along each row. The resultant array was plotted and using suitable thresholds, each line in the text was segmented out to give an array of images copntaining each line.
The same pocedure aling the columns of each image in the array, gave a final array of characters. This array of letters were passed to the machine learning model for further training.

### Designing and training of the MAchine Learning Model

The segmented characters now, have to be classified into their classed of alphabets and digits. Identifying this classification problem, a deep learning model was 
proposed for efficient traini9ng and to get accurate results. A Convolutional Neural Network (CNN) model was designed and was decided to use for the model.

The dataset for training the model was available as the [EMNIST](https://www.nist.gov/itl/products-and-services/emnist-dataset)
dataset of handwritten letters and digits. 
