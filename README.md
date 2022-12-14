# MN-Face-expression-recognition-
# 1.introduction


in this project i took a kaggle challenge
the data comes from 

https://www.kaggle.com/c/challenges-in-representation-learning-facial-expression-recognition-challenge .

i choosed to do a machine learning project that can recognize the facial expression (happy face , sad face).

Each image corresponds to a facial expression in one of 2 categories (0=happy, 1=sad). The dataset contains approximately 307 images.

# 2.Remove low quality  images

we first wented to clean up the data to remove low quality images and potentially dangerous images that could affect our project.

![Screenshot 2022-2](https://user-images.githubusercontent.com/76142720/207522112-5413e10e-79c7-446a-8778-cc459698f3e3.png)

# 3.LOAD DATA

we can all guess which image is related to which emotion. happy or sad

This task is quite easy for a human, but it may be a bit challenging for a predictive algorithm because:

the images have a low resolution.

the faces are not in the same position.

some images have text written on them.

some people hide part of their faces with their hands.
other images are in the back ground. 

However all this diversity of images will contribute to make a more generalizable model.

![Screenshot 2022-1](https://user-images.githubusercontent.com/76142720/207521137-4d66092f-a106-48d2-8e7f-cb32908bc8e8.png)

# 4.scale data

Once we have a dataset, we can apply transformations to prepare the data for the model

(as_numpy_iterator). Returns an iterator which converts all elements of the dataset to numpy.
Use as_numpy_iterator to inspect the content of the dataset. 
To see element shapes and types, print dataset elements.

ref: https://www.tensorflow.org/api_docs/python/tf/data/Dataset

![Screenshot 2022-3](https://user-images.githubusercontent.com/76142720/207532925-73673b0c-28c1-49ee-9a9a-9380d0303979.png)

# We define our CNN
We apply the ReLU function to introduce non linearity in our CNN
### ReLU
![Screenshot 2022-5](https://user-images.githubusercontent.com/76142720/207539044-01102c8f-9d21-4495-ba2a-8c57a82bca56.png)

 ReLU for short is a piecewise linear function that will output the input directly if it is positive, otherwise, it will output zero
 ### sigmoid
![4](https://user-images.githubusercontent.com/76142720/207536164-bf2cb81b-68b8-4486-9a05-1b26e4084471.gif)

in our case it's happy face or sad face;

we used a sigmoid function as our last activation function.
The main reason why we use sigmoid function is because it exists between (0 to 1). 
Therefore, it is especially used for models where we have to predict the probability as an output.
Since probability of anything exists only between the range of 0 and 1, sigmoid is the right choice.

# Train the model
Our best model managed to obtain a validation accuracy of approximately 98%

![Screenshot 2022-6](https://user-images.githubusercontent.com/76142720/207540575-644dff3a-6a1d-4954-ba81-63aa60ec4479.png)

# Analyze the results
We got outputs at each step of the training phase

![Screenshot 2022-7](https://user-images.githubusercontent.com/76142720/207542543-c75a1837-e8af-484e-841f-34c59ea1ad71.png)
![Screenshot 2022-8](https://user-images.githubusercontent.com/76142720/207542568-b0451956-e5ac-4444-89b5-4112774361f4.png)

# TEST 

![Screenshot 2022-9](https://user-images.githubusercontent.com/76142720/207545406-416bf253-9e7e-4ce0-846b-0a6d2104f651.png)

# ref
https://www.kaggle.com/c/challenges-in-representation-learning-facial-expression-recognition-challenge

https://developers.google.com/machine-learning/testing-debugging/metrics/interpretic

https://www.tensorflow.org/api_docs/python/tf/data/Dataset
