<!-- --- -->
<!--  title: 'Vision-based-sintering-parameters-reading-system' -->
<!-- --- -->

# **Vision-based sintering parameters reading system**

* Developed with Raspbian, OpenCV, scikit-learn, etc.
* Allow temperature reading & electric current reading.
* The SVM classifier trained by 12000 seven-segment digit images is [available](#Usage-of-classifier). 

<br>


## **Overview** 

### Installation

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<img src="https://i.imgur.com/Q4dpbUT.png" width="">


### User flow

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<img src="https://i.imgur.com/REH1HVo.png" width="">


<br>

## **Pre-settings**

Set up parameters for temperature reading & electric current reading.

<br>

### **Temperature reading**

- Localize the meter & obtain meter image by a perspective cropping.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<img src="https://i.imgur.com/MPOmwwD.png" width="">

- Determine the size, quantity, and location of interested digits.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<img src="https://i.imgur.com/lIpB4gI.png" width="">



<br>

### **Electric current reading**

- Localize the meter & obtain meter image by a perspective cropping.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<img src="https://i.imgur.com/lgXTYkc.png" width="">


- Localize the scales & determine the amperage between scales.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<img src="https://i.imgur.com/LxBMF5q.png" width="">




<br>

## **Vision-based sintering parameters reading** 
<!-- ## **Features**  -->



### **Temperature reading**

- Read temperature value of the sintering furnace.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<img src="https://i.imgur.com/eWPFPiS.png" width="">


### **Electric current reading**

- Read current value of the sintering furnace.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<img src="https://i.imgur.com/NUbuGvi.png" width="">


<br>


## **Demo video** 

* [Demo影片(中文)](https://www.youtube.com/watch?v=seJtVJjiknA)


## **Usage of classifier**

- **Step1**: Use following command to install required packages

        pip install scikit-learn==0.22 scikit-image==0.14.2 numpy==1.17.4

- **Step2**: Run the script with image path to get recognized digit

        python recognize_single_digit.py digit5.jpg



<br>

<!-- ## **Reference**

### **Navigation Drawer**
- https://www.tpisoftware.com/tpu/articleDetails/655
- https://spicyboyd.blogspot.com/2018/04/appandroidnavigation-drawer.html
- http://blog.tonycube.com/2014/02/android-navigation-drawer-1.html -->


## **Contact** 

* Contact me at jerming0515@gmail.com for complete source code.



<!-- <style>
.blue {
  color: blue;
}
.red {
  color: red;
}
</style> -->