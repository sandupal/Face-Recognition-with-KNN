# Face-Recognition-with-KNN

This project implements and evaluates KNN algorithim for Face Recognition using the Extended YaleB dataset.
The original images in the Extended YaleB dataset have been cropped and resized to 32 X 32. The dataset has 38 individuals 
and around 64 near frontal images underdi erent illuminations per individual. The file YaleB-32x32.mat contains variables "fea" and "gnd".
Each row of "fea" is a face and "gnd" is the label. Randomly selected (m = 10,20,30,40,50) images per individual with labels are used to form the
training set, and remaining images in the dataset are used as the test set. The K-NN algorithm (with k = 1) is applied on each of these five splits. 
Above procedure for k = 2,3,5,10 is repeated and the error rate E against k is plotted. The distance is the euclidean distance. Then this experiemnt
is repeated with Let k = 3 and m = 30 images per individual with labels to form the training set and remaining images in the dataset as the test set.
The distance metric is $p =1,3,5,10$ is used and errors are plotted against $p$ to examine how distance metric affects error rate. Initially pixel
intensities are used as features and subsequently LBP and HOG features are extracted from images and the process is repeated to understand how feature
extraction affects classification of images.
