
### **Sentiment Analysis of Book Reviews using NLP and Transformer Models**

### **Objective:**
The goal of this project is to perform sentiment analysis on product reviews using natural language processing (NLP) techniques. Multiple models are utilized, including traditional lexicon-based methods like VADER (Valence Aware Dictionary and sEntiment Reasoner) and state-of-the-art pre-trained transformer models such as RoBERTa, to analyze sentiment and compare their performance.

### **Approach:**

1. **Dataset:**
   - The dataset used contains Amazon fine food reviews, including product reviews with corresponding ratings (scores).

2. **Exploratory Data Analysis (EDA):**
   - Basic analysis of the review data was conducted using visualizations, such as plotting the distribution of review scores.
   - Data was pre-processed and limited to a subset of 500 reviews for faster analysis.

3. **Text Tokenization and POS Tagging:**
   - NLTK (Natural Language Toolkit) was used to tokenize the text of reviews and tag the tokens with part-of-speech (POS) labels.
   - Named entity recognition (NER) was performed to extract entities from the reviews.

4. **Sentiment Analysis with VADER:**
   - **VADER Sentiment Analysis** was used to analyze the sentiment of the reviews. It assigns a polarity score indicating positive, negative, or neutral sentiment.
   - VADER was applied to each review, and sentiment scores were captured.

5. **Sentiment Analysis with RoBERTa:**
   - A pre-trained **RoBERTa model** (an optimized version of BERT) was used to analyze the sentiment of the reviews.
   - RoBERTa produces sentiment probabilities for negative, neutral, and positive sentiments.
   - This model was applied to the reviews, and its results were compared with those from VADER.

6. **Combining Results:**
   - Sentiment analysis results from both VADER and RoBERTa were merged into a single dataset, combining both sets of features.
   - Visualizations were generated to compare sentiment scores across different review scores.

7. **Model Comparison:**
   - The performance of both models (VADER and RoBERTa) was compared by visualizing sentiment scores in a pairplot, with review scores as the hue.
   - This comparison illustrated how the models performed on both positive and negative reviews.

8. **Review Examples:**
   - Example reviews with extreme sentiments (positive and negative) were extracted and analyzed to demonstrate differences in sentiment predictions by VADER and RoBERTa.

9. **Transformers Pipeline:**
   - The **Transformers pipeline** was used for sentiment analysis as a quick and easy way to perform sentiment analysis using pre-trained transformer models.
   - This pipeline was tested on various sample texts and provided robust predictions.

### **Results:**
- The project demonstrated how both traditional lexicon-based sentiment analysis (VADER) and modern transformer-based models (RoBERTa) can be used to extract sentiment from text.
- RoBERTa generally provided more nuanced and accurate sentiment analysis for complex sentences.
- Visualizations showed that transformer models outperform simple lexicon-based models in understanding sentiment in product reviews.

### **Conclusion:**
This project highlights the power of combining classic NLP methods with modern transformer models to analyze and understand sentiment in textual data. By applying these techniques to review datasets, valuable insights can be extracted from product feedback. This can be particularly beneficial for businesses looking to analyze customer feedback, detect trends, and improve customer service.

