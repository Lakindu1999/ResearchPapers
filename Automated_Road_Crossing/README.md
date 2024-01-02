Automated Road Crossing System Using Real-Time Object Tracking

Abstract


Traffic congestion and pedestrian accidents are two major components that a busy city face today. Many social, economic and environmental problem increase due to that two issues. One of the biggest reason for that is the obsolete pedestrian light controlled crossing system exists these days. As a solution to this we have proposed real time object tracking automated road crossing system. The proposed system first take live video input to the system using webcam / CCTV Camera. For the testing phase we read a video file (frames) for input to the system. Then it converted into gray scale for more accuracy after that using blur function for noise reduction and detect the humans and indicate its using rectangle. In the meanwhile the system count number of persons waiting to road crossing. According to the algorithms of the project will be started.

According to the project algorithm waiting time will be displayed on the Arduino character display. Then the system shows green light to the pedestrians and red light to the vehicles.





Introduction


The Pedestrian push button traffic control or the Ped call button that exist in most crossing areas are used to change traffic light transitions by the pedestrians in order to have their turn to cross. Another device that is found in some areas is the Closed-circuit television cameras. They are also used to monitor areas or things that could to help security personnel’s investigate acts harmful to human and infrastructure. Hence cameras are now used for pedestrian detection feature to detect the presence of people. This type is used in the streets to know if the pedestrian wants to cross the street, which is similar with a Ped call system.[1] This makes a cameras on pedestrian lane have additional functionality to help the pedestrians consider their turn to cross. The application used is real-time which does not record the amount of frames of images to analyse. For cross-line roadways, multi-camera surveillance is implemented to utilize a mathematical approach for switching emergency events. On evening rush hours, surveillance processing for monitoring vehicle movements is essential.[1] This study of Haar Cascaded Algorithm for object and digital image recognition leads to Haar features have been studied intensely for the detection of objects, in particular for face detection. One another major feature used for object detection is provided by HOG as evaluated in. Pedestrians, faces and bicycles are successfully detected when represented by HOG  algorithm also used for pedestrian. [2]

The absence of initiating Ped call button while waiting by uninformed people was observed. Existing face detection and pedestrian detection algorithms, were not previously used in the pedestrian detections. The proposed system, should integrate an image processing system into a camera system thus eliminating the push button system.[3]


Objectives and Scope


The main objective of this project is to give flexible and safe road crossing for the pedestrians, with the help of Advanced Information Technology.

There have some more objectives for different parties like,
o	To minimize the traffic jam and pedestrian accident.
o	To minimize environment pollution and all other negative impacts of traffic congestion.
o	To endow the country with a law abiding, moral and socially useful person.
o	To make the society aware of the advancement of technology and the impact of computer science on it.




System Analysis


Identification of needs and feasibility study

The Pedestrian push button traffic control or the Ped call button that exist in most crossing areas are used to change traffic light transitions by the pedestrians in order to have their turn to cross the road.[1] But the problem with this system is that if the button is not working/broken, then the pedestrian control system is not working. With the current technology in the world, people need a more luxurious, quality and convenient system. In some developing countries, automatic pedestrian crossing have also been developed using infrared sensor (IR Sensor). But there are problems with this system as well. For example, if there is an object near the pedestrian crossing other than the people, the algorithm used to assume that one person is about to cross the road may work. And the accuracy of the data in this sensor may change depending on the weather.

After studying these key issues, we plan to look for solutions in a new dimension. Here we are use automated road crossing System using Computer Vision. For this, the concept of “real time object tracking” is mainly used to detect pedestrians waiting to road crossing and the output of the project will be displayed with the help of IoT devices. Research on this technique is still ongoing. But I realized that there were some issues with some of the research. For the example, an image obtained by using image processing can detect its people in timely manner, whereas the time it takes to capture the image and the time it takes to retrieve the output and the time it takes to repeat the same process will lead us to take a slight difference between the time on the live. So it is a huge shortcoming in this research. So here I am going live with video surveillance to detect people. And many of the ingredients used in my new research and this research are very similar. 

After studying them we decided to take this research to another new dimension. As a result, I responsibly offer this new research for the benefit of all.



Software requirement specifications (SRS)


Task : Automated Road crossing system using real-time object tracking

The system have solutions for defferent partisions;

•	For pedestrian :-

	Safe pedestrian crossing
	quick respond the the pedestrian
	Feel free pedestrian crossing

•	For Vehicle :-

	Safe driving
	Reduce traffic jams
	eco friendly

Funtional and non functional requirements :-

