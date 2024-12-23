# PythonAI-hw
PythonAI homework


The Project:

The project aims to detect vehicles from videos that are made with fixed cameras with great view of moving traffic. The goal is to extract statistical information from the footage, like the position, speed and type of the vehicles, and use it to gather useful conclusions regarding the safety, possibly maintenance locations or traffic in general. In practice, a .txt file is made that contains (for each frame) the class of vehicle, and the bounding box for it.

The Dataset:

I decided to use the ua-detrac dataset. I was looking for a dataset, that includes annotated videos of moving traffic from a fixed pole overlooking the vehicles. I also wanted something large enough to be able to reliably train my model. This is just that, videos from an urban enviroment, matching my needs.

The AI model:

The model used in the project is the ultralytics yolov11n. This model is the newest at the time of making the project, and is famous among the models used for object detection. I went with the 'n' (nano) model to make the training, validating processes faster, because it seemed like it is going to take a long time (even with the nano model and T4 gpu) to do anything resourceful. Because of this I had to limit a lof of facrtors when using the model (for example only 1 epoch when training)

Installation and running instructions:

The only file needed to replicate my project is the .ipynb colab file, everything is done there. (or at least i wasn't able to run into an error when trying to)
At first, it is important to connect to a T4 gpu. (I tried using my own system)
After opening the file, the project can be seen separated to steps. You just have to follow them, and at the end the model is done. Every step is labeled.
It is really important to do every step, excludig  optional ones. After the model is done, comes the practice. In the project you can choose a video (either download one on find one online and paste in its URL) and the model will label it first, creating a vehicle_detections.txt and a output_with_labels.mp4 file.
Then in the second part, the code tries to detect vehicles that have stopped. a another set of files are created here, named stopped_vehicles.txt and output_with_stopped_vehicles.mp4. You can download these files (video files recommended)
You can install the dataset and the pretrained model, links are provided under the sources.

Sources used:
https://github.com/ultralytics/ultralytics
https://docs.ultralytics.com/tasks/detect/#models
https://docs.ultralytics.com/datasets/detect/
https://www.kaggle.com/datasets/raguhudarare/videotraffic?resource=download
https://www.kaggle.com/datasets/dtrnngc/ua-detrac-dataset (this is the dataset that was used)
https://www.youtube.com/watch?v=ZN3nRZT7b24&list=PL1FZnkj4ad1P9gulU2Ud6y-1m1fKXTPGW&index=11
chatgpt (mainly syntax related questions)


Files that were used:

pythonAIhw.ipynb : file that stores the code written in google colab enviroment, This is where all of the source code can be found
The link for the google colab: https://colab.research.google.com/drive/10Pf3-FqIj1Qf2I0m6M1BGum96YyrOA9V?usp=sharing
This link is for a google drive that contains videos regarding the google colab file.
https://drive.google.com/drive/u/3/folders/1R9AihHURIV4v2njU7BQRH6ved6Ut6RS6
This drive contains the demo video as well.


