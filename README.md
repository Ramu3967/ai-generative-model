# ai-generative-model

A generative language model project involves developing a model that can generate human-like text based on input prompts.
The goal of a generative language model is to be able to generate coherent and contextually appropriate sentences and paragraphs that can be used for a variety of applications, including language translation, content creation, and chatbot development.
Some popular examples of generative language models include OpenAI's GPT-3 and Google's BERT. We have created a comparable Generative AI-Language Model.

Data Collection and Pre-processing:
To develop this tool, we have used the Gutenberg Corpus dataset, which is widely used for natural language processing and machine learning tasks.
The overall effect of preprocessing the text is to convert all characters to lowercase and remove all newline and carriage return characters and any double spaces from the file. The resulting preprocessed text can be used for further analysis or processing.

To perform this, We have used this code where subsequences of a given length are generated from a given text, along with the next character that follows each subsequence.

Model Creation:
To develop the model, we used a neural network model using the Keras API from the TensorFlow library. The model is designed to be used for sequence-to-sequence prediction, where the input is a sequence of characters, and the output is a probability distribution over the possible next characters.
The model consists of two layers:
The first layer is an LSTM layer with 128 units.
The second layer is dense layer.

Model Compiling and Training:
The model compilation is done through Keras ‘compile()’ method. It configures the model for training by specifying the optimizer, loss function, and any metrics to be evaluated during training and testing.
The next step is to train the model using the Keras fit() method, which fits the model to the training data.
While training process, the data were divided into batches of 128 samples each, and we trained the model for 30 epochs.

Text Generation:
After the model’s training is complete, we proceed to utilize it for text generation.
This code generates text using the trained neural network model. The generated text starts with a string ‘seed,’ which is then used to predict the next characters in the sequence.
The for loop iterates 1000 times, generating a new character in each iteration. At the end of the loop, the entire text is ultimately produced.

Conclusion:
In conclusion, the Generative Language Model project has demonstrated the impressive capabilities of modern language models. Through their ability to analyze and learn from vast amounts of text data, these models can generate coherent and natural-sounding language. While there are still limitations and challenges to be addressed, such as bias and accuracy, the potential for these models to transform how we communicate and interact with language is truly exciting.
 As research and development in this field continue, we can expect to see even more impressive applications of generative language models in the future.


