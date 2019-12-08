# Detectron2 + AIHub Dataset Tutorial
![image](https://user-images.githubusercontent.com/15168540/70385966-8ac3b980-19d6-11ea-94c7-7c793fb810f7.png)


[DEMO_VIDEO](https://youtu.be/QpmHKVqvufo)

## Pretrained Models:
* Trained with 13 classes ([label.csv](https://www.dropbox.com/s/byecey0zebrn203/aihub_13_classes_label.csv?dl=0))
* You have to change your config ([example](https://www.dropbox.com/s/knvv6tyd6mna9ec/Base-RetinaNet.yaml))  
-> Anchor Aspect Ratio to  
```[[0.65, 1.0, 2.47, 5.2, 18.12]]```
### RetinaNet
|Name|download|
|-|-|
|R50_3x|[model](https://www.dropbox.com/s/zuvj9qiuv5ntge9/retinanet_r_50_fpn_3x_aihub_final.pth) \| [metrics](https://github.com/visionNoob/detectron2_aihub_tutorial/blob/master/models/metrics.json)
