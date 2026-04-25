# FAISS Semantic Product Search

This project implements a semantic product search system using FAISS. Both products and user queries are represented as vector embeddings, allowing the system to retrieve results based on semantic similarity rather than exact keyword matching.

## Features

* Semantic search using vector embeddings
* Implementation of multiple FAISS indexing methods:

  * Flat L2
  * IVF Flat
  * HNSW
  * Product Quantization (PQ)
* Performance comparison based on execution time, memory usage, precision, and recall

## Key Findings

Flat L2 provides the highest accuracy but is slower. IVF improves search speed with some loss in accuracy. HNSW offers the best balance between speed and accuracy, making it suitable for real-time applications. Product Quantization significantly reduces memory usage but results in lower accuracy.

## Technologies Used

Python, FAISS, NumPy, Pandas, and Sentence Transformers

## Project Structure

notebook/ – Jupyter Notebook
data/ – Dataset
report/ – Project report
video/ – Demonstration video

## How to Run

Install the required dependencies:
pip install -r requirements.txt

Then open and run the notebook:
FAISS_Product_Search.ipynb

## Video Demonstration

You can watch the project demonstration here:
[Video Link](https://drive.google.com/file/d/1-wBnR7XF7q5mvvF2t8EFmdqAIvFByq6H/view?usp=sharing)

## Conclusion

Among the evaluated methods, HNSW provides the most effective trade-off between performance and accuracy, making it a strong choice for real-time semantic product search systems.

