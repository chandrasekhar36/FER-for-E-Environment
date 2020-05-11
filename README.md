# FER-for-E-Environment
The main aim of this project is to detect the emotion of a learner in E-Learning system by using his/her visual features
First I collected the data from public dataset DAiSEE(Data with 9068 video sequences). Then, crop the frames for every video sequence and assign a label to it.

Step 1:
Run Load_split_dataset module to load the data from directories and shuffle them and split them into 80% and 20% for trainig and testing purpose.Then, performe histogram quilization and store the same in pickle format 

step 2: Run the Train_dataset module to train the model.Its a hybrid approach where the features are extracted from images using CNN followed by classification by SVM classifier. The trained model is saved in res.

step 3: Run the FER module to use the trained model.
