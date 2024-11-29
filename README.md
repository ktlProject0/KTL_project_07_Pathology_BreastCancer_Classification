# KTL_project_07_Pathology_BreastCancer_Classification

Zip 파일은 경로 내 압축해제 후 사용.

        ./KTL_project_07_Pathology_BreastCancer_Classification
        |-- Code
        |   |   |-- 01. Training-checkpoint.ipynb
        |   |   `-- 02. Evaluation-checkpoint.ipynb
        |   |-- 01. Training.ipynb
        |   |-- 02. Evaluation.ipynb
        |   |-- monai
        |   |   |-- MOANI 라이브러리
        `-- Data
            |-- 10253 (환자번호)
            |   |-- 0 (Benign 영역)
            |       |-- ....png
            |   |-- 1 (Malignant 영역)
            |       |-- ....png

## Data Description
1. 학습용 데이터 (/Data/...)
   - 각 환자의 병리 슬라이드 영역에서 cancer:1, narmal:0 폴더명으로 구분

## Code Description
## Training.ipynb
  - 네트워크 학습 코드
  - Monai 프레임워크, DenseNet121 네트워크 구조 사용
## Evaluation.ipynb
  - 네트워크 성능 평가 및 분류 결과 가시화 (ROC Curve)
  - 학습완료 된 모델 가중치 (/Code/output/model_final.pth)
