# deep-learning-classification

## Summary

Within this challenge, I started out importing the tensorflow dependency which will ultimately allow me to execute splitting the data, create my X/y train/test variables, perform the keras sequential model, and perform the accuracy function to showcase the accuracy of my data set.

The first thing I did after reading the csv file was clean up the database by dropping the uneccesary columns into a new data frame. From there I dran a quick summary of the unique values within each column. After choosing my focus column APPLICATION TYPE and CLASSIFICATION, I went ahead and cleaned it up so that it is uniformed for when I create a get_dummies formula. 

Once the get_dummies df has been created, which is in a numerical format, I choose 'Is Successful as my target/feature arrays. The Xz an Y variables I created were then used in the X/y train/test values. From here, I scaled the X/y train/test data set by using the sctandardscaler() function, allowing me next to play around with layers/nuerons which will ultimately help me increase/decrease the accuracy of my data.

Lastly, to get to the accuracy calculation point, I chose to create 4 layers for my dataset, toggling with the units to try and raise the accuracy percentage. Once I decided on the number of layers I was satisfied with, I fitted and trained the model to generate the invidual accuruaccy levels within 100 epochs. Once that finshed runnig, I then ran the accuracy summary as well as saved that dataset into a HDF5 file.


## Results: Using bulleted lists and images to support your answers, address the following questions:

As mentioned in the summary, I chose 'Is Successful' as my target variable (y) and the rest of the columns as my feature variables (X) to create my new df that is later used to create the dummies set and then the kera squential model.

Because of my how long I was playing around with the number of layers/nuerons, I stuck with just the 4 layers, which generated an accuracy level of 72.92, which isn't ideal, but I'm sure whith even more layers and nuerons, the accuracy level could get well in the 80th percentile.

Here is a snapshot of the final summary evaluation of the dataset:
268/268 - 0s - 365us/step - accuracy: 0.7292 - loss: 0.5653
Loss: 0.5653499960899353, Accuracy: 0.7292128205299377

## Final Thoughts
While it took me a lot of trial and error to still not be able to get an accuracy level of 75% or higher, I would say that is one of the most challenging parts of using this method. That and figuring out the data parameters to ensure the model fits when setting the input_dim variable, otherwise it won't be able to run the model_fit process, which then you woudl use to get teh accuracy and other stats.


Summary: Summarize the overall results of the deep learning model. Include a recommendation for how a different model could solve this classification problem, and then explain your recommendation.



Data Preprocessing

What variable(s) are the target(s) for your model? "Is_Successful"
What variable(s) are the features for your model?
What variable(s) should be removed from the input data because they are neither targets nor features?
Compiling, Training, and Evaluating the Model

How many neurons, layers, and activation functions did you select for your neural network model, and why?
Were you able to achieve the target model performance? No as I was not able to come up with enough nuerons and units to get the target model performance.
What steps did you take in your attempts to increase model performance? "implemented more layers/nuerons to try and increase the accuracy, which is a big feat in itself.


