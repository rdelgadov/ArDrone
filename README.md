# ArDrone
Tutorial to use a Parrot ArDrone 2.0 with Pharo and LRP. 

### Initialization
To start using the Parrot ArDrone 2.0 with Pharo and LRP, you need to download a clean image from [download](https://pharo.org/web/download) page of Pharo.

### Installation
* After download the image of Pharo, you need to install the LRP in your image, do-it of the following in a playground window:

  ```pharo
  Gofer it
    smalltalkhubUser: 'jfabry' project: 'LiveRobotProgramming';
    configuration;
    loadDevelopment
  ```
* Now, with LRP installed, you have to download the ArDrone API to Pharo. The source can be merged to the current image using monticello browser, the package is allowed in this [link from smalltalkhub](http://smalltalkhub.com/#!/~CaroHernandez/ArDronePharo). If you don't know how download code from smalltalkhub or use monticello browser, you can read the chapter 8 from the book [Pharo by Examples](http://files.pharo.org/books/updated-pharo-by-example/).

* After merged
