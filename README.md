# MN-Face-expression-recognition-
### 1.introduction


in this project a took kaggle challenge
the data comes from https://www.kaggle.com/c/challenges-in-representation-learning-facial-expression-recognition-challenge .

i choosed to do a machine learning project that can recognize the facial expression (happy face , sad face).

Each image corresponds to a facial expression in one of 2 categories (0=happy, 1=sad). The dataset contains approximately 307 images.

### 2.Remove low quality  images

we first wented to clean up the data to remove low quality images and potentially dangerous images that could affect our project.

![Screenshot 2022-2](https://user-images.githubusercontent.com/76142720/207522112-5413e10e-79c7-446a-8778-cc459698f3e3.png)

### 3.LOAD DATA

we can all guess which image is related to which emotion. happy or sad

This task is quite easy for a human, but it may be a bit challenging for a predictive algorithm because:

the images have a low resolution.

the faces are not in the same position.

some images have text written on them.

some people hide part of their faces with their hands.
other images are in the back ground. 

However all this diversity of images will contribute to make a more generalizable model.

![Screenshot 2022-1](https://user-images.githubusercontent.com/76142720/207521137-4d66092f-a106-48d2-8e7f-cb32908bc8e8.png)

### 4.scale data

Once we have a dataset, we can apply transformations to prepare the data for the model

(as_numpy_iterator). Returns an iterator which converts all elements of the dataset to numpy.
Use as_numpy_iterator to inspect the content of the dataset. 
To see element shapes and types, print dataset elements.

ref: https://www.tensorflow.org/api_docs/python/tf/data/Dataset

![Screenshot 2022-3](https://user-images.githubusercontent.com/76142720/207532925-73673b0c-28c1-49ee-9a9a-9380d0303979.png)

