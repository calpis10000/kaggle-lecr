# kaggle-lecr
This repository is prv39th/pub39th training codes of  [Learning Equality - Curriculum Recommendations](https://www.kaggle.com/competitions/learning-equality-curriculum-recommendations) competition.
- The discription of this solution is available [here](https://www.kaggle.com/competitions/learning-equality-curriculum-recommendations/discussion/394896).  
- The inference notebook is available [here](https://www.kaggle.com/code/calpis10000/lecr-calpis-exp037).  

# Training Procedures
### 1. Create text features and Retriever dataset
- Create content feature: [[LECR] Common-Create content texts.ipynb](https://github.com/calpis10000/kaggle-lecr/blob/main/00_Common/%5BLECR%5D%20Common-Create%20content%20texts.ipynb)
- Create topics contexts for Retriever: [[LECR] Common-create contexts v3.ipynb](https://github.com/calpis10000/kaggle-lecr/blob/main/00_Common/%5BLECR%5D%20Common-create%20contexts%20v3.ipynb)
- Create topics contexts for Reranker: [[LECR] Common-create contexts v4-for-reranker.ipynb](https://github.com/calpis10000/kaggle-lecr/blob/main/00_Common/%5BLECR%5D%20Common-create%20contexts%20v4-for-reranker.ipynb)
- Create Retriever dataset: [[LECR] Retriever 037-01 Topics dataset.ipynb](https://github.com/calpis10000/kaggle-lecr/blob/main/01_Retriever/%5BLECR%5D%20Retriever%20037-01%20Topics%20dataset.ipynb)

### 2. Train Retriever
- Train Retriever: [[LECR] Retriever 054-03 Train.ipynb](https://github.com/calpis10000/kaggle-lecr/blob/main/01_Retriever/%5BLECR%5D%20Retriever%20054-03%20Train.ipynb)

### 3. Create Reranker dataset
- Create Reranker dataset (on Kaggle notebook): [[LECR] Retriever 054 Reranker dataset-100](https://www.kaggle.com/code/calpis10000/lecr-retriever-054-reranker-dataset-100)

### 4. Train Reranker
- Train Reranker: [[LECR] Reranker 078-03 Train.ipynb](https://github.com/calpis10000/kaggle-lecr/blob/main/02_Reranker/%5BLECR%5D%20Reranker%20078-03%20Train.ipynb)

# Environment
- Dataset creation was run on Google Colab or Kaggle notebook.
- Retriever training was run on Google Colab (GPU: A100).
- Reranker training was run on GCP with [Kaggle docker-python image](https://github.com/Kaggle/docker-python) (GPU: A100).
