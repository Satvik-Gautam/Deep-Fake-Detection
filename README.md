# Deep-Fake-Detection
Our project focuses on developing an advanced DEEPFAKE detection model by using MTCNN , InceptionResNet and LSTMs. MTCNN, a robust face detection framework, is used to crop out the face, while InceptionResNet does an analysis of facial attributes and the learns facial features corresponding to a real face, this neural network hence learns the difference in deepfake and real images.
for detection of deepfake videos we further add an LSTM , this LSTM helps us capture the temporal inconsistencies (flicker) in the deepfake videos , this makes our model more robust and accurate.

For Images , we plan to use an MTCNN to crop out the face images from each image , we will train an InceptionResnet to learn the facial features of a natural face , this way it can discern between a real and a deepfake image
-For Videos , we plan to use an MTCNN , then an InceptionResnet (same as for images) , but we add a layer of LSTM this way we can capture the flicker of deepfake videos, as LSTMs are good for capturing features in continuos data (videos in this case)

Our model is made more power efficient by careful and meticulous choice of neural network architectures , the RESIDUAL connections in the network solve the  vanishing gradient problem by using skip connections , the LSTMs also solve the vanishing gradient problem over long sequences making the training much more efficient , this way lesser epochs are required to train the AI model and hence lesser resources are required .Also the Inception modules (1x1 convolutions) help in cutting costs by reducing the amount of calculations required. This way we reduce the computational and power requirements of our deepfake detection model and hence make the model financially feasible


https://github.com/Satvik-Gautam/Deep-Fake-Detection/assets/115337328/3d7b42ba-3957-48f1-a505-cdc72d187a34

