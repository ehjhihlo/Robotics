# CSIE5047 Robotics: Chinese Poker Self-Playing Robot
We propose a robotic system "Chinese Poker Self-Playing Robot". Controlled by TM-5 robot arm, the robot can suck the cards from the card stack and put them on the card rack, then take a photo to get card information to decide which card to play.  
[Paper](https://drive.google.com/drive/folders/1NFoayeRmJ_lkm18iyVWcGBsV-6Qn89ku?hl=zh-tw)  
[Demo](https://www.youtube.com/watch?v=SdnazMHygp0)  

## Execution
One can execute the system by running the following command:
```
python3 image_sub_new.py

python3 send_script.py
```
## Yolov5 Object Detection
The yolov5 training code is loaded from [here](https://github.com/ultralytics/yolov5).  
### Training
Train the yolov5 model with the following script:
```
python3 train.py --img 416 --batch 16 --workers 2 --epochs 120 --data (poker card data path) --weights yolov5s.pt --cache
```
