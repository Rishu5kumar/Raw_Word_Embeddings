# Word Embeddings from Scratch using Python

This approach demonstrates the entire process of generating word embeddings using fundamental techniques, starting from data preparation to visualizing word vectors.

## Steps Involved

1. **Loading the Data**  
   The text data is loaded into the program in read mode. Each line is treated as a separate sentence for further processing.

2. **Preprocessing the Text**  
   - The newline characters (`\n`) at the end of each sentence are removed.
   - All text is converted to lowercase to ensure uniformity.
   
3. **Stopword Removal and Tokenization**  
   Common stopwords (e.g., "the", "is", "in") are filtered out, as they do not add meaningful information. The remaining words are tokenized, converting the text into a list of individual words.

4. **Creating Bigrams**  
   I generate bigrams (pairs of consecutive words) to capture relationships between words that commonly occur together. This step helps improve the context learning of the model.

5. **Generating a Unique Vocabulary**  
   A list of unique words (vocabulary) is created from the tokenized text. This vocabulary serves as the foundation for further embedding steps.

6. **Building a Word Dictionary**  
   Each unique word is assigned an index to create a word-to-index dictionary, where each word is represented by its corresponding unique integer.

7. **Performing One-Hot Encoding**  
   Using the word dictionary, one-hot encoding is applied. This represents each word as a sparse vector with a '1' at the index of the word, and '0's elsewhere, creating a numerical representation for each word in the vocabulary.

8. **Neural Network for Word Embedding**  
   A simple neural network model is built to learn word embeddings. The input layer accepts one-hot encoded words, and the output layer provides dense, low-dimensional word vectors that capture the semantic relationships between words.

9. **Visualization of Word Embeddings**  
   Finally, the learned word embeddings are visualized using matplotlib, allowing us to observe how semantically similar words are grouped closer together in the embedding space.

--- 
