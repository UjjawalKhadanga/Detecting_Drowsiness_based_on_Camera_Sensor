# Detecting_Drowsiness_based_on_Camera_Sensor

Fatigue is a safety problem that has not yet been deeply tackled mainly because of its nature. Fatigue, in general, is very difficult to measure or observe unlike alcohol and drugs, which have clear key indicators and tests that are available easily. Probably, the best solutions to this problem are awareness about fatigue-related accidents and promoting drivers to admit fatigue when needed. The former is hard and much more expensive to achieve, and the latter is not possible without the former as driving for long hours is very lucrative.

So, to tackle this problem, we have made an application which uses a camera sensor to take snaps of a driver driving a vehicle and gives him/her an alert signal in the real time. This application detects drowsiness of a driver based on the eye aspect ratio and whenever this ratio goes below some certain threshold, application gives an alerting sound.

![image](https://user-images.githubusercontent.com/79044490/202811431-77a6fa76-693d-4a55-aa3c-16ededd10d11.png)

There are many products out there that provide the measure of fatigue level in the drivers which are implemented in many vehicles. The driver drowsiness detection system provides the similar functionality but with better results and additional benefits. Also, it alerts the user on reaching a certain saturation point of the drowsiness measure.

## Hardware Requirements
WEBCAM and LAPTOP with basic hardware


## Features of Application

This application detects drowsiness of a driver based on the eye aspect ratio and whenever this ratio goes below some certain threshold, application gives an alerting sound. So, our application is supposed to work in such a way that a user can register and login such that the system can determine the base eye-aspect-ratio of a person signed-in (as the eye aspect ratio for alertness and drowsiness depends on person to person).

Here are the features of our application tested by our team members showing different aspects of the Drowsiness Detection System:

1.	Home Page: It has several pages which includes Home, Sign-up, Login, Warnings and Know more.

![1](https://user-images.githubusercontent.com/79044490/202721074-288ebc3c-f494-4fcf-96f9-4e794bd5183c.png)

2.	Overview of Sign-up/Login page for user: When a user signs up for the first time, he/she must take his/her snap in the camera so that the eye aspect ratio of that can be saved in the database for future reference when that person comes afterwards.

![4](https://user-images.githubusercontent.com/79044490/202721207-f6be1737-4ed7-4c77-957f-5adbaed6f601.png)
![3](https://user-images.githubusercontent.com/79044490/202721166-f35ad40f-dc3e-4b89-82b0-f82b1b54a4be.png)

After successful sign-up, user has to login into the system, and must select the STRART/STOP check box to start the process.

![7](https://user-images.githubusercontent.com/79044490/202721298-b68df2be-a20c-43b9-a004-813bb97aedb3.png)

3.	Whenever a user feels drowsy or sleepy, the camera detects by capturing the eye aspect ratio, that is, whenever user’s eyes close greater than 70% of size of user’s eyes for more than 30 seconds, the buzzer will start buzzing.

![8](https://user-images.githubusercontent.com/79044490/202721321-93087610-f67b-47a7-a955-974742619132.png)

4.	Whenever the alerting/buzzer sound is played, entry for time, e and Username is filled in Warning page. Later, if user wants to see the time of warnings, the user can go to warning page and can find time, date of every warning of a user.

![9](https://user-images.githubusercontent.com/79044490/202721343-3d4971ea-d7c3-468c-bc72-005fbf9e0bff.png)
![10](https://user-images.githubusercontent.com/79044490/202721371-8e731d9f-3e41-42e5-961d-9ee3534e3605.png)

 
 ## Requirements
 
IMPORTANT

    dlib==19.24.0
    imutils==0.5.3
    numpy==1.18.5
    opencv_python==4.3.0.36
    pandas==1.0.5
    Pillow==9.3.0
    pygame==2.1.2
    scipy==1.5.1
    streamlit==1.9.2

Use `pip install -r requirements.txt`to install the given requirements.

![image](https://user-images.githubusercontent.com/79044490/202812172-41c62f89-ed68-42da-9300-1f1fdc609a23.png)


## Usage

### Drowsiness Detection
Run script using:

    streamlit run drowsiness_detect.py
