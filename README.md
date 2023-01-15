<H1 align="center">
YOLOv7 Segmentation with DeepSORT Tracking </H1>


I have implemented the YOLOv7 Segmantation with DeepSORT Tracking, please support by giving a star.

[`yolov7-seg.pt`](https://github.com/WongKinYiu/yolov7/releases/download/v0.1/yolov7-seg.pt)

## Steps to run Code

- Clone the repository
```
https://github.com/MuhammadMoinFaisal/yolov7-segmentation-with-DeepSORT-Tracking.git
```
- Goto the cloned folder.
```
cd yolov7-segmentation-with-DeepSORT-Tracking
```
- Create a virtual envirnoment (Recommended, If you dont want to disturb python packages)
```
### For Linux Users
python3 -m venv yolov7seg
source yolov7seg/bin/activate

### For Window Users
python3 -m venv yolov7seg
cd yolov7seg
cd Scripts
activate
cd ..
cd ..
```

- Downloading the DeepSORT Files From The Google Drive
```
cd yolov7-segmentation-with-DeepSORT-Tracking
gdown "https://drive.google.com/uc?id=1BNZ1S5yflbQpbHeRM1fNeu_2WfuP17hJ&confirm=t"
unzip /content/yolov7-segmentation-with-DeepSORT-Tracking/deep_sort_pytorch.zip
```

- Downloading a Sample Video from the Google Drive
```
gdown "https://drive.google.com/uc?id=1o-G_Fs-XtF_Nn_fQdri6GZWYtD_3_Ckw&confirm=t"
```

- Upgrade pip with mentioned command below.
```
pip install --upgrade pip
```
- Install requirements with mentioned command below.
```
pip install -r requirements.txt
```
- Download weights from [link](https://github.com/RizwanMunawar/yolov7-segmentation/releases/download/yolov7-segmentation/yolov7-seg.pt) and store in "yolov7-segmentation-with-DeepSORT-Tracking" directory.

- Run the code with mentioned command below.
```
#for segmentation with detection + Tracking
python3 segment/predict.py --source videosfinal.mp4 --weights yolov7-seg.pt --track
```

- Output file will be created in the working directory with name <b>runs/predict-seg/exp/"original-video-name.mp4"</b>

## Colab File Link 
The google colab file link is provided below, you can check the implementation in Google Colab, and its a single click implementation, you just need to select the Run Time as GPU, and click on Run All.

[`Google Colab File`](https://colab.research.google.com/drive/1I6_UpDniCsOrL5fj_bTX337Jo_UWhPGQ?usp=sharing)


## DeepSORT Files

The DeepSORT files are uplaoded in the Google Drive Link Below.
[`DeepSORT Files`](https://drive.google.com/drive/folders/1YjbfZL0n6mQH-hvD_DpoxBLVj9prJMpG)

### RESULTS

#### Vehicles Semantic Segmentation 
![](./figure/1.png)

#### Vehicles Sematic Segmentation

![](./figure/2.png)

#### Vehicles Semantic Segmentation

![](./figure/3.png)

## References
- https://github.com/WongKinYiu/yolov7.git
