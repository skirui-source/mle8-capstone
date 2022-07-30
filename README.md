### mle8-capstone
## American Sign Language (ASL) Classifier using Convolution Neural Networks (CNN)

# By: Sheilah K. (@skirui-source) 


* The Sign Language MNIST data sourced from Kaggle  ---- is a database of American Sign Language hand gestures that has been curated 
for multi-class classification using convolutional neural networks

* The data stored in .csv format represents 28x28 grayscale images as rows of labels 0-25 (first column) and pixel values 
1-784 (remaining columns). Total 24 labels represent 1:1 mapping for letters A-Z, excluding cases for 9=J and 25=Z which require hand 
gesture motion. 

* training and test data contain 27,455 and 7172 images respectively.  


"The original image data represented multiple users repeating the gesture against different backgrounds. The Sign Language MNIST data came from greatly extending the small number (1704) of the color images included as not cropped around the hand region of interest. To create new data, an image pipeline was used based on ImageMagick and included cropping to hands-only, gray-scaling, resizing, and then creating at least 50+ variations to enlarge the quantity. The modification and expansion strategy was filters ('Mitchell', 'Robidoux', 'Catrom', 'Spline', 'Hermite'), along with 5% random pixelation, +/- 15% brightness/contrast, and finally 3 degrees rotation. Because of the tiny size of the images, these modifications effectively alter the resolution and class separation in interesting, controllable way" (Kaggle)
