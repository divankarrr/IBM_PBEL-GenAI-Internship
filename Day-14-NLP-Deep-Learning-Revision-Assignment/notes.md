# Day 14 Notes

# Q1. Tokenization

Tokenization splits text into smaller units called tokens.

Example:

Natural language processing is amazing

↓

["Natural", "language", "processing", "is", "amazing"]

Importance:

- First step of NLP
- Required before feature extraction

---

# Q2. Stemming

Stemming reduces words to their root form.

Examples

Running → run

Flying → fli

Advantages

- Faster preprocessing
- Reduces vocabulary size

Disadvantage

- Root words may not be meaningful.

---

# Q3. Lemmatization

Lemmatization converts words into meaningful dictionary words.

Examples

Running → Run

Cars → Car

Better → Good (depending on POS)

Advantages

- More accurate than stemming.
- Produces meaningful words.

---

# Q4. TF-IDF

TF = Term Frequency

IDF = Inverse Document Frequency

Purpose

Measures the importance of a word in a document relative to the entire corpus.

Advantages

- Reduces influence of common words.
- Highlights informative terms.

---

# Q5. Word2Vec

Word2Vec converts each word into a dense numerical vector.

Advantages

- Captures semantic similarity.
- Similar words have similar vector representations.

Applications

- Chatbots
- Translation
- Text Classification
- Recommendation Systems

---

# Q6. Simple RNN

Recurrent Neural Networks process sequential data by maintaining a hidden state.

Architecture

Input

↓

SimpleRNN

↓

Dense

↓

Output

Applications

- Time Series
- NLP
- Speech Recognition

---

# Q7. Bag of Words

Bag of Words converts text into a vector based on word frequency.

Characteristics

- Ignores word order.
- Simple and effective for basic NLP tasks.

---

# Q8. POS Tagging

Part-of-Speech Tagging assigns grammatical labels to words.

Examples

NN → Noun

VB → Verb

JJ → Adjective

RB → Adverb

Applications

- Information Extraction
- Machine Translation
- Grammar Checking

---

# Q9. Sequence Padding

Neural networks require input sequences of equal length.

Padding adds zeros to shorter sequences.

Types

- Pre Padding
- Post Padding

Advantages

- Uniform input size
- Easier batch processing

---

# Key Takeaways

✔ Tokenization is the first step in NLP.

✔ Stemming and Lemmatization reduce word variations.

✔ TF-IDF and Bag of Words convert text into numerical features.

✔ Word2Vec captures semantic relationships.

✔ RNNs are suitable for sequential data.

✔ POS Tagging identifies grammatical roles.

✔ Sequence padding standardizes variable-length text for neural networks.
