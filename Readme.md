CS 203: Software Tools & Techniques for AI
IIT Gandhinagar
Sem-II - 2024-25

________________________________________________________________

LAB 05

Total marks: 10

Submission deadline: 

Submission guidelines:

Code should be added to a GitHub repository, and the repository details should be shared.
Late submissions will be penalized 20% per day.

Google form submission link:

Note: By submitting this assignment solution you confirm to follow the IITGN's honor code. We shall strictly penalize the submissions containing plagiarized text/code.
________________________________________________________________

The goal of this assignment is to apply data augmentation techniques to improve the performance of an image classification model that distinguishes between cats and dogs.

This lab is to be completed in teams of size 2 students. Each team will annotate the data and then compute the inter-annotator agreement scores.

Task 1: Data Augmentation

Download the Cat & Dog Dataset (https://www.kaggle.com/datasets/samuelcortinhas/cats-and-dogs-image-classification?select=test) (Only download the test dataset; do not take the training dataset)

Create a train and test set (train-test ratio should be 80:20%).

Create Custom Function using Augly which will perform multiple random data augmentation according to input. (At least 10 data augmentation needs to be added like rotate, cropping, blur …)

Perform data augmentation using the above function, only on the train set. (The number of augmented images should be twice the train set, and images should be augmented thrice example: cropped → rotate→Blur)

Show the statistics of the newly created dataset. (Old dataset count and new dataset count)

Task 2: Model Training

Note: Initial weights of the model should be the same when training with both datasets.

Choose (microsoft/resnet-50)model from the hugging face and initialize its new weights.

Train model(created in the above point) on a downloaded dataset, without augmentation.

Train model(created in the first point) on a downloaded dataset with augmentation.

Get the precision, recall, F1 score, and accuracy of both the models on the test set.

Evaluation Criteria

Data Augmentation  (40%) :
Proper code

Showing bar graph for counts.

Train & Test

Augmented Train Set & Without Augmented Train Set

Number of Cat & Dog Images in both a train set and a test set.

Basics of ML (Like cat and dog images in the test set should be balanced)

Model Training (40%) :

Training parameters and information.

Model taken and its architecture diagram.

Properly calculating evaluation metrics without any library.

If getting poor/good results, then give an explanation. (At most 5 lines of explanation)

Documentation (20%) :

Proper documentation of code, graphs, and metrics.

