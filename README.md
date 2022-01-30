# Credit_Risk_Analysis

## Ensemble
Ensemble learning is the process of combining multiple models to improve the accuracy and robustness of the model. This will increase the overall performance of the model. 


The first ensemble model that was used is the Balanced Random Forest Classifier. Random Forsts takes several small tress where the results are not much better than a guess and combines them together for much better decision making power. 

Although the Balanced Accuracy Score is .77 , the f1 score for High Risk is only .06. This model is not accurate enough to provide a good prediction.

![image](https://user-images.githubusercontent.com/88912539/151712709-8ad67566-9c19-4659-9fc9-60194a45304e.png)


The next ensemble model that was tested is the Easy Ensemble AdaBoost Classifier. Like the Balanced Random Forest Classifier, this model provides a Balanced Accuracy Score of .93 but the f1 score for high risk is only .16 making it unacceptable for preditions.

![image](https://user-images.githubusercontent.com/88912539/151712725-e88b8f74-2040-48b1-87d7-12a7d8676c72.png)


## Resampling 

Resampling is the process of correcting Class Imbalance to provide a more accurate model by over samplingor under sampling. 

Running a Naive Randam Oversampling model did not provide an acceptable level of accuracy to be useful. The Balanced Accuracy Score for this model was lower than for the Ensemble models at .65 but the f1 reveals a score of just .02. 

![image](https://user-images.githubusercontent.com/88912539/151712798-9bd43e94-6ed5-4376-917d-6261d4e338a7.png)


When using the SMOTE Oversampling, the results were similar to the Naive Randam Oversampling with a Balanced Accuracy Score of .64 and an f1 of .02. 
![image](https://user-images.githubusercontent.com/88912539/151712806-0999e687-c4e3-4ffd-942c-847ea17014d8.png)


Oversampling did not provide a good predictive model so we next ran an Undersampling model. Undersampling proved to be even more inaccurate than oversampling with a Balanced Accuracy Score of just .54 and a f1 score of .01
![image](https://user-images.githubusercontent.com/88912539/151712817-a43fd5b9-d55b-46e7-832e-f01e03c7d007.png)


The final model that was a combination of over and under sampling. This model will provide evidence that over/under sampling did not yield better results. The Balanced Accuracy Score was .67 with the f1 score at .02. 

![image](https://user-images.githubusercontent.com/88912539/151712918-c6bc2c55-707c-48c3-963b-7a34e0cb3d40.png)

The data shows that the ensemble models were slightly better than resampling, I would conclude that none of these models were accurate enough to provide meaningful predictions. 
