# 2025 Midterm

[English Version](README_EN.md)

## 프로젝트 정보
- **학번**: 2024512003
- **이름**: 김세웅
- **주제**: Training embedding models possible in CPU environments

## 프로젝트 설명
이 프로젝트는 CPU 환경(M1 Pro 칩 포함)에서 효율적으로 실행할 수 있는 경량 임베딩 모델을 미세 조정하는 방법을 보여줍니다. 작은 기본 모델(`all-MiniLM-L6-v2`)을 사용하여 사용자 정의 데이터로 미세 조정합니다.

## 필수 요구사항
- Python 3.x
- PyTorch
- Transformers
- Sentence-Transformers
- 노트북에 나열된 기타 종속성

## Google Colab 사용자를 위한 중요 안내
**주의**: 이 프로젝트는 `data/` 디렉토리에 있는 데이터 파일을 사용하며, 이 파일들은 Google Colab과 자동으로 동기화되지 않습니다. Colab에서 노트북을 실행하기 전에 다음 데이터 파일을 Colab 환경에 수동으로 업로드해야 합니다:

- `data/sentence_pairs.jsonl`
- `data/external_data.jsonl`
- `data/combined_data.jsonl`

Colab 파일 브라우저를 통해 이 파일들을 업로드하거나, 노트북 시작 부분에 다음 코드를 사용할 수 있습니다:

```python
from google.colab import files
uploaded = files.upload()  # 필요한 파일을 업로드하라는 메시지가 표시됩니다
```

## 실행 방법
1. Google Colab에서 `fine_tun_embedding.ipynb` 노트북을 엽니다
2. 위에서 언급한 대로 필요한 데이터 파일을 업로드합니다
3. 노트북의 모든 셀을 실행하여 임베딩 모델을 학습하고 평가합니다
