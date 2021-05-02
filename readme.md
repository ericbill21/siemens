# Siemens Mobility’s AI Dependability Assessment

Dependability and reliability of machine learning classification systems are getting increasingly important as machine learning techniques are being applied in more and more domains, including safety-critical areas.
The task of the Siemens AI Dependability Assessment Student's Challenge is to provide a classifier for a given classification tasks as well as to determine an as-accurate-as-possible misclassification probability estimate.

In this paper, we describe a machine learning model that has been optimized for the safest classification possible. 
A multilayer feed-forward neural network was trained on the three given datasets. 
We introduce a custom loss function to reduce the number of safety-critical misclassifications.
Additionally, we detect predictions that are less certain than a determined threshold value and decide to resort to a safer classification in these instances.

Moreover, we describe the approach taken to determine a probability estimate for misclassifications: As training data quality is crucial to model performance and dependability, we develop several interpretations of training data and use these as indicators to estimate model accuracy. 

For the three given datasets, our approach provides reliable (though not guaranteed) misclassification rates no larger than 6.89%, 2.34%, and 2.62%, respectively.
