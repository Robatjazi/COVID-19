# Predict COVIS-19 based on chest X-ray
The goal of this experiment is predicting COVID-19 based on an open image dataset, [COVID-19 open dataset](https://github.com/ieee8023/covid-chestxray-dataset#covid-19-image-data-collection) 

Actual pathology tests for COVID-19 is time consuming and has to be done in laboratories. Because of increasing daily cases throughout the world, it would be a problem to diagnose in proper time. 
Early diagnosis of COVID-19 helps to stop spreading it.


The [COVID-19 open dataset](https://github.com/ieee8023/covid-chestxray-dataset#covid-19-image-data-collection) has 56 COVID-19 case out of 119 cases.
I am going t use 56 case as positive samples and use [Chest X-Ray Images (Pneumonia)](https://www.kaggle.com/paultimothymooney/chest-xray-pneumonia) dataset (selecting healthy cases randomly to match the number of COVID-19 cases) for negative samples.


* I used some of the pretrained CNN networks like VGG16, VGG19, EfficientNet, ...
* I got good results using VGG16 and VGG19 network, you can find the results in vgg16network2.ipynb




