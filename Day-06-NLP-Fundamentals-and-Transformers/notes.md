# Day 06 Notes

## NLP Pipeline

Raw Text

↓

Sentence Tokenization

↓

Word Tokenization

↓

Stopword Removal

↓

Stemming / Lemmatization

↓

Feature Extraction

↓

Model Building

---

## Tokenization

Sentence Tokenization

Splits text into sentences.

Word Tokenization

Splits sentences into words.

---

## Stemming

Produces root words.

Example

Running → Run

Studies → Studi

---

## Lemmatization

Produces meaningful root words.

Running → Run

Studies → Study

---

## Stopwords

Common words removed during preprocessing.

Examples

- is
- the
- and
- in

---

## Count Vectorizer

Converts text into word frequency vectors.

---

## TF-IDF

Assigns importance scores to words based on frequency across documents.

---

## N-Grams

- Unigram
- Bigram
- Trigram

Used for capturing context.

---

## POS Tagging

Assigns grammatical labels to words.

Examples

NN → Noun

VB → Verb

JJ → Adjective

---

## Named Entity Recognition

Detects entities such as

- Person
- Organization
- Location

---

## Transformers

Modern deep learning models for NLP.

Examples

- GPT-2
- BERT
- ChatGPT

---

## Hugging Face

Used the `pipeline()` API for text generation.

Controlled generation using:

- Temperature
- Top-K
- Top-P

Generated multiple responses using `num_return_sequences`.

---

## Key Learnings

✔ NLP preprocessing

✔ Feature extraction

✔ POS Tagging

✔ Named Entity Recognition

✔ Transformer models

✔ Hugging Face pipelines
