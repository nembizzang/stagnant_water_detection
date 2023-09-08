https://drive.google.com/file/d/1vSXo9MvB-b63m9xwuUDc_kzZsDKgut8-/view?usp=sharing

1.data 구성
├── data
│   ├── Annotations
│   │   ├── COCODataset          # MMDetection에 최적화된 COCODataset 형태의 json 파일
│   │   └── OnetoOne             # 이미지와 일대일 대응되는 json 파일
│   │       ├── test_json
│   │       ├── train_json
│   │       └── val_json
│   └── Images
│       ├── MaskImages           # 라벨링을 토대로 만든 마스킹 이미지
│       │   ├── pixel_accuracy   # PA 계산을 진행한 3장의 이미지
│       │   │   ├── mask         # 라벨링을 토대로 만든 마스킹 이미지
│       │   │   ├── origin       # 모델이 예측한 이미지 (3차원)
│       │   │   └── output       # 모델이 예측한 이미지 (1차원)
│       │   ├── test
│       │   ├── train
│       │   │   └── mask_256     # (256, 256) 사이즈의 마스킹 이미지
│       │   └── validation
│       │       └── mask_256
│       ├── OriginalImages       # 모델 학습에 사용한 원본 이미지
│       └── Remainder            # 모델 학습에 사용하지 않은 나머지 이미지