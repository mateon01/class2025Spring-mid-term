# 2025 Midterm Project

[한국어 버전](README.md)

## Project Information
- **Student ID**: 2024512003
- **Name**: Kim, Sewoong
- **Subject**: Training embedding models possible in CPU environments

## Project Description
This project demonstrates how to fine-tune a lightweight embedding model that can run efficiently on CPU environments, including M1 Pro chips. The implementation uses a small base model (`all-MiniLM-L6-v2`) and fine-tunes it with custom data.

## Prerequisites
- Python 3.x
- PyTorch
- Transformers
- Sentence-Transformers
- Other dependencies listed in the notebook

## Important Note for Google Colab Users
**ATTENTION**: This project uses data files located in the `data/` directory which are not automatically synchronized with Google Colab. Before running the notebook in Colab, you must manually upload the following data files to your Colab environment:

- `data/sentence_pairs.jsonl`
- `data/external_data.jsonl`
- `data/combined_data.jsonl`

You can upload these files through the Colab file browser or use the following code at the beginning of your notebook:

```python
from google.colab import files
uploaded = files.upload()  # This will prompt you to upload the required files
```

## How to Run
1. Open the `fine_tun_embedding.ipynb` notebook in Google Colab
2. Upload the required data files as mentioned above
3. Run all cells in the notebook to train and evaluate the embedding model
