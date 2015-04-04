# Introduction #

Test harness can be created in BPM inorder to test individual processes or services. Using Test harness, inputs to the process/service can be simulated. This allows individual pieces of the process to be tested independently while other areas of the process are still under development. In other words, test harness can be used to unit test a process or a service.


Here is an example to create one for the process:

Step 1: Let us consider 'ED Process of Patient Care' process. This process begins by welcoming the patient. This is followed by Conduct Initial Consult, Process Test Order Requests, FollowUp Consultations, Transporting the patient out of ED.
![http://i.imgur.com/dwFdZJU.jpg](http://i.imgur.com/dwFdZJU.jpg)

We will build a test harness for:Conduct Initial Consult.

Make a copy of 'Conduct Initial Consult' process. Under the process tab, select 'Conduct Initial Consult'. Right click on the process.
![http://i.imgur.com/Xu7tZUr.jpg](http://i.imgur.com/Xu7tZUr.jpg)

Step 2: Delete all the processes and services between the start and end points.

Add an Init script and pull the original conduct Initial Consultation process into this new process.

![http://i.imgur.com/30TL0Xr.jpg](http://i.imgur.com/30TL0Xr.jpg)

Step 3:
Initialize all the input variables under the Implementation section of the init script as seen in the screenshot:
![http://i.imgur.com/K7zXWPP.jpg](http://i.imgur.com/K7zXWPP.jpg)


(needs completion ! )
