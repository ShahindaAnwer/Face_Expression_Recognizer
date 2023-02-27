# Face Expression Recognizer

# Problem Statement
Facial expression recognition is a technology that detects emotions in human faces using biometric markers. It detects the 6 basic universal expressions; Happiness, Sadness, Anger, Surprise, Fear, and Disgust. Conveying nonverbal communication cues, Facial expressions play a powerful role in interpersonal relations, therefore, complementing speech by helping the listener to interpret the intended meaning of spoken words. Facial expression recognition is benificial to companies, as it helps them conduct market research, automatically measuring consumers' moment-by-moment facial expressions, making it easy to aggregate the results, resulting in better understanding of their needs. Facial expresion recognition can also be used in the video game testing phase, where developers gain insights and draw conclusions about the emotions experienced during game play and incorporate that feedback in the making of the final product. Basically, facial expression recognition is etremely helpful in behavioral testing, where understanding the genuine feedback of your customer is essential.

# Model

I used transfer learning with the Famous EfficientNetB2 as the backbone

![EfficientNetB2](https://user-images.githubusercontent.com/62629426/221707070-6b0fdb53-63d7-41cb-b55d-b436bc7c3797.png)

As we can see that EfficientNet achieves the highest accuracy, whilst having the least parameters out of most modern CNN architectures.

<img width="500" alt="models" src="https://user-images.githubusercontent.com/62629426/221452049-30538255-0bc4-4d62-84c1-19cf5608a84d.png">

EfficientNet are also scaled in a more principled way, than other models, basically, everything is gradually increasing.

![image](https://user-images.githubusercontent.com/62629426/221708947-8fa7e019-6f04-4bfb-a79a-e3e1b93bd681.png)
*(a) is a baseline network example; (b)-(d) are conventional scaling that only increases one dimension of network width, depth, or resolution. (e) is our proposed compound scaling method that uniformly scales all three dimensions with a fixed ratio.*

To get more information about the EfficientNet architecture check this out (https://towardsdatascience.com/complete-architectural-details-of-all-efficientnet-models-5fd5b736142)

### Libraries: 
- [Tensorflow - Keras](https://www.tensorflow.org/api_docs/python/tf/keras)
- [tensorflow](https://www.tensorflow.org/)
- [Pathlib](https://docs.python.org/3/library/pathlib.html)
- [Matplotlib](https://matplotlib.org/)
- [Numpy](http://numpy.org/)

### Results:
0: `Anger`, 1: `Disgust`, 2: `Fear`, 3: `Happiness`, 4: `Neutral`, 5: `Sadness`, 6: `Surprise`

### Accuracy:
- accuracy: 2.4218 
- Loss: 0.5043 
- Val_accuracy: 0.4563
- Val_loss: 1.3835
