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

* <b>[학습/평가 전체 소스코드](/PyTorch_CNN_MNIST_Dataset.ipynb)</b>는 Google Colab을 이용해 실행할 수 있도록 작성 중입니다.

* Todo: Pascal VOC 2007 format → Coco 2017 format
