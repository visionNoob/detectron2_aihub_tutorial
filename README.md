# AIHub Dataset + Detectron2 Tutorial
[Detectron2](https://github.com/facebookresearch/detectron2/tree/master/detectron2)에서 제공하는 Object Detection 알고리즘을 기반으로 [AI허브](http://aihub.or.kr/content/611)에서 제공하는 보행자 데이터셋을 학습시키기 위한 튜토리얼 문서입니다. 

또한, AI허브 보행자 데이터셋으로 학습된 pre-trained weight를 제공합니다. 

![image](https://user-images.githubusercontent.com/15168540/70385966-8ac3b980-19d6-11ea-94c7-7c793fb810f7.png)
![image](https://user-images.githubusercontent.com/15168540/70727477-1759d900-1d43-11ea-912b-de7c8797bdce.png)
![image](https://user-images.githubusercontent.com/15168540/70727520-28a2e580-1d43-11ea-80ab-636da041f292.png)


**데모 비디오**
[YouTube link](https://youtu.be/QpmHKVqvufo)

# Tutorials
1. [Detectron2 공식 튜토리얼 번역 (pre-trained by MS-COCO)](https://colab.research.google.com/github/visionNoob/detectron2_aihub_tutorial/blob/master/Detectron2_Tutorial_(kor_ver).ipynb)
2. [Detectron2 AIHUB 데이터셋 튜토리얼(inference)](https://colab.research.google.com/github/visionNoob/detectron2_aihub_tutorial/blob/master/Detectron2_AIHub_Tutorial.ipynb)
3. Detectron2 AIHUB 데이터셋 튜토리얼 (training) (준비중)

# AI허브 인도 보행 데이터셋 정보
[다운로드 링크](http://aihub.or.kr/content/611)

- 전체 이미지 수 : 105068장
- 객체 종류 : 27가지
- 전체 객체 수 : 1127907


## Data Statistics
|Class|#|Class|#|
|-|-|-|-|
|car|270978|tree_trunk|159540|
|person|143667|pole|130462|
|bollard|102722|traffic_sign|53463|
|traffic_light|49204|truck|44319|
|movable_signage|43303|potted_plant|29284|
|bicycle|19507|motorcycle|18108|
|bus|16020|bench|11116|
|chair|10122|barricade|6005|
|stop|5039|fire_hydrant|3385|
|table|3312|kiosk|3293|
|carrier|3083|stroller|790|
|scooter|429|parking_meter|251|
|dog|226|wheelchair|215|
|cat|63|
---
![image](https://user-images.githubusercontent.com/15168540/70509636-5be24a80-1b72-11ea-8a4d-a4fd0594012d.png)



# Pretrained Models (13 classes):
* Trained with 13 classes ([label.csv](https://www.dropbox.com/s/byecey0zebrn203/aihub_13_classes_label.csv?dl=0))
* You have to change your config ([example](https://www.dropbox.com/s/knvv6tyd6mna9ec/Base-RetinaNet.yaml))  
-> Change Aspect Ratios of Anchor to  
```[[0.65, 1.0, 2.47, 5.2, 18.12]]```
### RetinaNet (13 claases)
|Name|download|
|-|-|
|R50_3x|[model](https://www.dropbox.com/s/zuvj9qiuv5ntge9/retinanet_r_50_fpn_3x_aihub_final.pth) \| [metrics](https://github.com/visionNoob/detectron2_aihub_tutorial/blob/master/models/metrics.json)
