Problem Statement:      Blind individuals face numerous challenges in navigating their surroundings independently, particularly when it comes to identifying and avoiding obstacles in their path. Traditional assistive devices such as canes and guide dogs offer some assistance, but they have limitations in providing detailed information about the environment.

Approach towards the solution:      Our strategy to address the challenges encountered by individuals with visual impairments involves the development of an innovative assistive technology system. Leveraging the computational capabilities of ESP32-based camera modules in conjunction with OpenCV, a versatile computer vision library, we aim to implement advanced object detection algorithms. By utilizing the SSD (Single Shot MultiBox Detector) architecture with the package file `ssd_mobilenet_v3_large_coco_2020_01_14.pbtxt` and associated weights stored in `frozen_inference_graph.pb`, our system will perform real-time analysis of the surrounding environment. Through the fusion of sensor data and deep learning techniques facilitated by OpenCV, our solution will provide users with detailed insights into potential obstacles in their path. By prioritizing user-centric design principles and seamless integration, our goal is to empower individuals with visual impairments, enhancing their navigational experience and fostering greater independence in daily activities.

Tech Stack:
1. Hardware:
   - ESP32-based camera modules: Provides video input for object detection.
   - Processing chip: Executes the software components of the system and interfaces with the ESP32 camera module.
   - ESP pins: Used for hardware connections and interfacing with peripherals.
   - Wi-Fi and Bluetooth module: Enables wireless communication and networking capabilities.
 
2. Software:
   - OpenCV: A powerful computer vision library for processing video input, performing object detection, and displaying results.
   - TensorFlow and PyTorch: Deep learning frameworks used for training and deploying the object detection model.
   - SSD (Single Shot MultiBox Detector) architecture: A deep learning model architecture optimized for real-time object detection.
   - Pre-trained model files: Includes the package file (.pbtxt) and associated weights (.pb) for the object detection model.
   - Python: Programming language used for developing the software components of the system.
   - C++: Used for hardware coding and interfacing with the processing chip.
   - .ino files: Arduino sketch files for programming the ESP32 module.
   - Additional required libraries: Includes libraries for wireless communication, sensor interfacing, and other functionalities.

3. Networking:
   - Wi-Fi or Ethernet connection: Enables communication between the ESP32 module and other devices on the network.

4. Version Control:
   - Git: Version control system for managing the project's source code, tracking changes, and collaborating with team members.

Workflow Overview:

1. Hardware Integration:
   - We integrate essential hardware components into smart glasses, including an ESP32-based microcontroller, a camera module, and wireless modules (Wi-Fi, Bluetooth). The camera is strategically positioned to capture the wearer's surroundings.

2. Object Detection:
   - The camera captures live video, processed by the ESP32 microcontroller using OpenCV.
   - Employing the SSD architecture with TensorFlow or PyTorch, real-time object detection is performed, accurately identifying objects in the wearer's environment.

3. Distance Estimation:
   - Using geometric principles, the system calculates the distance between the wearer and detected objects.
   - By calibrating known object dimensions with their size in the video feed, precise distance estimation is achieved.

4. Class Prediction and Confidence:
   - Simultaneously, the system predicts the class of detected objects (e.g., person, chair) with high accuracy.
   - Deep learning algorithms, based on pre-trained models, facilitate reliable class prediction and confidence calculation.

5. Continuous Monitoring:
   - As the wearer moves, the system dynamically updates distance calculations for detected objects, ensuring real-time monitoring.
   - Variations in distance due to wearer and object movement are continuously adjusted.

6. User Alerting:
   - When the distance between the wearer and the object falls below a set threshold (e.g., 25 cm), the system triggers an alert.
   - Auditory feedback via headphones or a wearable device promptly notifies the wearer of approaching obstacles, enabling timely action.

7. Hardware-Software Synergy:
   - Hardware components (ESP32, camera) synergize seamlessly with software algorithms (OpenCV, TensorFlow/PyTorch), ensuring efficient data processing and accurate object detection.
   - This integrated approach optimizes performance, enabling rapid response and reliable detection capabilities.



  Circuitry Diagram:-
  
   ![WhatsApp Image 2024-05-11 at 05 47 12_2252994b](https://github.com/VishalRawatt/TeamIndia_HackFest/assets/94183896/647d241e-57e0-48a3-b9a1-6363c6f34215)

   
   ![WhatsApp Image 2024-05-11 at 05 47 11_3c5dadd1](https://github.com/VishalRawatt/TeamIndia_HackFest/assets/94183896/206f63ff-c4f0-4dac-845b-763f047799e9)


   Circuit Connection:-
![WhatsApp Image 2024-05-11 at 01 55 21_cdb76458](https://github.com/VishalRawatt/TeamIndia_HackFest/assets/94183896/78534828-1051-4a3d-8c4b-a100e07d27b8)



