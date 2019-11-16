# Varela Leaks using GPT-2

This is a test only of 'text and conversational generation' using GPT-2 Model of OpenAI.  My test demonstrates only that you could generate text using AI i am not involved in any political activity.

I used models 127M and 355M to emulate a conversation between to people.

The idea is just only to experiment and test the capabilities of the GPT-2 Model, the same idea could be applicable to a database of medical information and you could generate a chatbot model for doctor-patient consultancy.

There are 3 models of OpenAI GPT-2 but i tested 2 of 3.  I encourage you th [read the paper of OpenAI abut GPT-2](https://openai.com/blog/gpt-2-1-5b-release/) if you want to know more.


# How was the performance?

As you will see the GPT-2 did not do a great job in Spanish, that's because all the training data was set to be in English.  You could upload anything related to poetry, lyrics or a database of conversation and it will generate good conversations/styles of text representation.


# How to Use It

### For the 127M Model and 355M models are the same steps

- Download this notebook
- Upload to your google colab account
- Execute up to the cell ' from google.colab import files '
- Upload a file of text (i used as you see only the _chat.txt file of seguridad.zip)
- Up to the line !python gpt-2/src/train.py --model_name ... . You could tweak the hyperparameters before go ahead
- Training will starte after you execute this line
- You simply stop when you consider the training is enought by CTRL+C or the stop button
- On the lines below, near !cp checkpoint/run1/model-xxx, you must check the checkpoints folder and see in whic trainig you stoped (in that time I stoped, i.e., in the 355M to 3028 epochs)
- After changing that you can go ahead, there are two ways of GPT-2 to test
    - Unconditional sample generation:  This will generate samples indefinitely and you could tweak some parameters
    - Interactivo unconditional sample generation:  This will prompt you a input box and you could chat with the model.