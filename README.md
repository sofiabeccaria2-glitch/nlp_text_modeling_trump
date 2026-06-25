## nlp_text_modeling_trump
NLP topic modeling analysis of Trump's political speeches using BERTopic and transformer-based embeddings


# Project description
This project applies Natural Language Processing techniques to analyze a corpus of Donald Trump rally speeches (2019–2020). 

The objective is to identify recurring political narratives and understand how political language constructs and reinforces key frames such as immigration, economy, foreign policy, and electoral conflict.

Beyond topic extraction, the project focuses on the **structure of political discourse as a system of repeated narrative patterns.

# Research Objective

The goal is to use computational text analysis to investigate:

- How political narratives are constructed in campaign speeches 
- How themes are reinforced rather than diversified 
- How discourse varies across time and geography


# Dataset
The dataset consists of 35 Donald Trump rally speeches (2019–2020). 

Each speech is stored as a `.txt` file, with metadata (location, date, year) extracted from filenames.

# Methodology
The analysis pipeline includes:
- Text preprocessing (tokenization, cleaning, stopwords removal)
- Sentence-BERT embeddings for semantic representation
- Dimensionality reduction using UMAP
- Density-based clustering using HDBSCAN
- Topic modeling using BERTopic
- Topic representation using c-TF-IDF
- Chunking strategy to improve topic granularity

# Key Results
The analysis highlights that Trump’s speeches are characterized by:
- Strong repetition of core rhetorical frames across speeches
- A limited set of dominant narratives (immigration, economy, law and order, foreign policy)
- High semantic clustering around adversarial political communication
- Location- and time-dependent variation in emphasis of specific themes
Overall, the results suggest that political communication in rally speeches relies more on narrative reinforcement than thematic diversity.

# Visualization
The visual analysis allows exploration of:
- Topic distribution across time and geography
- Evolution of political narratives during the 2020 campaign
- Semantic similarity between political topics
- Hierarchical relationships between themes

# Key Visualization
Topic Structure
![Topics](figures/bertopic_intertopic_bar.html)

Topic Years Evolution
![Evolution](figures/bertopic_auto_yearsevolution.html)

Semantic Intertopic Map
![Map](figures/bertopic_intertopic_map.html)

Topic Similarity
![Similarity](figures/bertopic_similarity_heatmap.html)

# Project structure
Project structure:
data/ 		Raw speeches dataset  
notebooks/      Jupyter notebook analysis  
outputs/        	Generated results and visualizations  
README.md  Project documentation  


# Technological Stack
Technologies used:
- Python
- BERTopic
- Sentence Transformers (SBERT)
- UMAP
- HDBSCAN
- Scikit-learn
- Pandas
- NLTK
- Matplotlib / Plotly

 
# Topic Modelling Approach
- BERTopic pipeline
- SBERT embeddings
- UMAP + HDBSCAN
- c-TF-IDF representation

# Notes

This project combines NLP and computational social science approaches to study political discourse as structured narrative systems rather than isolated textual data.

# Reproducibility
Results are reproducible using fixed random seeds, although minor variations may occur due to stochastic components in UMAP and HDBSCAN.
