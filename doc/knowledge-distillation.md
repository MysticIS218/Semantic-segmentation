Syed Alam & Anosh Abraham

Knowledge Distillation

In this milestone 4, we created a new network that is smaller than the original and trained it using knowledge distillation. After training, we got our precision-recall values. One of the best ways to improve the performance of any algorithms in machine learning is to train many different models on the same data set and look at the average outcomes of the predictions. 

Knowledge distillation refers to the process of transferring knowledge from a larger model to a single small model that can be used under different variables. In order to use knowledge distillation we needed the following information. The first action is to create both teacher and student models. Here we assumed that the teacher is trained and fixed after which we then distill teacher to student. We essentially train a smaller model based on the already trained bigger model. Smaller model learns the behavior of the bigger model. 

![image](https://user-images.githubusercontent.com/91106087/205528865-87956155-5ca4-40c0-b0d5-e6d8c5cfd245.png)

![image](https://user-images.githubusercontent.com/91106087/205551436-855df07d-c5fe-4a82-83dc-dbc89415b42b.png)

![image](https://user-images.githubusercontent.com/91106087/205551457-dc8db8a4-6294-4106-8e7d-fb2930b78587.png)

![image](https://user-images.githubusercontent.com/91106087/205551478-531f3cb1-66f5-49dd-bb9d-c5d3484167f6.png)

![image](https://user-images.githubusercontent.com/91106087/205551488-075560f4-d5b9-42dc-bae5-c12e3023ec45.png)

![image](https://user-images.githubusercontent.com/91106087/205551498-e8ae6342-c1c5-4a78-8d26-33ca0bac4814.png)


We believe it will be necessary to use knowledge distillation in the future as we use larger models but have less available processing power to back them.

Implementing KD to our satellite segmentation imagery results in a better prediction before without it just like the results with our HPO method.

The curves however barely had any change to them with no changes in any trends.
