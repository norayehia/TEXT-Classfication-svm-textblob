# TEXT-Classfication-svm-textblob
In the text classification task on drug reviews data from uci using SVM (Support Vector Machine) and TF-IDF (Term Frequency-Inverse Document Frequency) with max features and n-gram range, several steps were involved to achieve effective results.

Firstly, the raw text data was preprocessed to ensure uniformity and cleanliness. This typically included tasks such as removing special characters, punctuation, and stopwords, as well as stemming or lemmatization to normalize the text.

Next, the data was vectorized using TF-IDF. TF-IDF assigns weights to words based on their frequency in the document and their rarity in the corpus. This helps to emphasize words that are important for distinguishing between different classes while downplaying common terms.

To further refine the vectorization process, max features were specified. This parameter controls the maximum number of features (words) to be considered, which helps in reducing computational complexity and overfitting, especially with large datasets.

Additionally, n-gram range was determined to capture the contextual information in the text. N-grams are contiguous sequences of n items (words in this case) from a given text. By specifying the range (e.g., unigrams, bigrams, trigrams), the model can capture not only individual words but also combinations of words, thus improving the classification accuracy.

After vectorization, the data was split into training and testing sets to evaluate the performance of the model. The SVM algorithm was then trained on the training set using the vectorized data, learning the underlying patterns and relationships between features and labels.

Once trained, the model was evaluated on the testing set to assess its performance metrics such as accuracy, precision, recall, and F1-score. These metrics help in gauging how well the model generalizes to unseen data and its ability to correctly classify instances into their respective classes.

To label the data, TextBlob, a Python library for processing textual data, was utilized. TextBlob offers functionalities for various natural language processing tasks including part-of-speech tagging, noun phrase extraction, sentiment analysis, classification, translation, and more. By leveraging TextBlob, the data could be efficiently labeled, facilitating supervised learning with the SVM algorithm.

In summary, by following these steps and utilizing SVM with TF-IDF, max features, n-gram range, and TextBlob for labeling, an effective text classification system could be developed, capable of accurately categorizing text data into predefined classes or categories.
