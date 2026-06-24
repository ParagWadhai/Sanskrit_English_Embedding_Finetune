# 🕉️ Sanskrit-English Multilingual Embedding Retrieval

## Setup
```bash
pip install sentence-transformers datasets faiss-cpu accelerate
```

## Run
Open `notebooks/Sanskrit_English_Embedding_Finetune.ipynb` in Google Colab.
Set runtime to GPU (T4). Run all cells top to bottom.

## Dataset
`JDhruv14/Bhagavad-Gita_Dataset` — 701 Sanskrit+English aligned verse pairs.
Loaded automatically via HuggingFace datasets.

## Model
Base: `intfloat/multilingual-e5-small`  
Fine-tuned with MultipleNegativesRankingLoss on 1892 training pairs.
