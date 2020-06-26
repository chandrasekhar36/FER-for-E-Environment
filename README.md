# FER-for-E-Environment
The main aim of this project is to detect the emotion of a learner in E-Learning system by using his/her visual features
First I collected the data from public dataset DAiSEE(Data with 9068 video sequences over #112 of subjects). Then, crop the frames for every video sequence and assign a label to it.

Steps to be followed: (Read carefully to run)

Step 1:
Run Load_split_dataset module to load the data from directories and shuffle them and split them into 80% and 20% for trainig and testing purpose.Then, performe contrast limited histogram equilization for evry image and store the same in pickle file.

step 2: Run the Train_dataset module to train the model.Its a hybrid approach where the features are extracted from images using (CNN + Handcarfted Model) followed by classification by SVM classifier. The trained model is available in res.

step 3: Run the FER module to use the trained model.

The features are extracted from an handcrafted model apart from the CNN. Next, The both features are combined and trained over a traditional ML classifier.

The proposed hybrid model can increase the accuracy(5% in this work). The Schematic diagram of proposed system is depicted below

![Proposed Hybrid Model](https://github.com/chandrasekhar36/FER-for-E-Environment/blob/master/res/Hybrid_model%20Architecture.png)
