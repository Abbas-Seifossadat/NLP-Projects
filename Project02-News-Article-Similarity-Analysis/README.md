# News Article Similarity Analysis using NLP

## Project Objective
Analyze semantic similarity between news articles using NLP techniques (GloVe embeddings, PCA, and K-Means clustering) to uncover hidden thematic patterns.

---

## Key Features
- **Text Vectorization**: Converts articles to 100D vectors using pre-trained GloVe embeddings.
- **Dimensionality Reduction**: Projects vectors to 2D space with PCA for visualization.
- **Clustering**: Groups articles into thematic clusters using K-Means.
- **Interpretation**: Validates clusters with word clouds and top-term analysis.
- **Interactive Tools**: Plotly-based Elbow Method and cluster visualization.

---

## Dataset
- **Source**: [HuffPost News Articles](https://github.com/mage-ai/datasets/blob/master/news_articles.csv) (55K+ articles).
- **Columns**: `topic`, `headline`, `description`, `author`, etc.
- **Sample Themes**: Politics, Wellness, Entertainment.

---

## Technical Approach
1. **Preprocessing**  
   Lowercasing, punctuation removal, stopword filtering.
2. **Embeddings**  
   GloVe (`glove.6B.100d.txt`) for word-to-vector mapping.
3. **Dimensionality Reduction**  
   PCA (24% variance captured in 2D).
4. **Clustering**  
   K-Means (`k=4` validated by Elbow Method).
5. **Validation**  
   Word clouds and top-50 term analysis per cluster.

---

## Results
### Cluster Themes Identified:
1. **U.S. Domestic Politics** (`clinton`, `gop`, `obama`)  
2. **Wellness & Public Health** (`health`, `cancer`, `sleep`)  
3. **Healthcare Policy** (`u.s.`, `republicans`, `care`)  
4. **Entertainment** (`film`, `star`, `awards`)  

![PCA Clusters](download_(2).png)  
*PCA-reduced article clusters (k=4) with partial overlap. Colors represent clusters, and red "X" marks denote centroids.*
