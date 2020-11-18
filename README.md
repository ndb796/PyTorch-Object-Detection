### PyTorch Object Detection

* 작성자: 나동빈(Dongbin Na / dongbinna@postech.ac.kr)
* 본 코드는 POSTECH의 **CSED703G 수업** 과제로 작성한 코드입니다.

### 1. Training and Testing Faster RCNN with ResNet-50 on Pascal VOC 2007 Dataset

* <b>[학습/평가 전체 소스코드](/Faster_RCNN_with_ResNet_50_on_PASCAL_VOC_2007.ipynb)</b>는 Google Colab을 이용해 실행할 수 있도록 작성했습니다.

|Average precision|mAP@0.5|mAP@0.6|mAP@0.7|mAP@0.8|mAP@0.9|FPS|
|-----------------|---|---|---|---|---|---|
|Faster RCNN|0.726|0.660|0.533|0.331|0.079|17.1|

* **[학습된 Faster RCNN with ResNet-50 on Pascal VOC 2007 모델 다운로드 (315MB)](https://postechackr-my.sharepoint.com/:u:/g/personal/dongbinna_postech_ac_kr/EQlL8YFVuKVFuk0K_X1RuigBWZO8g9IAuEiHGH-nkZ2PLg?download=1)**

#### 2. Training and Testing Mask RCNN with ResNet-50 on Pascal VOC 2007 Dataset

* <b>[학습/평가 전체 소스코드](/Mask_RCNN_with_ResNet_50_on_PASCAL_VOC_2007.ipynb)</b>는 Google Colab을 이용해 실행할 수 있도록 작성 중입니다.
* Todo: Pascal VOC 2007 format → COCO 2017 format
* Mask 속성이 존재하지 않기 때문에 Pascal VOC 2007 데이터셋을 COCO 데이터셋으로 포팅할 필요가 있는 것으로 보입니다. ([참고](https://github.com/open-mmlab/mmdetection/issues/26))

#### 3. Training and Testing YOLO v3 with DarkNet-53 on Pascal VOC 2007 Dataset

* <b>[학습/평가 전체 소스코드](/YOLO_v3_with_DarkNet_53_on_PASCAL_VOC_2007.ipynb)</b>는 Google Colab을 이용해 실행할 수 있도록 작성 중입니다.
* 먼저 [Peterisfar](https://github.com/Peterisfar/YOLOV3)의 구현을 참고했으나 학습 속도 및 FPS 속도가 너무 느립니다. (2 FPS)
* 과제 파일에서 제안한 [eriklindernoren](https://github.com/eriklindernoren/PyTorch-YOLOv3)의 구현을 이용해도 VOC 데이터셋 적용 이슈가 있었습니다.
* (In progress) MMDetection을 이용해 구현하고자 하였으나, loss가 감소해도 validation mAP가 계속 0이 나오는 이슈가 있습니다.
