## YOLO_tensorflow

Tensorflow implementation of [YOLO](https://arxiv.org/pdf/1506.02640.pdf), including training and test phase.

### Installation

1. Clone yolo_tensorflow repository
	```Shell
	git clone https://github.com/hizhangp/yolo_tensorflow.git
  cd yolo_tensorflow
	```

2. Download Pascal VOC dataset, we call the directory `PASCAL_VOC`
	```Shell
	mkdir data
	cd data
	wget http://host.robots.ox.ac.uk/pascal/VOC/voc2007/VOCtrainval_06-Nov-2007.tar
	tar -xvzf VOCtrainval_06-Nov-2007.tar
	cd ..
	ln -s $PASCAL_VOC$ data/pascal_voc
	```

3. Download [YOLO_small](https://drive.google.com/file/d/0B2JbaJSrWLpza08yS2FSUnV2dlE/view?usp=sharing)
weight file and put it in `data/weight`

4. Modify configuration in `yolo/config.py`

5. Training
	```Shell
	python train.py
	```

6. Test
	```Shell
	python test.py
	```

### Requirements
1. Tensorflow

2. OpenCV
