Syed Alam & Anosh Abraham


In this markdown, we will discuss the hyperparameter optimization method we used in order to improve the prediction accuracy when compared to the testing image and testing label. The method we were assigned was evolution. This method fine-tuned the model hyperparameters to improve the model’s performance on a validation set. Hyperparameter evolution is a method of Hyperparameter Optimization using a Genetic Algorithm (GA) for optimization.

Before implementing the method, our predicted images were fairly accurate but not accurate enough to the testing labels or images. This was when we ran the code with 3 epochs with verbose equalling 1 and batch size equalling 16. But now we editted the file to accept 100 epochs in a timely manner than before.

With this change we utilized a function called GASearchCV that implements the evolution hyperparameter optimization. With this function GASearchCV had many more parameters to include into the code. Next we trained and optimized the estimator `evolved_estimator.fit(X_train, y_train)`.

By implementing the evolutionary hyperparameter optimization, we got a noticeable but not substantial difference in predicted images when compared to the images we had previously in milestone 2. Some images are noticably more accurate compared to others when running with the HPO method. But it is still not close enough for it to be close to the testing labels and testing images. However, this does prove that hyperparameter methods do work in order to have more accurate predictions when training a validation set.h

The training loss and validation loss graph shows an overfit with validation loss having an increasing trend while training loss having a decreasing trend. With training and validation IoU, both training and validation IoU's have an increasing trend. With this we can see that the training loss was slowly decreasing while validation loss steadily increased with each passing epoch due to the HPO method we used. We could not get through with graphing the precision and recall curves so we cannot comment on the issue. However, we can conclude through assumption from the predicted images data, the precision/recall curves would have been more accurate as the parameters were more defined. As well having a greater number of epochs resulting in a more accurate predicted image. 
