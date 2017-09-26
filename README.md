# ArDrone
This is a basic tutorial to use a Parrot ArDrone 2.0 (from now Drone) with Pharo and LRP. These instructions require a basic understanding of Pharo.

### Pharo image
To start using the Drone with Pharo and LRP, you need to download a clean image from the [download](https://pharo.org/web/download) page of Pharo.

### Installation
* After downloading the image of Pharo, you need to install the LRP in your image, do-it-and-go the following script in a playground window:

  ```pharo
  Gofer it
    smalltalkhubUser: 'jfabry' project: 'LiveRobotProgramming';
    configuration;
    loadDevelopment
  ```
  
* Now, with LRP installed, you have to download the Drone API to Pharo. The source can be merged to the current image using Monticello browser, the package is available in this link from smalltalkhub: [http://smalltalkhub.com/#!/~CaroHernandez/ArDronePharo](http://smalltalkhub.com/#!/~CaroHernandez/ArDronePharo) (you may need to reload this page a few times). If you don't know how to download code from smalltalkhub or how to use the Monticello browser, you can read chapter 8 from the book [Pharo by Examples](http://files.pharo.org/books/updated-pharo-by-example/). The following image has the required package selected on the right: 

![monticello browser Drone-API](/img/PharoAPIDroneInstallation.png)

  Remember to load **ONLY** the last version of the package!. 

* After loading the API, you must load the bridge to connect the LRP with the Drone API. The code is in smalltalkhub again, you have to load the following link with Monticello browser: [http://smalltalkhub.com/#!/~CaroHernandez/LiveRobotics-ARDrone](http://smalltalkhub.com/#!/~CaroHernandez/LiveRobotics-ARDrone). And again you have to load the last version, like this image shows: 

![monticello browser bridge](/img/PharoBridgeLRP-ArDrone.png)

* Now that you have installed the Drone API, the LRP and the bridge between them, if you do a left click in the world of Pharo, you will see the following:

![lrp in pharo world menu](/img/PharoWorldMenu.png)

### Usage

You have completed all the installation steps. Now you can fly your Drone following the next short steps:

* Turn on your Drone and then connect to the Drone's wifi.
* Open Live Robot Programming in the Pharo world menu and you will see the following:
![LRP drone connect](/img/LRPDroneConnection.png)
* Click the Connect Button (it's necessary be connected to the Drone's wifi).
* If all is good, you will see a green circle and the battery level.
* Now you can click in the button **Take off** and the Drone will start flying. It's very important to have enough space for the drone to fly, if the Drone fails or was already damaged it can be dangerous.
* Also you have the LRP UI, in this UI you can create state machines for the Drone. In this [link](https://github.com/carolahp/ARDroneLRP-Tests) you have some examples to test. The tag follower examples don't work, because they were create to be used on a older version of the API. 

And that's all!, now you can fly your Drone with Pharo and LRP, and also create and modify state machines for the Drone.

**Important:** The video feature is not implemented in this tutorial so you will not see the drone camera, but it's coming on a next version!
