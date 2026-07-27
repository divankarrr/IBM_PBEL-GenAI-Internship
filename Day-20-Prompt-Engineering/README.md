# Day 20 – Prompt Engineering

📅 **Date:** 10 July 2026

---

# 🎯 Objective

Learn the fundamentals of Prompt Engineering, understand how prompts influence Large Language Models (LLMs), explore different prompting techniques, and gain practical exposure to IBM Granite and watsonx for enterprise Generative AI applications.

---

# 📚 Topics Covered

## Introduction to Prompt Engineering

Prompt Engineering is the process of designing clear and structured prompts to obtain accurate, relevant, and reliable outputs from Large Language Models.

---

## Why Prompt Engineering?

Better prompts lead to:

- More accurate answers
- Better reasoning
- Reduced hallucinations
- Structured outputs
- Higher productivity

---

## Anatomy of a Good Prompt

A good prompt contains:

- Role
- Task
- Context
- Constraints
- Output Format

Example:

Act as a Data Scientist. Explain Decision Trees to a beginner using one real-world example in less than 150 words.

---

## Good Prompt vs Bad Prompt

### Bad Prompt

Tell me about AI.

Output:

- Generic
- Unstructured
- Ambiguous

### Good Prompt

Act as a professor.

Explain CNN, RNN and Transformers.

Give one example each.

Maximum 200 words.

Output:

- Focused
- Structured
- High Quality

---

# Prompt Engineering Techniques

## Zero-Shot Prompting

The model receives only the instruction without examples.

Example

Classify this review as Positive or Negative.

---

## Few-Shot Prompting

Provide a few examples before asking the actual question.

Example

Positive → I loved this movie.

Negative → This was terrible.

Now classify:

The movie was average.

---

## Role Prompting

Assign an identity or expertise to the model.

Examples

- Act as a Software Engineer.
- Act as a Career Mentor.
- Act as a Professor.
- Act as a Cybersecurity Expert.

---

## Chain-of-Thought Prompting

Encourages the model to reason through the problem step by step.

Example

Think step by step before solving the problem.

---

## Output Formatting

Specify the required output structure.

Examples

- JSON
- Markdown
- Table
- Bullet List

---

# Foundation Models

Learned how foundation models are adapted to multiple downstream tasks through prompting and fine-tuning.

Examples

- GPT
- Gemini
- LLaMA
- IBM Granite
- Falcon

---

# IBM Granite

Enterprise foundation model developed by IBM.

Key Features

- Decoder-only Transformer
- Enterprise-ready
- Governance
- Auditability
- Transparency

Variants

- Granite Base
- Granite Instruct
- Granite Chat

---

# IBM watsonx Platform

Three core products:

## watsonx.ai

- Prompt Lab
- Foundation Models
- Fine Tuning
- AI Development

---

## watsonx.data

- Enterprise Data
- Retrieval-Augmented Generation (RAG)
- Data Governance

---

## watsonx.governance

- Bias Monitoring
- Explainability
- AI Governance
- Compliance

---

# Hands-on Activities

- Sentiment Classification using Zero-shot Prompting
- Good vs Bad Prompt Comparison
- Code Generation using Granite
- Grounded Question Answering (RAG)
- AI Language Tutor

---

# Practical Learning

- Designed effective prompts.
- Compared prompt engineering techniques.
- Learned enterprise AI workflow.
- Explored IBM Granite models.
- Understood watsonx ecosystem.

---

# Files

- Prompt_Engineering.ipynb
- README.md
- notes.md
- requirements.txt

---

# Learning Outcomes

After completing this session, I can:

- Design effective prompts.
- Apply Zero-shot and Few-shot prompting.
- Use Role Prompting.
- Apply Chain-of-Thought prompting.
- Control LLM output formatting.
- Understand IBM Granite models.
- Explain IBM watsonx components.
- Build enterprise-ready prompting workflows.

---

# Outcome

Built a strong understanding of Prompt Engineering techniques and enterprise Generative AI workflows using IBM Granite and watsonx. Learned how carefully designed prompts significantly improve the quality, accuracy, and usability of LLM outputs.
