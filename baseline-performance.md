We ran our program in order to get the 10 prediction images that would be compared to the testing label. 
Since the amount of time it would take to run 100 epochs was taking too long even with colab pro we reduced the number to 3 epochs to save time. 
Because of this the accuracy of the predictions are going to be noticeably less accurate than running through with 100 epochs. 
For some images the prediction was pretty accurate. For others it wasn’t accurate at all. 
Some of the testing labels don't line up with the testing image that was being displayed and or were blank. 
This also most likely has an effect on how the graphs look like for both the training and validation loss vs epochs as well as the precision recall curves. 
Even with only 3 epochs, the predictions were fairly accurate to the testing image/label. 
We could not get through with graphing the precision and recall curves on time so we cannot comment on the issue.
