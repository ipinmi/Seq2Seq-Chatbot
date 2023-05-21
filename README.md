# Seq2Seq-Chatbot
A Conversational chatbot built for machine translation using LSTM &amp; Seq2Seq Architectures, and Machine Translation (Multi30K) dataset.

## Project Overview
1. Build your Vocabulary & create the Word Embeddings
    - Built the vocabulary from the Multi30K dataset using the TorchText Fields module and Spacy Tokenizers for Deutsch and English.
    - Train the word embeddings using the Gensim Word2Vec model and Use Gensim to extract the word embeddings from one of its corpus'.
    - Data splits using the BucketIterator module.
    - Used NLTK and Gensim to create a function to clean the text and look up the index of a word's embeddings.  
<br>

2. Create the Encoder and Decoder Units
    - A Seq2Seq architecture consists of an encoder and a decoder LSTM units.  
    - Created an encoder with an LSTM unit.  
    - The second step of the architecture is to create a decoder using a second LSTM unit.
<br>


3. Combine them into a Seq2Seq Architecture
    - Combining the encoder and decoder units into a working model.
    - The Seq2Seq model must be able to instantiate the encoder and decoder. Then, it will accept the inputs for these units and manage their interaction to get an output using the forward pass function.  
    - The model architecture was two-layers deep, using an embedding sizes of 300 and dropout of 0.5 for both the encoder and decoder with a hidden size of 1024. 
<br>


4. Training, Evaluation and Hyper-parameter Tuning
    - Training the model using the Multi30K dataset using a Pytorch training loop.
    - Tuning the hyper-parameters of the model to improve the performance of the model.
    - The hyper-parameters that were tuned were the number of layers, the number of hidden units, the learning rate, and the batch size.  
    - The model achieved a train loss of 0.763 and a test loss of 3.646
<br>  


