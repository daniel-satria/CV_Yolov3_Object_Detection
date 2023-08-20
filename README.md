# YOLOv3 - Object Detection
Keras(TF backend) implementation of yolo v3 objects detection. 


![alt text](https://www.dmprof.com/wp-content/uploads/2020/06/a-closer-look-at-yolov3-03.png?raw=true)


## Paper
According to the paper YOLOv3: An Incremental Improvement

- [Mediafire](https://pjreddie.com/media/files/papers/YOLOv3.pdf)
- [Arxiv](https://arxiv.org/abs/1804.02767)

## Requirement
- OpenCV 3.4
- Python 3.6    
- Tensorflow-gpu 1.5.0  
- Keras 2.1.3

## Quick start

- Download official [Yolov3.weights](https://pjreddie.com/media/files/yolov3.weights) and put it on top of folder of project.

- Run the follow command to convert darknet weight file to keras h5 file. The `yad2k.py` was modified from [allanzelener/YAD2K](https://github.com/allanzelener/YAD2K).
```
python yad2k.py cfg\yolo.cfg yolov3.weights data\yolo.h5
```

- run follow command to show the demo. The result can be found in `images\res\` floder.
```
python demo.py
```

## Demo result

It can be seen that yolo v3 has a better classification ability than yolo v2.

- On Photo
  
![Demo Prediction](https://github.com/daniel-satria/CV_Yolov3_Object_Detection/blob/main/images/res/group_people.jpg?raw=true)


- On Video
  
![Demo GIF](https://github.com/daniel-satria/CV_Yolov3_Object_Detection/blob/main/images/a-closer-look-at-yolov3-06.gif)




## TODO

- Train the model.

## Reference

	@article{YOLOv3,  
	  title={YOLOv3: An Incremental Improvement},  
	  author={J Redmon, A Farhadi },
	  year={2018}



## Copyright
See [LICENSE](LICENSE) for details.
