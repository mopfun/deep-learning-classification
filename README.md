# deep-learning-classification

## Summary

Within this challenge, I started out importing the tensorflow dependency which will ultimately allow me to execute splitting the data, create my X/y train/test variables, perform the keras sequential model, and perform the accuracy function to showcase the accuracy of my data set.

The first thing I did after reading the csv file was clean up the database by dropping the uneccesary columns into a new data frame. From there I dran a quick summary of the unique values within each column. After choosing my focus column APPLICATION TYPE and CLASSIFICATION, I went ahead and cleaned it up so that it is uniformed for when I create a get_dummies formula. 

Once the get_dummies df has been created, which is in a numerical format, I choose 'Is Successful as my target/feature arrays. The Xz an Y variables I created were then used in the X/y train/test values. From here, I scaled the X/y train/test data set by using the sctandardscaler() function, allowing me next to play around with layers/nuerons which will ultimately help me increase/decrease the accuracy of my data.

Lastly, to get to the accuracy calculation point, I chose to create 4 layers for my dataset, after time toggling with the neurons, layers, and activation function, in attempt to increase the accuracy percentage. Once I decided on the number of layers I was satisfied with, I fitted and trained the model to generate the invidual accuruaccy levels within 100 epochs. Once that finshed runnig, I then ran the accuracy summary as well as saved that dataset into a HDF5 file.


## Results

As mentioned in the summary, I chose 'Is Successful' as my target variable (y) and the rest of the columns as my feature variables (X) to create my new df that is later used to create the dummies set and then the kera squential model.

After trying multiple number of nuerons, layers, and different activation functions, I ended up sticking with just the 4 neurons,layers, and activation functions which generated an accuracy level of 72.92%, which isn't ideal, but I'm sure whith even more layers and nuerons, the accuracy level could get well in the 80th percentile. I thoughht it was interesting that while I was playing with the layering, that while increasing the number of nuerons can be helpful, it can also be just as uneccessary as the increased learning also includes the noise within the data, creating an overfitting process. This can ultimately create poor performance on new unseen data.

Here is a breakdown of the final summary evaluation of the dataset:
268/268 - 0s - 365us/step - accuracy: 0.7292 - loss: 0.5653
Loss: 0.5653499960899353, Accuracy: 0.7292128205299377

## Final Thoughts
While it took me a lot of trial and error to still not be able to get an accuracy level of 75% or higher, I would say that is one of the most challenging parts of using this method. That and figuring out the data parameters to ensure the model fits when setting the input_dim variable, otherwise it won't be able to run the model_fit process, which then you woudl use to get the accuracy and other stats.

With more practice and knowledge of the neural network, I'm sure I will be able to get the accuracy up to a higher preference level, but again, there are cons in doing so depending on how much you add within the neurons, layers, and activation functions.

I think another method to consider would be the keras-tuner method since the whole thought behind this method is to enhance the models machine learning through 'tuning' the hyperparameters before the training step. Doing this will allow the optimal combinations to be selected with the sample data, thus ultimately giving you the highest accuracy percentage generated through the machine learning.