# video-based-face-mask-recognition-by-opencv

This project is a video-based face mask recognition system using OpenCV and deep learning. The code contains a function called "detect_and_predict_mask" which takes a video frame, a pre-trained face detection model, and a pre-trained face mask recognition model as inputs.

The function first resizes the input frame to a standard size of 224x224 pixels, creates a blob from the image, and passes it through the face detection model to obtain the face detections. The detected faces are then passed through the face mask recognition model to predict whether the person in the frame is wearing a face mask or not.

The function returns a list of faces, their corresponding locations, and the predictions from the face mask recognition model. These predictions are used to draw a bounding box around each detected face and label it as wearing a mask or not.

Additionally, the code also includes a training phase for the face mask recognition model. It uses a pre-trained MobileNetV2 model and fine-tunes it on a dataset of masked and unmasked faces. The training process is monitored using metrics such as loss and accuracy, which are plotted using Matplotlib.

Overall, this project is a useful application of computer vision and deep learning for real-world problems, particularly in the context of the ongoing COVID-19 pandemic where face mask detection is crucial for public health and safety.
