# This describes how to integrate web services in a BPM

[Back to Table of Contents](Table_Of_Contents.md)

## Integrating web services ##

1. Create a new Integration Service (Eg. Fahrenheit to Celsius. )

![http://imgur.com/7rWaFuD.png](http://imgur.com/7rWaFuD.png)

2. Edit the implementation of the service. For this example we are using an already existing WSDL service (http://www.w3schools.com/webservices/tempconvert.asmx?WSDL).

![http://imgur.com/rghf2Ao.png](http://imgur.com/rghf2Ao.png)


Click:

Discover: To verify the URL is working and connecting to.

View: To view the WSDL.

Generate Types: To view the types of values that can be generated from WSDL.


3. Design an User Interface- Human Service using the integration service designed in the previous step.


![http://imgur.com/AivIU7Q.png](http://imgur.com/AivIU7Q.png)


4. Design a Business process to use the User Interface defined in the previous step.

![http://imgur.com/lGOHsLE.png](http://imgur.com/lGOHsLE.png)


5. Execute the process:

![http://imgur.com/7ThYEJj.png](http://imgur.com/7ThYEJj.png)



![http://imgur.com/7dZnHTZ.png](http://imgur.com/7dZnHTZ.png)