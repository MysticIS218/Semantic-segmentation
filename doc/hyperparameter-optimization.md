Syed Alam & Anosh Abraham

In this markdown, we will discuss the hyperparameter optimization method we used in order to improve the prediction accuracy when compared to the testing image and 
testing label. 
The method we were assigned was evolution. 
This method fine-tuned the model hyperparameters to improve the model’s performance on a validation set. 
Hyperparameter evolution is a method of Hyperparameter Optimization using a Genetic Algorithm (GA) for optimization.

Before implementing the method, our predicted images were fairly accurate but not accurate enough to the testing labels or images. 
Since we can’t run 100 epochs for our predicted images because of runtime, we still ran with 3 epochs but this time with verbose being 3 since that’s the max number 
to run with for that variable. 
The batch size remaining the same with 16.
Verbose being equal to three doesn’t yield much of a difference nor affects the computation time much. 

We utilized a function called GASearchCV that utilizes the evolution hyperparameter optimization. 
With this function GASearchCV had many more parameters to deal with compared to history1 and history2 in the aerial imagery github file. 
Next we trained and optimized the estimator `evolved_estimator.fit(X_train, y_train)`.

By implementing the evolutionary hyperparameter optimization, we got a noticeable difference in predicted images when compared to the images we had previously in 
milestone 2 but not enough for it to be close to the testing labels and testing images. 
This does prove that hyperparameter methods do work in order to have more accurate predictions when training a validation set.
