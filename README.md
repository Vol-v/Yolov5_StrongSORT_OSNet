# Yolov5 + StrongSORT with OSNet fork
```latex
@misc{yolov5-strongsort-osnet-2022,
    title={Real-time multi-camera multi-object tracker using YOLOv5 and StrongSORT with OSNet},
    author={Mikel Broström},
    howpublished = {\url{https://github.com/mikel-brostrom/Yolov5_StrongSORT_OSNet}},
    year={2022}
}
```
This is a fork of a Yolov5+StrongSORT repository for my CV project. 

### Notable changes

#### track.py

track.py file was changed according to the project. 
Number of detections per frame was changed to two, since there are only two dogs that need to be detected.
After nonmax suppression I added an additional check that classes that were detected are different. If they are the same - I change the bbox with lower class probability to opposite class.
 
### Example

In the runs/track/ you can find an example of algorithm working with pretrained yolov5
