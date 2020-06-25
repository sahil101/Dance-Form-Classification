# Dance-Form-Classification
 Model To classify 8 Indian Classical Dance forms.


1.Importing all the necessary packages needed to build the Model.
2.Using Pandas , Reading the train.csv file to get the names of images and with the help of cv library , preprocessing the images and converting them into arrays of equal widths and heights , here Width = 224.
3.For creating y_train data,  Performed one_hot_encoding on the 8 classes and also keeping a label_to_category mapping to map the predictions.
4.Because the dataset used is small and can lead to overfitting , Data Augmentation is used to generate more data .Hence preventing the overfitting of the data.
5.In this particular problem I've used Xception Model with activation function , "Relu" .
6.Hyperparatmeters used are : loss        -> categorical_crossentropy
			      optimizer   -> Adam optimizer
			      metrics     -> accuracy
			      batch_size  -> 32
			      epochs      -> 325
			      output      -> sigmoid


7.After Compiling the Model , 
Accuracy        : 0.9828 
Loss            : 0.1229
Validation Loss : 2.1347
Validation Acc  : 0.8219


8.After this we follow the step 2 to generate the Testing Data . 
9.Then Keeping the predictions in the csv file using csv library.  