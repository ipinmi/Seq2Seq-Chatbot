# Seq2Seq-Chatbot
A Conversational chatbot built using LSTM &amp; Seq2Seq Architectures, and Machine Translation (Multi30K) dataset.

## Project Overview
1. Build your Vocabulary & create the Word Embeddings
    - Built the vocabulary from the Multi30K dataset using the TorchText Fields module and Spacy Tokenizers for Deutsch and English.
    - Train the word embeddings using the Gensim Word2Vec model and Use Gensim to extract the word embeddings from one of its corpus'.
    - Data splits using the BucketIterator module.
    - Used NLTK and Gensim to create a function to clean the text and look up the index of a word's embeddings.  
<br>

2. Create the Encoder Unit
    - A Seq2Seq architecture consists of an encoder and a decoder unit.  
    - Created an encoder with an LSTM unit.  
<br>

3. Create the Decoder Unit
    - The second step of the architecture is to create a decoder using a second LSTM unit.  
<br>


4. Combine them into a Seq2Seq Architecture
    - Combining the encoder and decoder units into a working model.
    - The Seq2Seq2 model must be able to instantiate the encoder and decoder. Then, it will accept the inputs for these units and manage their interaction to get an output using the forward pass function.  
<br>


5. Training, Evaluation and Hyper-parameter Tuning
    - Training the model using the Multi30K dataset using a Pytorch training loop.
    - Tuning the hyper-parameters of the model to improve the performance of the model.
    - The hyper-parameters that were tuned were the number of layers, the number of hidden units, the learning rate, and the batch size.  
<br>  


## Project Timeline
1. **Prepare data (~2 hours)**
Build your vocabulary from a corpus of language data. The Vocabulary object is described in Lesson Six: Seq2Seq. 
<br>  


2. **Build Model (~4 hours)**
Build your Encoder, Decoder, and larger Sequence to Sequence pattern in PyTorch. This pattern is described in Lesson Six: Seq2Seq. 
<br>  


3. **Train Model (~3 hours)**
Write your training procedure and divide your dataset into train/test/validation splits. Then, train your network and plot your evaluation metrics. Save your model after it reaches a satisfactory level of accuracy. 
<br>  


4. **Evaluate & Interact w/ Model (~1 hour)**
Write a script to interact with your network at the command line. 
<br>  

