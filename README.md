
# Project Title

Footfall counting in a video




## Description

For the given assignmnet I have used Nvidia-Deepstream 6.2 SDK, CUDA version 11.8,python 3.8, Ubuntu 20.04.

## Video

Due to time constraint I have trimmed the hour long video into 34 mins video and have used the same to do the assignment.

## Model

I have used yolov8m model which is already pretrained on coco dataset containing 80 classes.

## Accuracy

Accuracy = Number of correct predictions / Total number of predictions

The manual count for exit is 17, but the computer count is of 18. Accuracy with respect to exit is of 94%.

The manual count for entry is 2 ,the computer count is also 2. Accuracy with respect to entry is of 100%

## Link

Here I am attaching the link for infered video,please find the same.

link:https://drive.google.com/file/d/1RMTT3bI-hohDKelLue_8zYrg4k-6908u/view?usp=drive_link

## commands

```
git clone https://github.com/Yashovardhan0317/nextbrain

cd nextbrain/nvdsinfer_custom_impl_Yolo

sudo make clean

sudo make

cd ..
```
 
to download the wts file, the wts file should be placed in same location as that of yolov8m.cfg file

```
gdown --fuzzy https://drive.google.com/file/d/1yNC839YLgpvDBHrPWQZ89EstrH6NwvUS/view?usp=sharing
```

to run the code use following command.

```
sudo python3 deepstream_nvdsanalytics.py file:/path/to/video.mp4
```