1.	Performance reqirements :

	New technologies should be included
	Accuracy of the pedestrian detection should be good level
	The CCTV camera should be mounted proper place.
	The program must be tome colplexity
	The program must be maintainable and timely.

2.	Safety requirements :

	The program should be safe for the pedestrian and the drivers
	The material used for components of the system be weather protected.
	The camera captures must be protect human rights.



Diagrams

![classdiagram](https://github.com/Lakindu1999/ResearchPapers/assets/86758637/7610f03b-0077-4131-9373-3eb1fa2a0781)
Class Digaram of the Project

![UseCase](https://github.com/Lakindu1999/ResearchPapers/assets/86758637/6dd45652-ddd8-4466-bdf7-9a15eb82690e)
Use Case Diagram of the Project

![stateChart](https://github.com/Lakindu1999/ResearchPapers/assets/86758637/220f4acd-6340-447e-b3e2-f4d8599ed1dd)
State chart of the Project


System Design


Modularisation details

Modularization is a technique in which software system is divided into multiple discrete and independent modules, which are expected to be capable of carrying out task(s) independently. These modules may work as basic constructs for the entire software. Designers tend to design modules such that they can be executed and/or compiled separately and independently. Modular design unintentionally follows the rules of ‘divide and conquer’ problem-solving strategy this is because there are many other benefits attached with the modular design of a software.[6]

This is not just software, it is a combination of software and hardware. The System has two major blocks and each block has its own mechanism to produce the final output. The first module describes the programming part of the system, it contains HOG human detection algorithm, waiting time managing algorithm, human counting algorithm of submodules. And the Second module describes the hardware part, and it contains the pedestrian traffic light system, vehicle traffic light system, and pedestrian countdown time algorithm of submodules.



Data integrity and constraints


In Database Management Systems, integrity constraints are pre-defined set of rules that are applied on the table fields (columns) or relations to ensure that the overall validity, integrity, and consistency of the data present in the database table is maintained. Evaluation of all the conditions or rules mentioned in the integrity constraint is done every time a table insert, update, delete, or alter operation is performed. The data can be inserted, updated, deleted, or altered only if the result of the constraint comes out to be True. Thus, integrity constraints are useful in preventing any accidental damage to the database by an authorized user.[7]

OpenCV ships with a pre-trained HOG + Linear SVM model that can be used to perform pedestrian detection in both images and video streams.[8] First, we make a call to hog = cv2.HOGDescriptor() which initializes the Histogram of Oriented Gradients descriptor. Then, we call the setSVMDetector to set the Support Vector Machine to be pre-trained pedestrian detector, loaded via the cv2.HOGDescriptor_getDefaultPeopleDetector() function. That predefined function includes dataset of the millions of humans, Pedestrians and its trained very well.

![Block-diagram-of-the-human-detection-system-using-HOG](https://github.com/Lakindu1999/ResearchPapers/assets/86758637/56856955-844f-48ab-bd52-6a423897277b)
Block diagram of the human detection system



User Interface Design


User interface is the front-end application view to which user interacts in order to use the software. User can manipulate and control the software as well as hardware by means of user interface. Today, user interface is found at almost every place where digital technology exists, right from computers, mobile phones, cars, music players, airplanes, ships etc.

User interface is part of software and is designed such a way that it is expected to provide the user insight of the software. UI provides fundamental platform for human-computer interaction. UI can be graphical, text-based, audio-video based, depending upon the underlying hardware and software combination. UI can be hardware or software or a combination of both.[10]

UI is broadly divided into two categories:
•	Command Line Interface
•	Graphical User Interface

Here we are using a graphical user interface(GUI). This allows the viewer to output the live video captured by the camera to the computer. Also, pedestrians are shown a waiting time and a countdown time by a character display.

![ss01](https://github.com/Lakindu1999/ResearchPapers/assets/86758637/ec3cb0f3-751f-4c0e-b60f-28c583ca7d0a)
Example of GUI Interface of the project

![H0f20be399c96479ca1d95796f554b44e3](https://github.com/Lakindu1999/ResearchPapers/assets/86758637/72ead3cf-4269-407d-8592-7603e4440a11)
16 X 2 Character Display


Coding

Comments and Description

Comments are text notes added to the program to provide explanatory information about the source code. They are used in a programming language to document the program and remind programmers of what tricky things they just did with the code and also helps the later generation for understanding and maintenance of code. The compiler considers these as non-executable statements. Different programming language uses a different way of including the comments in the source code.[11]


Error handling

Error in Python can be of two types i.e. Syntax errors and Exceptions. Errors are the problems in a program due to which the program will stop the execution. On the other hand, exceptions are raised when some internal events occur which changes the normal flow of the program.[12]

Syntax Error: As the name suggests this error is caused by the wrong syntax in the code. It leads to the termination of the program.
While we were working on this project, we encountered a large syntax errors, for example, not importing the package, not using the pre-defined functions correctly, incorrect loops and handling a large number of conditions. We checked them line by line one by one and built the correct final research. 

Exceptions: Exceptions are raised when the program is syntactically correct, but the code resulted in an error. This error does not stop the execution of the program, however, it changes the normal flow of the program.

![image](https://github.com/Lakindu1999/ResearchPapers/assets/86758637/fa7859d3-46a7-4903-ae63-ab6e6834a449)
Exception Handling



Parameters calling/passing

Parameter passing involves passing input parameters into a module and receiving output parameters back from the module.

Developers jumping into Python programming from other languages like C++ and Java are often confused by the process of passing arguments in Python. The object-centric data model and its treatment of assignment is the cause behind the confusion at the fundamental level. Python’s argument passing model is neither “Pass by Value” nor “Pass by Reference” but it is “Pass by Object Reference”.[13]

We have used many functions in this project. In some cases, a few parameters are used as an argument and a few parameters as a return type. A special feature of Python is ability to set multiple return type parameters at once. This will be a huge contribution to our project.

![image](https://github.com/Lakindu1999/ResearchPapers/assets/86758637/85dba4be-e7d7-4e3a-8c98-d8b5b93a23fb)
Project argument example

![image](https://github.com/Lakindu1999/ResearchPapers/assets/86758637/b7aa0c29-4ace-44c4-a34f-af121317eb36)
Multiple return type example



 System Security measures

Database/data security 

In our project the project affects to the real-life daily problem. It means the project all about pedestrian crossing. Only we have datasets for training and give predictions to the system. Then for that purpose we want huge amount of data to get accurate output of the project, the data are store at the H.O.G algorithm. HOG algorithm get access for that data and compare the live detection image with trained data and give the output of the prediction and check if it is true or false with the algorithm. The dataset was encoded to coordinates for better and fast performance and it may affect to the security of the dataset.


Creation of User profiles and access rights

The main purpose of our project use for police of the country. In that project there have no user profiles. Only there have system display interface and that system access are can be used for that the system are owned company or organization.

![image](https://github.com/Lakindu1999/ResearchPapers/assets/86758637/76e65a67-9b2f-425d-b5f2-55acd8779475)
User Interface of the Project


Reports and screen
![image](https://github.com/Lakindu1999/ResearchPapers/assets/86758637/7bf28f29-cb16-411b-9811-b0209c3c63ea)
Upper view of the Project

![image](https://github.com/Lakindu1999/ResearchPapers/assets/86758637/ed0e9972-668a-45fa-a9f3-8df49e36aa5b)
Side view of the Project

![image](https://github.com/Lakindu1999/ResearchPapers/assets/86758637/167cfd72-666f-4f83-955e-c2e8791aa872)
Pedestrian detecting

![image](https://github.com/Lakindu1999/ResearchPapers/assets/86758637/60b497f4-7784-4dd1-a50a-31da0e1ed8a2)
Countdown time counting

![image](https://github.com/Lakindu1999/ResearchPapers/assets/86758637/89f35aed-6ca6-42ec-a5f2-51837328215b)
Waiting time counting

![image](https://github.com/Lakindu1999/ResearchPapers/assets/86758637/37a9cd5d-a476-4822-a922-ee3586ead60f)
People cross the road

![image](https://github.com/Lakindu1999/ResearchPapers/assets/86758637/5786cc22-49e2-4a53-8057-5bfefab65220)
Waiting the pedestrian command in lcd display

![image](https://github.com/Lakindu1999/ResearchPapers/assets/86758637/ec7999c9-a656-448e-abc2-e1a30879b65e)
Waiting time calculate in lcd display

![image](https://github.com/Lakindu1999/ResearchPapers/assets/86758637/d1a8cada-2bfd-4d49-b1b2-6a20f7318df8)
Countdown time calculate in lcd display



Future scope and further enhancement of the Project

This model can be developed to reduce traffic as well. We can develop this model to take random samples of vehicles that were on the road at that time and store their speed. If sample vehicles have speed beneath a particular speed level our model determine that there’s traffic and if vehicles from the sample maintains a speed above the speed level this model determines that there is less or no traffic at the road and according to that decision, we can construct the algorithm for pedestrian crossing if no traffic people can cross the road many times(small time period) otherwise we give the road to crossing after few times(some big time people waiting to road crossing). Using that new future scope, we can reduce the traffic congestion.

Motorbikes and other small vehicles are careless about people who are crossing the road and we can detect and recognize vehicle license plate from a video in real time and take legal actions against them.

Modifying and install with new features to this model we can track the speed of every vehicle pass out the pedestrian crossing with the help of the CCTV camera. the main purpose of that feature is to track the high speed of the vehicle and notify the traffic police stand after the road crossing.


Assumptions

we have to assume that the recorded video has to be considered as the live video since it’s a simulation and I have used a video clip from a live streaming of a crowded street in Japan to create a scenario.

I have assumed that pedestrian count will be 4 and countdown time is 20 seconds, So that when 4 pedestrian are detected, waiting and countdown time(20 seconds) will be displayed consecutively. 

I have taken 50 seconds and 100 seconds as next - call - time but it will depend on the crowd of a particular city or a particular crossing and traffic conditions.

![image](https://github.com/Lakindu1999/ResearchPapers/assets/86758637/bc0a9d64-d98d-41f5-88e1-73a4f6fb83d2)
Assumptions

![image](https://github.com/Lakindu1999/ResearchPapers/assets/86758637/ef5dc9ec-97f9-4d2a-8dec-6141bbee9f23)
Assumptions


Bibliography / References

[1]	] Shraddha, K. Walikar, A. Kumar, ] Pg, and ] Principal, “Computer Vision: Pedestrian Detection image processing algorithm for Traffic light system”.
[2]	“[IJET V2I3P6] Authors: Ajeeth, Sandhya raani M.” https://dokumen.tips/engineering/ijet-v2i3p6-authors-ajeeth-sandhya-raani-m.html (accessed May 06, 2022).
[3]	C. O. Manlises, J. M. Martinez, J. L. Belenzo, C. K. Perez, and M. K. T. A. Postrero, “Real-time integrated CCTV using face and pedestrian detection image processing algorithm for automatic traffic light transitions,” 8th International Conference on Humanoid, Nanotechnology, Information Technology, Communication and Control, Environment and Management, HNICEM 2015, Jan. 2016, doi: 10.1109/HNICEM.2015.7393205.
[4]	“Software Engineering Paradigms And Models Information Technology Essay.” https://www.uniassignment.com/essay-samples/information-technology/software-engineering-paradigms-and-models-information-technology-essay.php (accessed May 06, 2022).
[5]	“Software Engineering | Iterative Waterfall Model - GeeksforGeeks.” https://www.geeksforgeeks.org/software-engineering-iterative-waterfall-model/ (accessed May 06, 2022).
[6]	“Software Design Basics.” https://www.tutorialspoint.com/software_engineering/software_design_basics.htm (accessed May 06, 2022).
[7]	“Integrity Constraints in DBMS - Scaler Topics.” https://www.scaler.com/topics/dbms/integrity-constraints-in-dbms/ (accessed May 06, 2022).
[8]	“Pedestrian Detection OpenCV - PyImageSearch.” https://pyimagesearch.com/2015/11/09/pedestrian-detection-opencv/ (accessed May 06, 2022).
[9]	“OpenCV HOG Hyperparameter Tuning for Accurate and Fast Person Detection.” https://debuggercafe.com/opencv-hog-hyperparameter-tuning-for-accurate-and-fast-person-detection/ (accessed May 06, 2022).
[10]	“Software User Interface Design.” https://www.tutorialspoint.com/software_engineering/software_user_interface_design.htm (accessed May 06, 2022).
[11]	“Concept of Comments in Computer Programming - GeeksforGeeks.” https://www.geeksforgeeks.org/concept-of-comments-in-computer-programming/ (accessed May 06, 2022).
[12]	“Python Exception Handling - GeeksforGeeks.” https://www.geeksforgeeks.org/python-exception-handling/ (accessed May 06, 2022).
[13]	“Pass by reference vs value in Python - GeeksforGeeks.” https://www.geeksforgeeks.org/pass-by-reference-vs-value-in-python/ (accessed May 06, 2022).
[14]	“Data Validation - Overview, Types, Practical Examples.” https://corporatefinanceinstitute.com/resources/knowledge/data-analysis/data-validation/ (accessed May 06, 2022).
[15]	“HOG (Histogram of Oriented Gradients): An Overview | by Mrinal Tyagi | Towards Data Science.” https://towardsdatascience.com/hog-histogram-of-oriented-gradients-67ecd887675f (accessed May 06, 2022).
[16]	“Software Testing Methodologies.” https://smartbear.com/learn/automated-testing/software-testing-methodologies/ (accessed May 06, 2022).
[17]	“The process of detecting and removing of existing and potential error called as bugs in a software - Brainly.in.” https://brainly.in/question/28009187 (accessed May 06, 2022).
 
