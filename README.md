# Emotion_Detection
Facial expression Detection
Dataset is taken form kaggle: https://www.kaggle.com/ashishpatel26/fer2018?select=fer20131.csv

It has 35,000 images for training, testing and validation.

Details about the model:
The model has achieved 95% on training set and 66% on test set.

#How to use the model:
Just download the model and load the model using following commands.

model = tf.keras.models.load_model('./final_model.h5')

To predict:

resize the image the to (48, 48, 3) and use following command

model.predict([imgarr])

Note: face from the image should be cropped and is sent as input to the model.
