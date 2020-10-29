## STUDENT ATTENDANCE USING FACIAL RECOGNITION SYSTEM 

***###This is an automatic student attendance system using face recognition. The aim is to automate the process of attendance maintenance.


## FACE RECOGNITION 

Face recognition is a biometric recognition technique.
Biometric recognition is an information system that allows the identification of a person based on some of its main physiological and behavioral characteristics.
Face recognition is a broad problem of identifying or verifying people in photographs and videos, a process comprised of detection, alignment, feature extraction, and a recognition task
It has 4 steps which are :
1. **Face Detection** 
2. **Data Gathering**
3. **Data Comparison**
4. **Face Recognition** 


## TECHONLOGY USED

* [OPENCV](https://opencv.org/about/)

* [TKINTER](https://docs.python.org/3/library/tkinter.html)

* [HAAR-CASCADE CLASSIFIER](https://docs.opencv.org/3.4/db/d28/tutorial_cascade_classifier.html)

* [LocalBinaryPatternHistogram (LBPH) recognizer](https://docs.opencv.org/master/df/d25/classcv_1_1face_1_1LBPHFaceRecognizer.html)

* [trainner.yml](https://docs.opencv.org/master/dd/d65/classcv_1_1face_1_1FaceRecognizer.html)

* [PIL](https://pillow.readthedocs.io/en/stable/)


## HOW THE SYSTEM WORKS?

1. **DATA COLLECTION**:
<br>

![capture](https://github.com/memudualimatou/STUDENT-ATTENDANCE-USING-FACIAL-RECOGNITION-SYSTEM-OPENCV/blob/master/Docs/Images/Capture12.PNG =250x250)




The student interact with the system through the graphical user interface(GUI) above.
The first step the student has to enter his details(Name and ID) this details will be stored in a csv file **'StudentDetailss.csv'**, the ID is Matric Number on the GUI.
second step, the student will click on the **CAPTURE IMAGE** button to capture his faces, here 50pictures of the student will be taken and stored in the **TrainingImages** Folder.  The **haar-cascadeclassifier** file to detect faces through the video stream while the student face is being captured.
the notification board will print ou the student details after a succesfull data collection.


<br>

![capture2](https://github.com/memudualimatou/STUDENT-ATTENDANCE-USING-FACIAL-RECOGNITION-SYSTEM-OPENCV/blob/master/Docs/Images/555.PNG =250x250)


***
2. **IMAGE TRAINED**

The student has to click on the  **TRAIN IMAGE** button which will link his details, face features to the **LBPHrecognizer** to ease further face recognition,
the recognizer will save the face features in the **trainner.yml** and "IMAGE TRAINED" will be printed on the GUI notification board after a successfull linkage.

***
3. **FACE TRACKING**

The student has to click on the **TRACK IMAGE** button to allow the face recognizer to track his face through a video stream, when trhe system successfully recognize the student face, his details will show and "ATTENDANCE UPDATED" will be printed out otherwise , the ID will be Unkown and "ID UNKOWN, ATTENDANCE NOT UPDATED" will be printed out.
Simustenously, a csv file **AttendanceFile.csv'** will be updated with the ID,NAME of the student and DATE Aand TIME at which his face has recognized.
the Unkown face captured will be store in the **UnkownImages** folder.<br>


![capture3](https://github.com/memudualimatou/STUDENT-ATTENDANCE-USING-FACIAL-RECOGNITION-SYSTEM-OPENCV/blob/master/Docs/Images/ezgif.com-gif-maker%20(1).gif)

***
## SYSTEM REQUIREMENT

1. OpenCV-contrib-python  version:4.2.0.34
2. TkInter version:8.6
3. PIL version:7.0.0


check this link to view the trainner file.
https://bitbucket.org/memudu_alimatou/facial-recognition-opencv/src/master/

