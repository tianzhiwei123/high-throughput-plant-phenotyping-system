## Introduction
- An Automated, High-throughput Plant Phenotyping System using Machine Learning-based Plant Segmentation and Image Analysis
## Folder structure
```
├── image_acquisition
│   ├── db_analysis_computer_side.py
│   ├── raspberry_side.py
│   └── sync.sh 	# data synchronization between a db_analysis_computer and a raspberry pi
├── image_processing
│   ├── analysisResult 	# result images after execution ('visualization.m')
│   │   └── README.md
│   ├── raw_data 		# raw tray images
│   │   └── README.md
│   ├── test_data		# preprocessed images after execution('preprocessing.py')
│   │   └── README.md
│   ├── train_data 		# ground truth images for training ('training.m')
│   │   └── README.md
│   ├── trainingResult
│   │   ├── training_rf.mat 	# random forest model after execution ('training.m')
│   │   ├── training_slicParameters.mat	
│   │   └── training_superpixelData.mat
│   ├── vlfeat 				# libraries for generating superpixels
│   ├── draw_contours.m 	# function of draw superpixel using contours
│   ├── preprocessing.py 	# distortion correction, cropping, arrangement
│   ├── subdir.m 			# function of file searching recursively
│   ├── test.m 				# segmentation and data processing
│   ├── training.m 			# generating a classification model
│   └── visualization.m 	# visualization using segmented images
└── README.md
```
## Development environment
- Image acquisition
	- pyserial 3.4
- Preprocessing
	- Python 2.7
	- OpenCV 3.1.0 (python)
	- Numpy 1.11.3
	- imutils 0.4.5
- Training, segmentation, visualization
	- Matlab R2016b (9.1)
	- VLFeat -- Vision Lab Features Library 0.9.20

## Usage

### Training
### Preprocessing
### Test
### Visualzaion

## Raw image
![](raw_data_example.png)

## Training image
![](gt_example1.png) ![](gt_example2.png)

## Preprocessed / superpixel / segmentation image
![](processed_example.bmp) ![](superpixel_example.bmp) ![](segmentation_example.bmp)

## Preprocessed result folder
![](preprocess_example.png)

## Segmentation result folder
![](segmentation_processing_example.png)


## Visualization
![](time_series_example.png)

![](visualization_example2.png)
![](visualization_example3.png)