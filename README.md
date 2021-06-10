# Image-Captioning-with-InceptionV3-

Image captioning integrates two subtasks of objection detection and text generation for creating captions for the input images. Image captioning models usually entail a feature extraction model and a RNN model for sequence generation. This project uses a baseline model [1] for image captioning and improves this model with a better feature extraction model ([InceptionV3](https://cloud.google.com/tpu/docs/inception-v3-advanced))[4] and some RNN modifications (with GloVe embedding [2]). The dataset for training the model is Flickr8k [3]. In this dataset each image is labeled with five short sentences that describe the image. Below is a sample image with its descriptive captions. 

![image](https://user-images.githubusercontent.com/34719495/121538769-0a1eb880-c9d3-11eb-8bff-800253938721.png)

Dog with brindlecolored coat is running across the yard.

Brown dog with red collar jumping across the leafy lawn. 

Brown and black dog runs through the leaves. 

The brown dog is wearing red collar. 

Brown dog is running.

The image captioning model has to learn how to come up with the best caption for any given picture. So the model has an object detection module and a text generation algorithm combined together. The InceptionV3 model, which performs the object detection task, is an improvement upon Google’s original InceptionV1 (GoogleNet) model. This model introduces the idea of an Inception layer, a combination of 1x1, 3x3, and 5x5 Convolutional layers concatenated into a single output vector.






## References
1. How to Develop a Deep Learning Photo Caption Generator from Scratch, by Jason Brownlee on June 27, 2019 in Deep Learning for Natural Language Processing.
2. Pennington, Jeffrey, Richard Socher, and Christopher D. Manning. "Glove: Global vectors for word representation." Proceedings of the 2014 conference on empirical methods in natural language processing (EMNLP). 2014.
3. Rashtchian, Cyrus, et al. "Collecting image annotations using amazon’s mechanical turk." Proceedings of the NAACL HLT 2010 Workshop on Creating Speech and Language Data with Amazon’s Mechanical Turk. 2010.
4. Szegedy, Christian, et al. "Rethinking the inception architecture for computer vision." Proceedings of the IEEE conference on computer vision and pattern recognition. 2016.

