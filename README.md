# ArDrone
This is a basic tutorial to use a Parrot ArDrone 2.0 (from now Drone) with Pharo and LRP. You need a basic level about Pharo to undestand some instructions.

### Pharo image
To start using the Drone with Pharo and LRP, you need to download a clean image from [download](https://pharo.org/web/download) page of Pharo.

### Installation
* After download the image of Pharo, you need to install the LRP in your image, do-it of the following in a playground window:

  ```pharo
  Gofer it
    smalltalkhubUser: 'jfabry' project: 'LiveRobotProgramming';
    configuration;
    loadDevelopment
  ```
  
* Now, with LRP installed, you have to download the Drone API to Pharo. The source can be merged to the current image using monticello browser, the package is allowed in this link from smalltalkhub: [http://smalltalkhub.com/#!/~CaroHernandez/ArDronePharo](http://smalltalkhub.com/#!/~CaroHernandez/ArDronePharo). If you don't know how download code from smalltalkhub or use monticello browser, you can read the chapter 8 from the book [Pharo by Examples](http://files.pharo.org/books/updated-pharo-by-example/). The following image, shows the code that you need to load in your image: 

![monticello browser Drone-API](/img/PharoAPIDroneInstallation.png)

  Remember load **ONLY** the last version of package!. 

* After loaded the API, you must load the bridge to connect the LRP with the Drone API. The code is in smalltalkhub, again you have to load with monticello browser this link: [http://smalltalkhub.com/#!/~CaroHernandez/LiveRobotics-ARDrone](http://smalltalkhub.com/#!/~CaroHernandez/LiveRobotics-ARDrone). And again you have to load the last, how shows the image: 

![monticello browser bridge](/img/PharoBridgeLRP-ArDrone.png)

* Now you have installed the Drone API, the LRP and the bridge between them so if you make a left click in the world of Pharo, you will see the following:

![lrp in pharo world menu](/img/PharoWorldMenu.png)

### Usage

Ok, you have pass all the installation steps so now you can flight your Drone following the next short steps:

* Turn on your Drone and then connect to the Drone's wifi.
* Open Live Robot Programming in the Pharo world menu and you will see the following image :
![LRP drone connect](/img/LRPDroneConnection.png)
* Click in Connect Button (It's necessary be connected to the Drone's wifi).
* If all is good, you will see a green circle and the battery level.
* Now you can click in the button **Take off** and the Drone starts to flight. It's very important have a medium place to flight because if the Drone had damage, can be dangerous in a small place. 
* Also you have the LRP UI, in this UI you can create state machines for the Drone. In this [Link](https://github.com/carolahp/ARDroneLRP-Tests) you have some examples to test, but the tag follower examples don't work, because they were create to used on a old version of API. 

And that is all!, now you can flight your Drone with Pharo and LRP, create and modify state machines for the Drone.

**Important:** The video feature is not implemented in this tutorial so you will not see the drone camera , we are working to implemented!
