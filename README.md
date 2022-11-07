Baseline Performance Markdown
Introduction
In this markdown, we will go over the base performance of the semantic segmentation of satellite imagery given the seed repository and necessary adjustments. To begin, the given seed repository gives us an idea of what a basic form of semantic segmentation is capable of without any form of optimization.

Data Preprocessing
For the preparation of data, we followed the guidelines laid out in the video by "Digital Sreeni" in that we began by first taking and "normalizing" the data given. In this case, it was a set of photos that were all of different sizes. Using patchify, we cut images into easily divisible sections. Each section was then placed into a numpy array. It is from that array that we begin to fed our training algorithm. Specifically, the images were broken up into patches that were easily divisible by 256 i.e. 2048 x 1024. To ensure that this had been done properly, we followed the example given and ran checks throughout the code to observe any results. Once the photos were in proper size, we began to replace the RGB pixel information with numpy int values. From there, we were able to begin properly processing the data and running the trainers.

Training
For training, we run a multiple unet model with a total loss function. In the modeling, we train in batch sizes of 16. In our case we simply chose to follow the guidelines and run one hundred total epochs for training this model. Noticeably, the performance here is poor. The model takes a significant amount of time to train, though it does produce favorable results. The loss was minimal throughout runtime, and rarely went over a value 1.01.

UNET
Results
Link to all results posted here (in a separate file) https://github.com/Jihxdul/Semantic-Segmentation-of-Satellite-Imagery/blob/milestone-2/MileStone-2-Results.md
