# Day 09 Notes

## What is NLP?

Natural Language Processing (NLP) is a branch of Artificial Intelligence that enables computers to understand, process, analyze, and generate human language.

Examples:

- Chatbots
- Machine Translation
- Speech Recognition
- Sentiment Analysis
- Text Summarization
- Spam Detection

---

# NLP Pipeline

Raw Text

↓

Sentence Tokenization

↓

Word Tokenization

↓

Stemming

↓

Lemmatization

↓

Stop Word Removal

↓

Dependency Parsing

↓

Feature Extraction

↓

POS Tagging

↓

Named Entity Recognition

↓

Chunking

↓

Machine Learning Model

---

## Tokenization

Tokenization converts text into smaller meaningful units called tokens.

Types of Tokenization:

### Sentence Tokenization

Splits a paragraph into individual sentences.

Example:

Today is Sunday. I am learning NLP.

↓

["Today is Sunday.", "I am learning NLP."]

---

### Word Tokenization

Splits sentences into words.

Example:

Machine Learning is amazing.

↓

["Machine","Learning","is","amazing"]

---

### Character Tokenization

Splits text into individual characters.

Example:

AI

↓

A

I

---

### Subword Tokenization

Splits words into smaller meaningful units.

Useful for:

- BERT
- GPT
- Transformer Models

---

## Importance of Tokenization

- Converts text into processable format.
- Helps feature extraction.
- Improves language modelling.
- Supports text search and retrieval.
- Forms the basis for most NLP tasks.

---

## Stemming

Reduces words to their root form.

Examples:

Playing → Play

Running → Run

Studies → Studi

Advantages:

- Faster

Disadvantages:

- Root word may not be meaningful.

---

## Lemmatization

Produces meaningful dictionary words.

Examples:

Running → Run

Studies → Study

Advantages:

- More accurate than stemming.

---

## Stop Words

Frequently occurring words that usually add little meaning.

Examples:

- is
- the
- and
- a

Removing stop words reduces noise in text data.

---

## Dependency Parsing

Shows grammatical relationships between words in a sentence.

Helps understand sentence structure.

---

## Count Vectorizer

Converts text into numerical vectors using word frequencies.

Used as a feature extraction technique before training ML models.

---

## POS Tagging

Assigns grammatical labels to words.

Examples:

NN → Noun

VB → Verb

JJ → Adjective

RB → Adverb

---

## Named Entity Recognition (NER)

Identifies important entities from text.

Examples:

Person

Organization

Location

Date

Money

---

## Chunking

Groups related words together into meaningful phrases.

Example:

"The beautiful red car"

↓

[Noun Phrase]

---

# Popular NLP Libraries

### NLTK

Complete toolkit for NLP learning.

### SpaCy

Industrial-strength NLP library.

### TextBlob

Easy-to-use NLP library.

### Gensim

Topic Modelling

Word Embeddings

### Scikit-learn

Feature extraction

Machine Learning

---

# Key Takeaways

✔ NLP enables computers to understand human language.

✔ Tokenization is the first step in NLP preprocessing.

✔ Lemmatization produces meaningful root words.

✔ Count Vectorizer converts text into numerical features.

✔ POS Tagging and NER help computers understand sentence meaning.

✔ SpaCy and NLTK are among the most widely used NLP libraries.

✔ A strong understanding of preprocessing is essential before building advanced NLP or Generative AI applications.
