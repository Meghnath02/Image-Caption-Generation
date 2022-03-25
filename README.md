# Image-Caption-Generation
This project requires basic Deep Learning concepts like Convolution Neural Networks, Transfer Learning, Recurrent Neural Networks, Gradient Descent, Feed-Forward, Back-propagation, Text Processing, Python syntax, Python data structures, Keras library etc.

#### DATA: Flickr 30k
It contains 30K images and 5 Captions for every image file.

#### Image Feature Extraction: Transfer Learning technique 
Used VGG as base model for transfer learning and weights as “imagenet” . Removed the last layer from the loaded model, as this is the model used to predict a classification for a photo.


#### Merge Model
The merge model combines both the encoded form of the image input with the encoded form of the text description generated so far.
The combination of these two encoded inputs is then used by a very simple decoder model to generate the next word in the sequence.
The approach uses the recurrent neural network only to encode the text generated so far.

#### Metric: BLEU
BLEU stands for Bilingual Evaluation Understudy.
It is an algorithm, which has been used for evaluating the quality of machine translated text. We can use BLEU to check the quality of our generated caption.
