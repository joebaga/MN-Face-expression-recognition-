# MN-Face-expression-recognition-
### 1.introduction


in this project a took kaggle challenge
the data comes from https://www.kaggle.com/c/challenges-in-representation-learning-facial-expression-recognition-challenge .

i choosed to do a machine learning project that can recognize the facial expression (happy face , sad face).

Each image corresponds to a facial expression in one of 2 categories (0=happy, 1=sad). The dataset contains approximately 307 images.

### 2.Remove low quality  images

we first wented to clean up the data to remove low quality images and potentially dangerous images that could affect our project.

![Screenshot 2022-2](https://user-images.githubusercontent.com/76142720/207522112-5413e10e-79c7-446a-8778-cc459698f3e3.png)

### LOAD DATA

we can all guess which image is related to which emotion. happy or sad

This task is quite easy for a human, but it may be a bit challenging for a predictive algorithm because:

the images have a low resolution.

the faces are not in the same position.

some images have text written on them.

some people hide part of their faces with their hands.

However all this diversity of images will contribute to make a more generalizable model.

![Screenshot 2022-1](https://user-images.githubusercontent.com/76142720/207521137-4d66092f-a106-48d2-8e7f-cb32908bc8e8.png)
