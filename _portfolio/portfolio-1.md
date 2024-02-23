---
title: "NLDBQuery"
excerpt: "NLP Project to talk with your database 1<br/><img src='example.png'>"
collection: portfolio
---

# NLDBQuery

NLDBQuery is a project that utilizes Google's free Gemini API as the base for interacting with a database using plain English queries. The text model initially uses general queries and terms, as it has not been trained on the specific database schema. To improve the model's accuracy, few-shot learning is employed. Specific queries that the model finds difficult to answer are processed, and their embeddings are stored in Vector databases (ChromaDB). When a user provides a prompt, the model searches for similar queries using an example Selector based on the word embeddings, resulting in more accurate answers.

The input and output interface for the user is simple and designed using Streamlit. All the APIs for different models are accessed through Hugging Face, and pipelines and prompts are created using Langchain.

![Example Image](example.png)

## Frameworks and Tools Used
- Google's Gemini API
- Hugging Face (for accessing APIs)
- Langchain (for creating pipelines and prompts)
- ChromaDB (for storing query embeddings)
- Streamlit (for user interface)

## GitHub Repository
[GitHub Repository](https://github.com/OmSDeshmukh/NLDBQuery)

## License
This project is licensed under the MIT License. See the LICENSE file for details.

