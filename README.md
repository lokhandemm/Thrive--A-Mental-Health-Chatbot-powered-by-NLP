# Thrive – Mental Health Chatbot 
  
**Thrive** is a hybrid AI chatbot designed to offer emotional support and promote mental wellness through accessible, 24/7 assistance. It combines retrieval-based and generative models to provide thoughtful, medically accurate responses to users experiencing stress, anxiety, or emotional discomfort.

---

## Project Overview

In today’s fast-paced world, mental health issues like stress, anxiety, and loneliness are common, especially among youth. Thrive aims to create a safe, judgment-free space where users can share how they feel and receive supportive responses or guidance—without waiting or fear of stigma.

This chatbot is not a replacement for therapy, but a first step towards mental health awareness and self-care.

---

## Objectives

- Detect signs of emotional distress in user messages  
- Provide helpful, accurate, and empathetic responses  
- Share crisis helpline information when necessary  
- Ensure easy and engaging interactions through a clean UI and responsive backend

---

## Problem Statement

1. Bridging mental health support gaps by providing immediate, AI-driven support  
2. Making emotional assistance accessible regardless of location or time  
3. Using NLP to personalize guidance and coping strategies

---

## Datasets Used

1. Mental Health FAQ (Kaggle)  
2. NLP-based Mental Health Conversations (Kaggle)  
3. Psychology Dataset Split (HuggingFace)

These datasets were merged into a final dataset (`Merged2.csv`) with:
- `Questions`: Common user queries  
- `Response`: Full professional replies  
- `Summarized_Response`: TF-IDF based summaries for faster retrieval

---

## System Architecture

The chatbot follows a three-step pipeline:

1. **Input Processing**  
   - Tokenization, stopword removal, lemmatization  
2. **Response Selection**  
   - Checks for crisis indicators and returns helpline info if found  
   - Matches query using TF-IDF + cosine similarity  
   - Falls back on Google Gemini LLM for unmatched queries  
3. **Response Generation**  
   - Ensures messages are empathetic, medically sound, and concise

---

## Technologies Used

- Python  
- TF-IDF Vectorization  
- Cosine Similarity  
- Google Gemini LLM (fallback model)  
- NLP preprocessing libraries  
- CSV-based dataset for retrieval

---

## Features

- 24/7 availability  
- Real-time responses  
- Clean and user-friendly interface  
- Crisis detection and redirection  
- Hybrid chatbot model (retrieval + generative)

---

## Future Scope

- Add multilingual support for wider reach  
- Integrate voice-based interaction  
- Implement mental health progress tracking (mood logs, visual trends)

---

## Team Members

- Maithili Lokhande  
- Dnyaneshwari Nagpure  
- Nikita Biswas  
- Sanvika Dakhale  

**Guided by:** Prof. Aarti Karandikar

---

## References

- Codecademy – Retrieval-Based Chatbot Cheatsheet  
  https://www.codecademy.com/learn/retrieval-based-chatbots/modules/retrieval-based-chatbots/cheatsheet  
- GenerativeAI.net – Generative AI Resources  
  https://generativeai.net/  
- Engati – Hybrid Chatbot Examples  
  https://www.engati.com/glossary/hybrid-chatbot-examples  
