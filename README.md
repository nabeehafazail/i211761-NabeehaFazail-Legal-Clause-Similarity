Legal Clause Similarity
This repo contains my assignment for A2-CS452 on detecting semantic similarity between legal clauses.

Files
- `i211761-NabeehaFazail-Legal-Clause-Similarity.ipynb` → Jupyter Notebook with preprocessing, BiLSTM and Attention models, training and evaluation
- `i211761_NabeehaFazail_A2-CS452.pdf` → Report PDF

Dataset
- Kaggle Legal Clause Dataset: https://www.kaggle.com/datasets/bahushruth/legalclausedataset
- Contains clause text and category
- Train/test split: 80/20

Models
1. BiLSTM
   - Embedding → BiLSTM → Dense → Dropout → Sigmoid
2. Attention Encoder
   - Embedding → LSTM → Attention → Dense → Dropout → Sigmoid

Results

| Model | Accuracy | Precision | Recall | F1 | ROC-AUC |
|-------|----------|-----------|--------|----|---------|
| BiLSTM | 0.9876 | 0.9800 | 0.9956 | 0.9877 | 0.9963 |
| Attention | 0.9513 | 0.9189 | 0.9899 | 0.9531 | 0.9688 |

How to Run
1. Install dependencies: `pip install tensorflow pandas numpy scikit-learn matplotlib`
2. Open the notebook: `jupyter notebook i211761-NabeehaFazail-Legal-Clause-Similarity.ipynb`
3. Run all cells keeping dataset in that folder.

Author
NabeehaFazail — FastID: I211761
