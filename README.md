# Hindi-Character-Recognition
Recognises Hindi Character using pen gesture drawn in front of a camera. The project is trained on 36 Devanagari Characters. Uses CNN based Deep learning for recognising the Hindi characters .
Emoji detection using hand gestures.<br /><br />

Used contour detection for Emoji Recognition using hand gestures.<br /><br />

Used 12 emojis to classify hand gesture.<br />
Emoji dataset can be downloaded from https://www.kaggle.com/eliasdabbas/emoji-data-descriptions-codepoints?select=Screen+Shot+2019-04-04+at+12.59.10+AM.png<br /><br />

Procedure :-<br />
1. Create hand gestures dataset using Create_Dataset.ipynb<br />
2. Create ".csv" file for all hand gestures using Create_csv.ipynb<br />
3. Train our model using Training.ipynb<br />
4. Run Emoji detection using Emoji_Detection.ipynb<br /><br />

Methodology :-<br /><br />

Creating hand gesture dataset :-<br />
Used webacam to captue hand gestures.<br />
Detected hand colors using cv2.inRange().<br />
Detected contours of hand gestures and captured 1000 images of each classes.<br /><br />

Creating csv file for gesture dataset :-<br />
Converted images in array using np.asarray()<br />
added class number in the first column of the dataframe<br />
and stored in a csv file.<br /><br />

Pre-processing of data :-<br />
Imported teh dataset<br />
Shuffled all the rows in our dataset.<br />
And sliced the Data and class labels from our dataset.<br /><br />

Then, we split the data and labels into training and testing part<br />
To feed our labels to our model, one-hot encode them.<br /><br />

Building the model :-<br />
After preparing our data<br />
We will build our CNN based Deep Neural Network using Keras library.<br />
After building our model<br />
Compile our model with<br />
Loss = "Categorical_Crossentropy"<br />
Optimizer = "Adam"<br /><br />

Training the model :-<br />
Then we will train our model on prepares Data and labels.<br />
We acheived 99.96% traning accuracy.<br /><br />

Saving the Model :-<br />
Then we will save our model for future use.<br /><br />

Then start Emoji_recognition.ipynb to run our real time project.<br />
A sample of the running project is shown below :-<br /><br />

<img src="https://github.com/gearhead0909/Emoji-Recognition/blob/master/Emoji%20Recognition%20screenshot.png" alt="alt text" width="500" height="300">
