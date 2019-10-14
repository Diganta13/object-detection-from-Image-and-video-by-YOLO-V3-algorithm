# object-detection-from-Image-and-video-by-YOLO-V3-algorithm

In this article, we we’ll be using a Python library called ImageAI that has made it possible for anyone with basic knowledge of Python to build applications and systems that can detect objects in videos using only a few lines of programming code. ImageAI supports YOLOv3, which is the object detection algorithm we’ll use in this article.

To get started, you will install a number of Python libraries and ImageAI. If you have any of the dependencies mentioned below already installed on your computer, you can jump straight to the installation of ImageAI. Also ensure the Python version you have installed on your computer is Python 3.

pip3 install the following dependencies:

i. TensorFlow (tensorflow)

ii. Numpy (numpy)

iii. SciPy (scipy)

iv. OpenCV (opencv-python)

v. Pillow (pillow)

vi. Matplotlib (matplotlib)

vii. H5py (h5py)

viii. Keras (keras)

ix. ImageAI (https://github.com/OlafenwaMoses/ImageAI/releases/download/2.0.2/imageai-2.0.2-py3-none-any.whl )


Now that we’ve installed the tools you need, we’ll be using a trained YOLOv3 computer vision model to perform the detection and recognition tasks. We can download the model file via this link. This model is trained to detect and recognize 80 different objects, named below:

person, bicycle, car, motorcycle, airplane,
bus, train, truck, boat, traffic light, fire hydrant, stop_sign,
parking meter, bench, bird, cat, dog, horse, sheep, cow, elephant, bear, zebra,
giraffe, backpack, umbrella, handbag, tie, suitcase, frisbee, skis, snowboard,
sports ball, kite, baseball bat, baseball glove, skateboard, surfboard, tennis racket,
bottle, wine glass, cup, fork, knife, spoon, bowl, banana, apple, sandwich, orange,
broccoli, carrot, hot dog, pizza, donot, cake, chair, couch, potted plant, bed,
dining table, toilet, tv, laptop, mouse, remote, keyboard, cell phone, microwave,
oven, toaster, sink, refrigerator, book, clock, vase, scissors, teddy bear, hair dryer,
toothbrush.

For the purpose of this article, we’ve provided a sample video that you can download and use to write code to detect and recognize objects in the video. Download the video via this link.

Next, we create a Python file and give it a name, e.g FirstVideoDetection.py. Then we copy both the downloaded video and YOLOv3 model file into the folder where our FirstVideoDetection.py file is. Once you have done that, we write the exact code below into our FirstVideoDetection.py file.



Before we run our Python code, here’s an in-depth explanation of the preceding code:

1) In the fourth line, we created an instance of the VideoObjectDetection class.

2) In the fifth line, we set the model type to YOLOv3, which corresponds to the YOLO model we downloaded and copied to the folder.

3) In the sixth line, we set the model path to the file path of the model file we copied into the folder.

4) In the seventh line, we loaded the model into the instance of the VideoObjectDetection class that we created.

5) In the eight line, we called the detectObjectsFromVideo function and parsed the following values into it:

i. input_file_path: This refers to the file path of the video we copied into the folder.

ii. output_file_path: This refers to the file path to which the detected video will be saved.

iii. frames_per_second: This refers to the number of image frames that we want the detected video to have within a second.

iv. log_progress: This is used to state that the detection instance should report the progress of the detection in the command line interface.

6) The detectObjectsFromVideo function will return the file path of the detected video. This file path will be printed in the ninth line of code once the detection task is done.
