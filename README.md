Retrieval-Augmented Generation (RAG) for Indian Legal Applications

Overview

This project implements a Retrieval-Augmented Generation (RAG) pipeline to answer legal questions based on Indian law. By combining semantic retrieval and natural language generation (NLG), the system provides accurate, context-aware responses using datasets from the Indian Constitution, Code of Criminal Procedure (CrPC), and Indian Penal Code (IPC).

Features

Data Preprocessing: Standardizes and cleans datasets by removing duplicates and inconsistencies.
Semantic Search: Uses FAISS for efficient similarity-based retrieval of relevant legal texts.
Answer Generation: Employs the open-source Flan-T5-base model for generating human-like responses.
Embedding Creation: Leverages all-mpnet-base-v2 for creating dense text embeddings.

Datasets

The project uses three JSON datasets covering key aspects of Indian law:

Indian Constitution QA: Fundamental rights, governance, and duties.
CrPC QA: Procedural aspects like arrests, bail, and trials.
IPC QA: Substantive criminal law, including offenses and punishments.
Each dataset contains questions and answers, enabling semantic retrieval and contextualized response generation.

Requirements

Software

Python 3.8 or higher
Libraries
Transformers: For pre-trained models like Flan-T5-base.
FAISS-CPU: For efficient similarity search.
Sentence-Transformers: For embedding generation.
Torch: For handling deep learning computations.
Install all libraries using the following command:


Key Components

1. Retrieval-Augmented Generation (RAG)
RAG combines retrieval of relevant knowledge with generation to produce grounded and context-aware answers.

2. FAISS (Facebook AI Similarity Search)
Used for fast similarity searches in the embedding space.
Enables efficient retrieval of the top-k relevant question-answer pairs for any user query.
3. Embedding Model
Model: all-mpnet-base-v2 (Sentence-BERT variant).
Purpose: Creates numerical representations of text for semantic similarity.
4. Natural Language Generation (NLG)
Model: Flan-T5-base (Open Source).
Purpose: Generates fluent, human-like answers using the retrieved legal context.

Acknowledgments

Hugging Face: For providing open-source models like Flan-T5-base and all-mpnet-base-v2.
FAISS: For efficient similarity search.
Indian Law: For the publicly available datasets on Kaggle.
