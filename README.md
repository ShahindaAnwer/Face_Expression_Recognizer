# Face Expression Recognizer

### Libraries: 
- [Tensorflow - Keras](https://www.tensorflow.org/api_docs/python/tf/keras)
- [tensorflow](https://www.tensorflow.org/)
- [Pathlib](https://docs.python.org/3/library/pathlib.html)
- [Matplotlib](https://matplotlib.org/)

### Data: https://www.dropbox.com/s/si11cws2pyho1bp/archive.zip

### Steps:
1. Import packages and load data
2. Getting directory path 
3. Split path to get label names
4. Encode Labels
5. Split and train data
6. Apply resizing and data augmentation
6. Create model, compile then fit

### Model:
I used transfer learning, with the help of the famous EfficientNetB2 model

### Results:
0: `Anger`, 1: `Disgust`, 2: `Fear`, 3: `Happiness`, 4: `Neutral`, 5: `Sadness`, 6: `Surprise`

### Accuracy:
- accuracy: 2.4218 
- Loss: 0.5043 
- Val_accuracy: 0.4563
- Val_loss: 1.3835
