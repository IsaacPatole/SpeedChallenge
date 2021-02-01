# SpeedChallenge
Comma.ai speed challenge

The goal of this challenge is to predict the speed of a vehicle based on just a dash-cam input. 
You can dowload the dataset from here: https://github.com/commaai/speedchallenge

Speed can be calculated by the distance covered by the vehicle in a particular time. In our case we have frames and their corresponding speed in the text file.
In order to calculate the distance we need to know the difference between any n consecutive frames. 

Have a look at this blog to understand it better: https://medium.com/weightsandbiases/predicting-vehicle-speed-from-dashcam-video-f6158054f6fd

My goal was to implement the architecture given above in Pytorch and run it in Google colab. 

In order to run the code: 
1) Create the folder in Google colab, upload the videos and .txt file and clone all my codes in it.
2) Run car_speed_data_prep.ipynb to extract frames from the video and create a csv file in the format of frame_location-index-speed
3) pytorch_speed_nn.ipynb is the architecture defined by the above article.
4) I have created another architecture in addition to the architecture above. In addition to the Optical-Flow I've also added difference between two frames in the network in order to make it understand more representation of the data, have a look at pytorch_speed_nn2.ipynb
5) I have created a code so that you can test the model on the test video and save the output in the txt file.



Special thanks to Comma.ai for the challenge, also to Joval Sardinha for helping me getting started through his article.












