# Small-Object-Detection

<a href="https://colab.research.google.com/drive/14jbS3PoEEKZNkVMofrKQl2bHLC8oxA_y#scrollTo=rDuvNsnH0OEV" rel="nofollow"><img src="https://camo.githubusercontent.com/96889048f8a9014fdeba2a891f97150c6aac6e723f5190236b10215a97ed41f3/68747470733a2f2f636f6c61622e72657365617263682e676f6f676c652e636f6d2f6173736574732f636f6c61622d62616467652e737667" alt="Open In Colab" data-canonical-src="https://colab.research.google.com/assets/colab-badge.svg" style="max-width: 100%;"></a>


train-yolov10-local.ipynb 파일을 실행하면 <br>
data, weights, yolov10, YOLOv10-Experiment 파일을 생성하게 됩니다. <br>
데이터 셋은 필요에 따라 data 폴더 내부에 업로드 해주시기 바랍니다. <br>

# YOLOv10 설계 모듈 `yolov10/ultralytics/nn/modules` 

```plaintext
ultralytics/
└── nn/
    └── modules/
        ├── __pycache__/        # (컴파일된 Python 파일 캐시)
        ├── __init__.py          # 패키지 초기화 파일
        ├── block.py             # 네트워크의 기본 블록 (예: Residual, C2f 등)
        ├── conv.py              # CNN 관련 Convolution 연산 정의
        ├── head.py              # YOLO 헤드 (Detection Head, Output Layer)
        ├── transformer.py       # Transformer 기반 구조 (Attention 등)
        ├── utils.py             # 유틸리티 함수 (가중치 초기화, 텐서 변환 등)
