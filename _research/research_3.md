---
layout: research_layout
name: Indraprastha Institute of Information Technology, New Delhi, India
description: I am scheduled to work with <a href="https://www.iiitd.edu.in/~anands/">Dr. Saket Anand</a> in the field of autonomous robotics from december till june 2016.
---

I am working as a research assistant in Dr. Saket Anand's group at Indraprastha Institute of Information Technology, Delhi on autonomous robotics for 5-6 months. We are one of the 13 teams cut down from 259 initially competing in the <a href="http://www.sparktherise.com/program-detail/driverless-car-challenge">"Spark For Rise"</a> driverless car challenge initiated by Mahindra. The objective of this competition is to revolutionise driving on the streets of India with the thinking that if autonomous cars can run on Indian roads, they can run on any road in the world.  

Our team is called <a href="https://www.facebook.com/swarathatiiitd">"Swarath"</a>. We are a mix of faculty and students from IIIT-Delhi, who together have expertise in vision, robotics, embedded systems, sensing, and communications. Our ultimate goal is to launch autonomous shuttles that provide anytime last mile connectivity in Indian cities.  


Additionally, I am auditing CSE 222: Algorithms Design and Analysis taught by <a href="https://www.iiitd.ac.in/rajiv"> Dr. Rajiv Raman</a>.

<iframe width="480" height="385" src="https://www.youtube.com/embed/KvLOf7OfSc4" frameborder="0" allowfullscreen></iframe>


###***UPDATES***:

#### First Week!  

So I started off my first week by spending some time familiarizing myself with ROS. ROS is Robot Operating System and is used to interface multiple nodes with each other. This is done by communicating asynchronously through topics or synchronously through services. A node is basically an executable that sends information via messages. One node publishes messages to a topic and another node subscribes to that message. This is how information is transmitted.  

For example, a light sensor can be interfaced as one node and motors can be interfaced as another node. Data can be streamed through the sensors, published to a topic and subscribed by the motors.  

#### Second Week!

One of our team members Shubham, from IIT Kanpur, wrote an OpenCV code to detect bunches of lines from an image using the hough transform for the lane detection algorithm. He additionally wrote a function to remove clusters.  

Using Shubham's code, I implemented a ROS uvc_Camera_node (Publisher) that publishes a live video feed to the default topic camera/image_raw. Next I wrote a c++ source code to implement a subscriber that receives the images sent by the uvc_camera_node and in turn publishes the processed images to another custom built topic camera/image_processed. I embedded Shubhams code in this source code.  

I followed this tutorial to set up my ROS nodes. <a href="https://siddhantahuja.wordpress.com/2011/07/20/working-with-ros-and-opencv-draft/">Sid's Blog</a> 

Also, my classes in CSE 222 is going wonderfully. This week, we studied about proofs- the proof by contradiction and the proof by induction. 
