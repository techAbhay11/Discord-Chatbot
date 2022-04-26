Why we built this:

We wanted to create AI that could talk like a fictional character. Discord has become a very popular community messaging platform. It uses bots that can be programmed to reply to any message. So we thought of building a Discord Chat Bot that could message like a fictional character. It will help us to understand the Generative Pre-trained Transfomer Model which is a very popular language model.


Flow explanation:

We decided to make a chat bot based on the character of Harry Potter. We gathered the required dataset from Kaggle. We found a movie script dataset for the first Harry Potter movie. The dataset was a CSV file consisting of two columns, character name and dialogue line.
We trained the model in Google Colab. Google Colab was used because they provide GPU on the cloud as the model can be too heavy to train on a local machine. The Jupyter Notebook is connected to our Google Drive to access and store files. Instead of training from scratch, we will load Microsoft's pre-trained GPT, DialoGPT-medium, and fine-tune it using our dataset. We trained the model for 12 epochs. After training the model, it is stored in our Google Drive.
Then we deployed the model to HuggingFace. HuggingFace provides a free API for us to query the model. The model was pushed via git from the Google Drive folder.
We built a discord bot using Javascript that could send API requests to our hosted model. We created a Discord application and set the permissions for the bot in our Discord server.
We used Replit to host the backend of the bot. NodeJS server was used to deploy the bot functions.
