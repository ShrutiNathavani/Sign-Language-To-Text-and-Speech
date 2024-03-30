# **Sign-Language-To-Text-and-Speech-Conversion 💬👋**

## **Abstract**

Sign language is one of the oldest and most natural forms of language for communication. In this project, we have developed a real-time method using neural networks for finger spelling-based American Sign Language (ASL). We propose a convolutional neural network (CNN) approach to recognize hand gestures from camera images. The CNN method aims to identify hand gestures from a camera image by utilizing the position and orientation of the hand for training and testing data. The hand undergoes filtration and classification to predict the class of hand gestures, followed by training the CNN using calibrated images.

**The Final Outcome Of Our Project:** 
- `hello_there.mp4`: [Video demonstrating the project]

## **Introduction**

American Sign Language (ASL) serves as a predominant means of communication for individuals with communication-related disabilities such as deafness and muteness. Communication involves the exchange of thoughts and messages through various mediums, including speech, signals, behavior, and visuals. Deaf and dumb (D&M) individuals express their ideas through hand gestures, which are nonverbally exchanged messages understood through vision, known as sign language. This project aims to develop a model to recognize fingerspelling-based hand gestures, forming complete words by combining each gesture.



![image](https://github.com/ShrutiNathavani/Sign-Language-To-Text-and-Speech/assets/77912009/e9b62ed7-3c42-4768-b04c-a149a71c8d19)



## **Requirements**

Over 70 million deaf individuals worldwide rely on sign languages for communication, enabling them to learn, work, access services, and participate in communities. However, teaching sign language to everyone is challenging. Therefore, the goal is to develop a user-friendly Human-Computer Interface (HCI) that understands American Sign Language, simplifying communication for the deaf and dumb community.

## **Objective**

The primary objective is to create a computer software application and train a CNN model capable of interpreting images of hand gestures in American Sign Language. The system converts recognized gestures into text format and optionally into audio format, enhancing communication accessibility.

## **Scope**

The system benefits both the deaf and dumb community and individuals unfamiliar with sign language. By interpreting sign language gestures, the system provides output in both text and speech formats, promoting inclusivity and bridging communication barriers.

## **Modules**

### **Data Acquisition**

- **Electromechanical Devices**: Utilize devices for precise hand configuration and position data. Although effective, this approach is costly and less user-friendly.
- **Vision-based Methods**: Utilize computer webcams to observe hand gestures, offering a cost-effective solution for natural interaction between humans and computers.

### **Data Pre-processing and Feature Extraction**

- **Hand Detection**: Employ the MediaPipe library for image processing to detect hands from webcam images. MediaPipe provides robust hand landmark estimation and tracking, essential for accurate gesture recognition.
- **Image Processing**: Convert detected regions of interest (ROI) to grayscale images using OpenCV library. Apply Gaussian blur and thresholding techniques to enhance image quality.
- **Data Collection**: Gather images of different signs from various angles for sign letters A to Z.

### **Gesture Classification**
- **MediaPipe Landmark System**: Use MediaPipe to detect hand landmarks from webcam images. Draw and connect these landmarks in a simple white image to overcome challenges related to background and lighting conditions.

  ![image](https://github.com/ShrutiNathavani/Sign-Language-To-Text-and-Speech/assets/77912009/f02208e8-2554-4359-b1f3-b8124d8037ef)


![image](https://github.com/ShrutiNathavani/Sign-Language-To-Text-and-Speech/assets/77912009/ab0f2d82-9246-4add-99dc-dd4d4f4a3315)

![image](https://github.com/ShrutiNathavani/Sign-Language-To-Text-and-Speech/assets/77912009/388e0458-7c6f-4c13-b7aa-08ded2651ef2)

![image](https://github.com/ShrutiNathavani/Sign-Language-To-Text-and-Speech/assets/77912009/50d2ba3c-bb95-4cbb-985b-be85a8e88380)



- **Convolutional Neural Network (CNN)**:
  
CNN is a class of neural networks that are highly useful in solving computer vision problems. They found inspiration from the actual perception of vision that takes place in the visual cortex of our brain. They make use of a filter/kernel to scan through the entire pixel values of the image and make computations by setting appropriate weights to enable detection of a specific feature. CNN is equipped with layers like convolution layer, max pooling layer, flatten layer, dense layer, dropout layer and a fully connected neural network layer. These layers together make a very powerful tool that can identify features in an image. The starting layers detect low level features that gradually begin to detect more complex higher-level features

Unlike regular Neural Networks, in the layers of CNN, the neurons are arranged in 3 dimensions: width, height, depth.

The neurons in a layer will only be connected to a small region of the layer (window size) before it, instead of all of the neurons in a fully-connected manner.

Moreover, the final output layer would have dimensions(number of classes), because by the end of the CNN architecture we will reduce the full image into a single vector of class scores.

**Convolutional Layer:**

In convolution layer I have taken a small window size [typically of length 5*5] that extends to the depth of the input matrix.

The layer consists of learnable filters of window size. During every iteration I slid the window by stride size [typically 1], and compute the dot product of filter entries and input values at a given position.

As I continue this process well create a 2-Dimensional activation matrix that gives the response of that matrix at every spatial position.

That is, the network will learn filters that activate when they see some type of visual feature such as an edge of some orientation or a blotch of some colour. 


![image](https://github.com/ShrutiNathavani/Sign-Language-To-Text-and-Speech/assets/77912009/4b5099a6-135f-4ca0-98ec-6cc07cf1c5ca)


  ![image](https://github.com/ShrutiNathavani/Sign-Language-To-Text-and-Speech/assets/77912009/58b77e4e-3d2c-4bf0-8ea7-de50d52b423c)

**Pooling Layer:**

We use pooling layer to decrease the size of activation matrix and ultimately reduce the learnable parameters.

There are two types of pooling:

**Max Pooling:**

In max pooling we take a window size [for example window of size 2*2], and only taken the maximum of 4 values.

Well lid this window and continue this process, so well finally get an activation matrix half of its original Size.

**Average Pooling:**

In average pooling we take average of all Values in a window pooling

![image](https://github.com/ShrutiNathavani/Sign-Language-To-Text-and-Speech/assets/77912009/a662883e-a520-4aa7-9452-82eb07cf4c4c)


### **Text To Speech Translation**

- Translate recognized gestures into words using the `pyttsx3` library. This feature simulates real-life dialogue and enhances user experience.

## **Project Requirements**

### **Hardware Requirement:**
- Webcam

### **Software Requirement:**
- **Operating System**: Windows 8 and Above
- **IDE**: PyCharm
- **Programming Language**: Python 3.9
- **Python Libraries**: OpenCV, NumPy, Keras, MediaPipe, TensorFlow

## **System Diagrams**

### **System Flowchart**

![System Flowchart](https://github.com/ShrutiNathavani/Sign-Language-To-Text-and-Speech/assets/77912009/f6a9b8c3-a2b5-485b-977c-846bd689d5e9)

### **Use-case Diagram**

![Use-case diagram](https://github.com/ShrutiNathavani/Sign-Language-To-Text-and-Speech/assets/77912009/69e077ed-b12a-4a9a-9cb2-9d3d64b345f0)

### **DFD Diagram**

![DFD diagram](https://github.com/ShrutiNathavani/Sign-Language-To-Text-and-Speech/assets/77912009/85081d60-7dab-440f-b0f9-3f90b8a761d7)

### **Sequence Diagram**

![Sequence diagram](https://github.com/ShrutiNathavani/Sign-Language-To-Text-and-Speech/assets/77912009/f633d5c0-cbbf-43d4-a628-da79a46cfa88)

---

This README provides an overview of the Sign-Language-To-Text-and-Speech-Conversion project, outlining its objectives, modules, and system requirements. For further details, refer to the accompanying documentation and codebase.

## **License**

This project is licensed under the [MIT License](LICENSE).

## **Acknowledgements**

We would like to thank the developers of OpenCV, NumPy, Keras, MediaPipe, and TensorFlow for their invaluable contributions to this project.

