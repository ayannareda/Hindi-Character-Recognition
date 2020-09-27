# Hindi-Character-Recognition
Recognises Hindi Character using pen gesture drawn in front of a camera. <br />
The project is trained on 36 Devanagari Characters. <br />
Uses CNN based Deep learning for recognising the Hindi characters .<br /><br />

Used contour detection for Hindi Character Recognition using pen gestures.<br /><br />

Used 36 hindi devanagri characers to classify gesture.<br />
Dataset can be downloaded from https://archive.ics.uci.edu/ml/datasets/Devanagari+Handwritten+Character+Dataset<br /><br />

Procedure :-<br />
1. Create ".csv" file for all gestures using Create_csv.ipynb<br />
3. Train our model using Training.ipynb<br />
4. Run Character detection using Hindi_character_detection.ipynb<br /><br />

Methodology :-<br /><br />

Dataset Collected :-<br />
The image database of Handwritten Devanagari characters. <br />
There are 36 classes of characters with 2000 examples each. <br />
The dataset is split into training set(85%) and testing set(15%).<br /><br />

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
We acheived 96.90% traning accuracy.<br /><br />

Training Accuracy :-<br /><br />
<img src="https://github.com/gearhead0909/Hindi-Character-Recognition/blob/master/Accuracy.png" alt="alt text" width="500" height="300"><br />

Training Loss :-<br /><br />
<img src="https://github.com/gearhead0909/Hindi-Character-Recognition/blob/master/Loss.png" alt="alt text" width="500" height="300"><br />

Evaluating the Model :-<br />
Evaluated the model on the test dataset.<br />
Achieved an accuracy of 91.89% generalised accuracy.<br /><br />

Saving the Model :-<br />
Then we will save our model for future use.<br /><br />

Then start Hindi_Character_Recognition.ipynb to run our real time project.<br />
A sample of the running project is shown below :-<br /><br />

<img src="https://github.com/gearhead0909/Hindi-Character-Recognition/blob/master/Screenshot.png" alt="alt text" width="500" height="300">
