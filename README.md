# Image Captioning with Sentiment Analysis

Hey there, NLP enthusiasts! 👋

If you're looking to dive into the world of image captioning and sentiment analysis models, this notebook is your perfect starting point. These models are two of the most popular tasks in NLP, and this notebook provides a solid foundation for your exploration.
Whether you're a seasoned pro or just starting out, I'm confident you'll find valuable insights and resources here. So grab a cup of coffee, get comfortable, and let's embark on this exciting journey together! ☕📚

I have implemented four different models for image captioning and sentiment analysis. These models consist of two phases: first, generating captions for input images, and then predicting the sentiment of each generated caption using pre-trained sentiment analysis models. All models have been trained and evaluated using the "Flickr8k" dataset.

1. The first architecture utilizes the `"microsoft/git-base"` model for image captioning and the `"cardiffnlp/twitter-roberta-base-sentiment-latest"` model for sentiment analysis from HuggingFace. This model undergoes a fine-tuning phase for the image captioning model on the Flickr8k dataset. The implementation is structured in multiple classes, adhering to an object-oriented approach.

2. The second architecture employs the `"nlpconnect/vit-gpt2-image-captioning"` model for image captioning (which yielded more accurate results compared to the previous model) and the same `"cardiffnlp/twitter-roberta-base-sentiment-latest"` model for sentiment analysis from HuggingFace. Similar to the first architecture, this model also undergoes a fine-tuning phase. To make a difference from the previous one, this one is implemented as a set of functions. The pre-trained model in this architecture generated more accurate captions than the previous one.

3. The third architecture is similar to the second one, but in this case, the image captioning model is not fine-tuned. Instead, the pre-trained models are directly used to predict captions and then detect their sentiments.

4. The fourth architecture involves implementing a pure image captioning model using Keras from scratch. However, I utilized the reference [link](https://keras.io/examples/vision/image_captioning/) (provided in the section header) and its code. For sentiment analysis, a different pre-trained `Bert` model from tfhub is utilized.

 I'm hoping this will give you a nice starting point for exploring multi-task learning with **Vision** and **NLP**.
 
P.S. Feel free to reach out if you have any questions or need a helping hand. 😊

