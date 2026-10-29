# Lab 6: NLP Fundamentals - Tokenization, Embeddings and Text Chunking

**Student:** Shahzad Sadiq
**Roll Number:** 387
**Subject:** Artificial Intelligence Lab
**Teacher:** Rasikh Ali
**Section:** BSA 3D

## Setup
1. `python -m venv .venv`
2. Activate it (Windows: `.venv\Scripts\Activate.ps1`)
3. `python -m pip install numpy scikit-learn sentence-transformers`
4. `python -m pip freeze > requirements.txt`

## Task 1 (Beginner)
- `python task1_tokens.py`
- `python task1_chatbot_check.py`
- `python guided_chatbot.py`

## Task 2 (Intermediate)
- `python task2_chunks.py`
- `python guided_embeddings.py`
- `python task2_semantic.py`
- `python guided_suggestions.py`

## Task 3 (Advanced)
- `python create_dataset.py` (corpus.json and queries.json are already created, delete them first to run it again)
- `python task3_retrieval.py > output_task3.txt` (also creates retrieval_log.csv)
- `python document_chatbot.py`

## Other files
- `lab6_search.py` shared retriever
- `docs_data.py` the five synthetic documents
- `scenario1_handbook.py` to `scenario5_equipment.py` scenario scripts
- `guided_tokens.py`, `guided_chunks.py`, `guided_limits.py`, `guided_metrics.py` guided examples

All documents are synthetic teaching data written for this lab. Model: sentence-transformers/all-MiniLM-L6-v2 (CPU). Code is adapted from the lab manual by Rasikh Ali.
