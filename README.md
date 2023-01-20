# Smart Environment Eye [SEE]
####  *DeepBrain Team contribution in Smartathon challange*
\
***Smart Environment Eye [SEE]** is an advanced AI-powered object detection system that can detect and classify visual pollutants in real-time. The system is equipped with state-of-the-art computer vision techniques to accurately detect and classify pollutants such as graffiti, garbage, sand on roads, potholes, cluttered sidewalks, bad billboards, etc...*

<img src="project_images\f1.PNG" width="500px" hight="500px"/> 

*The system can be installed on an Android device, an Edge device, or can be integrated with city
surveillance cameras, the system will be connected to GPS and the Internet and can send detected visual
pollutants, their type, and their location in real-time to city officials and display them via a monitoring
dashboard, allowing them to take immediate action and keep the city clean.*
<img src="project_images\f2.PNG" width="500px" hight="500px"/> 

[Demo](https://huggingface.co/spaces/alshimaa/SEE)

[app](https://drive.google.com/file/d/1-0rna-jzAHyEjBUvbf3qIy2G3foGiIZo/view?usp=sharing)


## ***Training and detection***


- download and run the [notebook](https://drive.google.com/file/d/1OrQnXXaFTzuo6-_7malWLoszdM8pgjuX/view?usp=sharing)

-  For **Training** you will need to download [this yaml](https://drive.google.com/file/d/1fntLs720iULfH-cgd2kTcbeaPRwUWymp/view?usp=sharing) file in the folder "./dataset/yolov7/data/" ,  and you will need to change number of classes nc = 80 to nc=11 in ./dataset/yolov7/cfg/training/yolov7.yaml 

- For **Detection** 
  - Download model [weights](https://drive.google.com/file/d/1Cw9F1tevtxwx9ZyCVx7aGjiknQD99muO/view?usp=sharing)
  
  - run 
  `! python detect.py --weights " model.pt path" --img 736 --conf 0.27 --source "testing image path" --save-txt`
