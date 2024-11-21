# face-detection
Yolo11n을 활용한 Face Detection 모델 개발

# 데이터셋
- My Face
  - Galaxy S10으로 찍은 1,210장의 jpg
  - Yolo8n 모델로 진행한 Annotation TXT File
- Other Face
  - 7,238장의 다른 사람 사진
  - 7,238개의 Annotation TXT File

# Procedure
1. Pre-processing
  - Annotation
    - Roboflow
    - Yolo8n.pt
  - Labeling
2. Data Augumentation
  - RandomBrightnessContrast(brightness_limit=0.2, contrast_limit=0.2, p=0.5)
  - GaussNoise(var_limit=(10.0, 50.0), p=0.5)
  - Blur(blur_limit=3, p=0.3)
3. Make Structure to use YOLO11n
  - create label txt file
  - move jpg file
4. Run
5. Enhancing
6. Save
