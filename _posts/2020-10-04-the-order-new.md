---
title: The Order New
sub-title: Yeah! Let's Do This
author: Angga
date: 2020-10-04 16:00:00 +0000
feature-img: "/uploads/gnvk6tmrjxzultxc9qblha-1.jpg"
layout: post
categories: ayam

---
Next, begin to enter the parameters of your load test. In this example we will have 10 virtual users access StackOverflow. We have a 3 second ramp-up-time, a minimum delay of 500 ms, and a maximum delay of 10,000 ms:

Below is a description of the primary fields in the simple test setup.

* **URL** – This is the full URL of the page you wish to load test. This should include the URL scheme (e.g. http:// or https://). For example, http://www.stackoverflow.com
* **Number of Users** – This is the number of users that will be simulated. Let’s use 10 so we use the a RedLine13 server. 10 processes will be started to simulate visitors to the URL provided.
* **Iterations Per User** – This is the number of times each user will visit the URL. This is useful in simulating page refreshes. In this case, each user may have cached versions of resources (i.e. images, stylesheets, scripts, etc.) that are found on the page. Let’s use the default of 1 so we can use a free RedLine13 server. Note: this is the primary difference between running a 100 user test with a single iteration and a 10 user test with 10 iterations.
* **Ramp Up Time** – It evenly distributes the start time of each test over the interval. After that delay, it starts the test, at which point another delay will be introduced based on the min/max delay setting before loading the first URL. Let’s set to 3 seconds.
* **Minimum Delay** – This sets the minimum delay _in milliseconds (1/1000th of a second)_ that will be simulated per user before each request of the URL. Let use 500 milliseconds.
* **Maximum Delay** – This sets the maximum delay _in milliseconds_ that will be simulated per user before each request of the URL. Let’s use the default of 10,000.