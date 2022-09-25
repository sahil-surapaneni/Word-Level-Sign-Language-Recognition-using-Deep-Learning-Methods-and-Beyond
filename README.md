# Word-Level-Sign-Language-Recognition-using-Deep-Learning-Methods-and-Beyond
EECS 442 (Computer Vision) Final Project

## Introduction
Effectively using American Sign Language (ASL) is a pertinent problem for the roughly 600,000 deaf people in the United States [1]. Communicating through sign language for them is necessary but still difficult. For example,
ineffective communication with their health care providers
has led to health care avoidance among the deaf population [11]. Hence, there is a significant need in the wider
community for a way to accurately understand sign language.
Error rates in computer vision have decreased significantly since 2010 [4], hence computer vision models may
provide an effective way to translate sign language for
people with no familiarity in sign language. However,
many existing sign language models are out of date and
in-comprehensive [2]. ASL also depends on body movements and motions, which many models trained on images
do not capture, so it is important to make a model for videos.
Therefore, we explore several models in this paper to find
an effective solution for the problem of interpreting ASL.
Accurate computer vision models for recognising ASL
could also be applied to other sign languages through transfer learning or using similar models, making the task more
important as over 430 million people worldwide have ’disabling’ hearing loss, with this number set to increase to 700
million by 2050 [10].
In our work, we decided to explore the ways in which
machine learning models in video-related recognition tasks
can be applied to recognizing sign language words. We also
develop a baseline model to compare the performances to.

## Dataset
We used the Word-Level American Sign Language
[(WLASL)](https://github.com/dxli94/WLASL) dataset obtained from the official github [6],
which consists of sign videos from youtube and other
sources. The videos are of relative high quality, with the
signer standing in the center and facing directly at the camera. We chose this dataset since it is the largest dataset for
Word-Level American Sign Language Recognition. However, we found many of the videos they used in their original paper were now missing from the dataset, which became a source of issue for us. For consistency sake, we
used the data for the top 100 appearing glosses (words in
ASL). In their original dataset, they had 2038 videos across
the 100 glosses, while only 991 were available when we
downloaded. the dataset.

## Implementation
We slightly tweaked the existing preprocessing procedures from the github of the WLASL dataset [6] to get our
dataset. The preprocessing involved reading in each video
frame and then scaling and croping them to (224, 224, 3).
All the deep-learning models tested in this paper were
written from scratch. The inspiration for the models we
used came from a variety of papers published on Sign Language Recognition and video classification.
The models were implemented in PyTorch, and the pretrained models such as ResNet34 were obtained from the
torchvision models.
The baseline product manifold method was written from
scratch in Python based on the algorithm outlined in the
original paper about it [7].

## Full Information
Please Refer to **Final_Project_Writeup.pdf** in the repository for the full project writeup!

