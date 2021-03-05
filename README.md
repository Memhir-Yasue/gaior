<img width="1158" alt="GAIORHEAD" src="https://user-images.githubusercontent.com/39225610/109847278-fe299a80-7c1c-11eb-890b-5121f00f3491.png">


![AIplays](https://user-images.githubusercontent.com/39225610/109858312-a7768d80-7c29-11eb-9a89-da5681c2422f.gif)





## Project Abstract
GAIOR (Game Agnostic Input-Output Register) is a software application that will empower gamers and enthusiasts to be able to train a machine learning model to play any computer game. While the user is playing a game of their choice, GAIOR, on the backend, will continuously collect data from the monitor and keystrokes and will preprocess, and store this data. After enough samples have been taken, an AI model can then be generated that will be able to play the game - live!

## Conceptual Design
The first step in any machine learning project is data collection and data preprocessing. When it comes to training an AI to play a video game, most people had to write their own scripts to capture the screen and joystick/keyboard input. This adds an unnecessary hurdle for those who simply wish to see an AI play a video game. The goal of this project is to eliminate this hurdle by providing the user with software that's ready _out-of-the-box_ - that is, all that a user would have to do is turn GAIOR on and start playing their favorite video-game. In the backend, GAIOR will collect and preprocess 20+ frames per second and map each of them to the correct keystroke pressed at that instance of time. This data will be represented as a one-hot-encoding and will be stored either on a database either on the local machine or on the cloud. Later, the data can be retrieved to train an ML model which can play the video-game. We'll utilize Java or C++ or Python to create the keylogger and screen capturing component, and Python w/ OpenCV, Pandas, and Numpy to process the data. 

In short, we'll create
- A screen capture and keylogger
- A database (probably MySQL)
- An API to connect to a cloud storage service (Like Amazon S3, EBS, GCP Cloud Storage, ... etc)
- A desktop GUI interface for the user to start the recorder, fields for connecting to the database or cloud storage
