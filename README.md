# Facial-Expression-Recognition-with-keras
Build and train a convolutional neural network (CNN) in Keras from scratch to recognize facial expressions. The data consists of 48x48 pixel grayscale images of faces. The objective is to classify each face based on the emotion shown in the facial expression into one of seven categories (0=Angry, 1=Disgust, 2=Fear, 3=Happy, 4=Sad, 5=Surprise, 6=Neutral). You will use OpenCV to automatically detect faces in images and draw bounding boxes around them.
## Key concepts
- Develop a facial expression recognition model in Keras.
- Build and train a convolutional neural network (CNN).
- Deploy the trained model to a web interface with Flask.
- Apply the model to real-time video streams and image data.
## Project structure
###### **Task 1: Introduction and Overview**
- Introduction to the data and and overview of the project.
- Import essential modules and helper functions from NumPy, Matplotlib, and Keras.
###### **Task 2: Explore the Dataset**
- Display some images from every expression type in the Emotion FER dataset.
- Check for class imbalance problems in the training data.
###### Task 3: Generate Training and Validation Batches
- Generate batches of tensor image data with real-time data augmentation.
- Specify paths to training and validation image directories and generates batches of augmented data.
###### Task 4: Create a Convolutional Neural Network (CNN) Model
- Design a convolutional neural network with 4 convolution layers and 2 fully connected layers to predict 7 types of facial expressions.
- Use Adam as the optimizer, categorical crossentropy as the loss function, and accuracy as the evaluation metric.
###### Task 5: Train and Evaluate Model
- Train the CNN by invoking the model.fit() method.
- Use ModelCheckpoint() to save the weights associated with the higher validation accuracy.
- Observe live training loss and accuracy plots in Jupyter Notebook for Keras.
###### Task 6: Save and Serialize Model as JSON String
- Sometimes, you are only interested in the architecture of the model, and you don't need to save the weight values or the optimizer.
- Use to_json(), which uses a JSON string, to store the model architecture.
###### Task 7: Create a Flask App to Serve Predictions
- Use open-source code from "Video Streaming with Flask Example" to create a flask app to serve the model's prediction images directly to a web interface.
###### Task 8: Create a Class to Output Model Predictions
- Create a FacialExpressionModel class to load the model from the JSON file, load the trained weights into the model, and predict facial expressions.
###### Task 9: Design an HTML Template for the Flask App
- Design a basic template in HTML to create the layout for the Flask app.
###### Task 10: Use Model to Recognize Facial Expressions in Videos
- Run the main.py script to create the Flask app and serve the model's predictions to a web interface.
- Apply the model to saved videos on disk.
