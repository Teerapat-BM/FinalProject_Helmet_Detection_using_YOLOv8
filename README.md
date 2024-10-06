# Helmet_Detection using YOLOv8
First step :
Create Python environment
    > Python:Create Environment
    > Choose : Python v. 3.7 --> 3.11 # if have error, try to use python version 3.8 

First Command :
    " .venv\Scripts\activate "

Image Genarator :
    - select your video
    - change path in file img.py on line 17 to your folder which you select to save.
    - use this command " pip install labelimg ultralytics " for install labelimg and cv2 framework.
    - type " labelimg " in terminal for open labelimg framwork. 
    - create folder label and change save label in this folder.
    - change model for use to YOLO and create rectangle to helmet,
    - when finished this process create dataset folder.
    - in dataset folder, create images and labels folder.
    - in images and labels folder, create training and validation folder.
    - copy all datas classes and images and paste to training and validation folder.
    - zip this file.

Train model(Colab) :
    - upload zip file to your google drive
    - open yolov8_trainmodel.ipynb in colab
    - when conneted google drive, change path to your zip file and unzip it with code in colab
    - create a new file name " data.yaml " in folder dataset and run
    - when process was finished, check in folder runs\detect\train\weights
    - download best.pt and last.pt to model folder

Install framework libary : 
    " pip install fastapi[standard] sqlalchemy scipy requests"

Run program :
    " fastapi dev api.py "
    " cd frontend "
    " python -m http.server 8080 "
    " python count.py "

Checking api server and dastboard:
    " http://localhost:8000/docs "
    " http://localhost:8000 "

Thanks!!