Syed Alam & Anosh Abraham

Knowledge Distillation

In this milestone 4, we created a new network that is smaller than the original and trained it using knowledge distillation. After training, we got our precision-recall values. One of the best ways to improve the performance of any algorithms in machine learning is to train many different models on the same data set and look at the average outcomes of the predictions. 

Knowledge distillation refers to the process of transferring knowledge from a larger model to a single small model that can be used under different variables. In order to use knowledge distillation we needed the following information. The first action is to create both teacher and student models. Here we assumed that the teacher is trained and fixed after which we then distill teacher to student. We essentially train a smaller model based on the already trained bigger model. Smaller model learns the behavior of the bigger model. 

![image](https://user-images.githubusercontent.com/91106087/205528865-87956155-5ca4-40c0-b0d5-e6d8c5cfd245.png)

![image](https://user-images.githubusercontent.com/91106087/205551575-a0e1e934-c52f-4cdf-91de-e8f7dfcbeff0.png)

![image](https://user-images.githubusercontent.com/91106087/205551603-b53acad9-3642-45c8-9149-6cb47d1be04c.png)

![image](https://user-images.githubusercontent.com/91106087/205551617-c8c8a539-29ed-440d-8597-e8244cbb2904.png)

![image](https://user-images.githubusercontent.com/91106087/205551635-f26bd42a-a021-4de7-8a0f-813631ebdcd4.png)

![image](https://user-images.githubusercontent.com/91106087/205551644-cc6a5e27-0ee0-4732-8657-e07be14da391.png)



We believe it will be necessary to use knowledge distillation in the future as we use larger models but have less available processing power to back them.
