Syed Alam & Anosh Abraham

In this milestone 4, we created a new network that is smaller than the original and trained it using knowledge distillation. After training, we got our precision-recall values. One of the best ways to improve the performance of any algorithms in machine learning is to train many different models on the same data set and look at the average outcomes of the predictions. 

Knowledge distillation refers to the process of transferring knowledge from a larger model to a single small model that can be used under different variables. In order to use knowledge distillation we needed the following information. The first action is to create both teacher and student models. Here we assumed that the teacher is trained and fixed after which we then distill teacher to student. 

![image](https://user-images.githubusercontent.com/91106087/205528865-87956155-5ca4-40c0-b0d5-e6d8c5cfd245.png)
