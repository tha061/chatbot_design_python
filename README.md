# chatbot_design_python

This repository provides source code to build a chatbot in python.
Chatbots play a pivotal role for businesses as they can effortlessly handle a barrage of customer queries and messages without any slowdown. 
They have single-handedly reduced the customer service workload for us by automating a majority of the process. 
They do this by utilizing techniques backed with Artificial Intelligence, Machine Learning, and Data Science.
Chatbots work by analyzing the input from the customer and replying with an appropriate mapped response. 
To train the chatbot, you can use Recurrent Neural Networks with the intents JSON dataset while the implementation can be handled using Python. 

# requires
pip install tensorflow keras pickle nltk

train_chatbot.py — In this file, we will build and train the deep learning model that can classify and identify what the user is asking to the bot.

gui_Chatbot.py — This file is where we will build a graphical user interface to chat with our trained chatbot.

intents.json — The intents file has all the data that we will use to train the model. It contains a collection of tags with their corresponding patterns and responses.

# how to run
python train_chatbot.py

Results:
words_th.pkl: The words.pkl pickle file contains all the unique words that are the vocabulary of our model.
classes_th.pkl: The pickle file can be used to store all the tag names to classify when we are predicting the message.

model file: chatbot_model_th.h5: This is a hierarchical data format file in which we have stored the weights and the architecture of our trained model.

# GUI of a chatbot
run: python gui_chatbot.py
Creating graphical user interface for our chatbot
In our GUI file, we will be using the Tkinter module to build the structure of the desktop application and then we will capture the user message and again perform some preprocessing before we input the message into our trained model.

The model will then predict the tag of the user’s message, and we will randomly select the response from the list of responses in our intents file.

#######
