# mle8-capstone
## American Sign Language (ASL) Classifier using Convolution Neural Networks (CNN)

### By: Sheilah K. (@skirui-source) 

### Metadata
* The Sign Language MNIST data sourced from Kaggle posted by unknown author with username "tecperson" ---- 
URL : https://www.kaggle.com/datamunge/sign-language-mnist

* The data stored in .csv format represents American Sign Language hand gestures; 28x28 grayscale images as rows of labels 0-25 (first column) and pixel values 1-784 (remaining columns).

* Total 24 labels represent 1:1 mapping for letters A-Z, excluding cases for 9=J and 25=Z which require hand 
gesture motion. 

* training and test data contain 27,455 and 7172 images respectively.  


### Data Lineage 

* Original: color images of multiple users repeating the gesture against different backgrounds. 

* To create new data, an image pipeline was used based on ImageMagick: 
    - cropping to hands-only
    - gray-scaling, resizing, 
    - creating at least 50+ variations to enlarge the quantity. 
    - modification and expansion strategy: filters ('Mitchell', 'Robidoux', 'Catrom', 'Spline', 'Hermite')
    - 5% random pixelation
    - +/- 15% brightness/contrast
    - 3 degrees rotation
