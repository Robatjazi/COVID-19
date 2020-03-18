# Predict COVIS-19 based on chest X-ray
The goal of this experiment is predicting COVID-19 based on an open image dataset, [COVID-19 open dataset](https://github.com/ieee8023/covid-chestxray-dataset#covid-19-image-data-collection) 

Actual pathology tests for COVID-19 is time consuming and has to be done in laboratories. Because of increasing daily cases throughout the world, it would be a problem to diagnose in proper time. 
Early diagnosis of COVID-19 helps to stop spreading it.


The [COVID-19 open dataset](https://github.com/ieee8023/covid-chestxray-dataset#covid-19-image-data-collection) has 56 COVID-19 cases out of 119 cases.
I am going to use 56 case as positive samples and use [Chest X-Ray Images (Pneumonia)](https://www.kaggle.com/paultimothymooney/chest-xray-pneumonia) dataset (selecting healthy cases randomly to match the number of COVID-19 cases) for negative samples.

* I used some of the pretrained CNN networks like VGG16, VGG19, EfficientNet, ...
* I got good results using VGG16 and VGG19 network, you can find the results in vgg16network2.ipynb


### Sample COVID-19 and healty cases
![Result](https://github.com/Robatjazi/COVID-19/blob/master/covid-19_3.png)

### Following is the results of the experiment:


#### Classification Rreport

|               | precision     |  recall     |   f1-score    |   support     |
| ------------- | ------------- | ----------- | ------------- | ------------- | 
| covid         | 0.92          | 1.00        | 0.96          | 12            |
| healty        | 1.00          | 0.92        | 0.96          | 12            |
|               |               |             |               |               |
| accuracy      |               |             | 0.96          | 24            |
| macro avg     | 0.96          | 0.96        | 0.96          | 24            |
| weighted avg  | 0.96          | 0.96        | 0.96          | 24            |


#### Confusion Matrix
![Result](https://github.com/Robatjazi/COVID-19/blob/master/covid-19_1.png)



#### Loss and Accuracy
![Result](https://github.com/Robatjazi/COVID-19/blob/master/covid-19_2.png)


