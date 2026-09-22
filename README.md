# PageIndex-Guided Multimodal GraphRAG: Document Intelligence Beyond Text
## What it does
This project builds a multimodal Graph-RAG system that combines PageIndex-guided document structuring with knowledge graph reasoning. It is designed to improve retrieval and grounding over long, visually complex documents such as annual reports, where information is spread across text, layout, and figures. The system parses PDFs, extracts entities and relationships using large language models, builds a knowledge graph, and indexes content for retrieval so that question answering stays accurate even when the source document is long and mixed in format.

## Why I built it
This is my MSc dissertation project at the University of Salford, and it also forms the basis of a research paper I am preparing for submission to ICLR.

## Tools used
Python, Neo4j, OpenAI API, vector indexing, PDF parsing tools, and RAGAS for evaluation.

## How to run it
1. Clone this repository and install the dependencies listed in requirements.txt.

2. Add your OpenAI API or any other key to a .env file.

3. Place the PDF documents you want to process in the input folder.

4. Run the pipeline script to parse the PDFs, extract entities and relationships, and build the knowledge graph in Neo4j.

5. Run the evaluation script to test retrieval and answer quality using the RAGAS metrics.

## Results
The system was benchmarked against two baseline setups, a vector-only RAG system and a standard GraphRAG system, using RAGAS metrics including faithfulness, context precision, context recall, and answer relevancy. The dissertation achieved a distinction grade, and the full evaluation results and comparison tables are included in the project write-up.
