# PythonAI-hw
PythonAI homework


The Project:

The project aims to detect vehicles from videos that are made with fixed cameras with great view of moving traffic. The goal is to extract statistical information from the footage, like the position, speed and type of the vehicles, and use it to gather useful conclusions regarding the safety, possibly maintenance locations or traffic in general.

The Dataset:

I decided to use the ua-detrac dataset. I was looking for a dataset, that includes annotated videos of moving traffic from a fixed pole overlooking the vehicles. I also wanted something large enough to be able to reliably train my model. This is just that, videos from an urban enviroment, matching my needs.

The AI model:

The model used in the project is the ultralytics yolov11n. This model is the newest at the time of making the project, and is famous among the models used for object detection. I went with the 'n' (nano) model to make the training, validating processes faster, because it seemed like it is going to take a long time (even with the nano model and T4 gpu) to do anything resourceful. 

Iinstallation and running instructions:

The only file needed to replicate my project is the .ipynb colab file, everything is done there. (or at least i wasn't able to run into an error when trying to)
After opening the file, the project can be seen separated to steps. You just have to follow them, and at the end the model is done.
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

dataset.yaml : file that stores the path for the dataset that is used to train and validate the model
pythonAIhw.ipynb : file that stores the code written in google colab enviroment


