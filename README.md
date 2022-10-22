#  anomaly detection on plant village dataset . 
### Anomaly detection .. what is it? :
Anomaly detection is one of the most common use cases of machine learning. Finding and identifying outliers helps to prevent fraud, adversary attacks, and network intrusions that can compromise your company’s future.
Generally speaking, an anomaly is something that differs from a norm: a deviation, an exception. In software engineering, by anomaly we understand a rare occurrence or event that doesn’t fit into the pattern, and, therefore, seems suspicious. Some examples are:

sudden burst or decrease in activity;
error in the text;
sudden rapid drop or increase in temperature.
![image](https://user-images.githubusercontent.com/95174361/197326075-9cd0042e-06d7-4d1e-9e07-6391a6afb1c5.png)


In our case , the anomalies will be image outliers where the image will be of a plant leaf . 

some visualizations : 
![image](https://user-images.githubusercontent.com/95174361/197326145-248b0e77-a60d-42e3-b533-35694da0fdbf.png)
healthy leaves 
![image](https://user-images.githubusercontent.com/95174361/197326174-0cc09810-d855-4add-a447-46772dd195d8.png)
diseased leaves:
![image](https://user-images.githubusercontent.com/95174361/197326191-c490d81f-21bd-4096-a7bb-3a1fd69337a3.png)

Main library used to detect : Alibi-detect ,
Alibi Detect is an open source Python library focused on outlier, adversarial and drift detection. The package aims to cover both online and offline detectors for tabular data, text, images and time series. The outlier detection methods should allow the user to identify global, contextual, and collective outliers.
I have used Auto Encoder to detect outliers. there are many others like VAE ,prophet and some gaussian methods as well.
Documentation: https://docs.seldon.io/_/downloads/alibi-detect/en/v0.5.1/pdf/

Library used to detect and localize : tensorflow with globalAverage pooling layer and vgg16 model . 
