# Dance-Form-Classification
 Model To classify 8 Indian Classical Dance forms.


1.Importing all the necessary packages needed to build the Model.<br>
2.Using Pandas , Reading the train.csv file to get the names of images and with the help of cv library , preprocessing the images and converting them into arrays of equal widths and heights , here Width = 224.<br>
3.For creating y_train data,  Performed one_hot_encoding on the 8 classes and also keeping a label_to_category mapping to map the predictions.<br>
4.Because the dataset used is small and can lead to overfitting , Data Augmentation is used to generate more data .Hence preventing the overfitting of the data.<br>
5.In this particular problem I've used Xception Model with activation function , "Relu" .<br>
6.Hyperparatmeters used are : loss        -> categorical_crossentropy<br>
			      optimizer   -> Adam optimizer<br>
			      metrics     -> accuracy<br>
			      batch_size  -> 32<br>
			      epochs      -> 325<br>
			      output      -> sigmoid<br>


7.After Compiling the Model , <br>
Accuracy        : 0.9828 <br>
Loss            : 0.1229<br>
Validation Loss : 2.1347<br>
Validation Acc  : 0.8219<br>


8.After this we follow the step 2 to generate the Testing Data .<br> 
9.Then Keeping the predictions in the csv file using csv library.  <br>
