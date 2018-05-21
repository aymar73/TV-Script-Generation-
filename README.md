# TV-Script-Generation-
Used RNN, LSTM, WORD EMBEDDING


Unit Testing is a reliable method to test the code of all the modules independently before integration. That way we can be more or less certain that our project is free from error at any point. 
This paradigm of developing code for unit testing along with a project code enable clean, confident and fast development. We can read up more on this if we wish here(http://docs.python-guide.org/en/latest/writing/tests/).

It's also important to remember that unit testing can't catch all the bugs in a code. So the code may have bugs even though all tests pass.

# Getting the project files
The project files can be found in the public GitHub repo, in the tv-script-generation folder. You can download the files from there, but it's better to clone the repository to computer

git clone https://github.com/udacity/deep-learning.git

This way you can stay up to date with any changes made by pulling the changes to your local repository with git pull.

# The function get_embed applies embedding to input_data and returns embedded sequence.

Another way to do this concisely would be:

return tf.contrib.layers.embed_sequence(input_data, vocab_size, embed_dim)
Embeddings are particularly important because they map the words to a numerical representation for the neural network to process.

Word2Vec was a landmark paper on embedding representations. The famous example King - Man + Woman = Queen ! This is a terrific explanation about the mechanics behind them (http://mccormickml.com/2016/04/19/word2vec-tutorial-the-skip-gram-model/)

Tensorflow provides a variety of other methods to construct an RNN (https://www.tensorflow.org/api_guides/python/nn#Recurrent_Neural_Networks).

Google is doing some very exciting work with RNNs to generate art and even music. Check it out here (https://magenta.tensorflow.org/)
