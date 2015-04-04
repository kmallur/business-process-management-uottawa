# This describes how to integrate web services in BPM
(Alpha version- By Kavya )

[Back to Table of Contents](Table_Of_Contents.md)

## Integrating web services ##

1. Create a new Integration Service from 'Implementation' section. Click on '+' to see the options available. Click on 'Integration Service'. Call it as shown below:

![http://i.imgur.com/FnMiqlA.jpg](http://i.imgur.com/FnMiqlA.jpg)

2. The user is now taken to the Integration Service screen. From the pallet on the right hand side of the screen, drag and drop 'Web Service Integration' between the start and end points as shown below. Name the service and connect to the start and end points.

![http://i.imgur.com/0CjM6QK.jpg](http://i.imgur.com/0CjM6QK.jpg)

3. Select the service added in step2 and goto 'Implementation section'. Click on 'Discover' button seen next to the WSDL URI option. Provide the WSDL that you want to use in the doalog and click on the 'Discover' button provided in the dialog. as shown in the screenshot below:
WSDL: http://137.122.93.142/CalculatorWSApplication/CalculatorWS?wsdl

![http://i.imgur.com/bKfe34P.jpg](http://i.imgur.com/bKfe34P.jpg)

You will notice that the WSDL will be successfully added to the WSDL URI section.

4. After the WSDL is added, click on 'Generate Types' seen next to 'Discover' button. Click on Next in the Generate Type Wizard to see the mapping types. Click on Next and finish.

![http://i.imgur.com/HlGUXaw.jpg](http://i.imgur.com/HlGUXaw.jpg)

![http://i.imgur.com/s2Gd6Em.jpg](http://i.imgur.com/s2Gd6Em.jpg)

5. You will see the operations of this calculation webservice populated successfully.
Select 'add(float,float)' operation. An End Point Address URL will be created.
![http://i.imgur.com/b3nVic6.jpg](http://i.imgur.com/b3nVic6.jpg)

6. Data Mapping:
Now click on 'Data Mapping' under 'Properties' section. You will see input and output mapping sections.
Create two input variables of type 'Decimal'(say input1 and input2). Also create a decimal type output variable (say, output).
Map these created variables in the 'Data Mapping' section as shown in the screenshot below:

![http://i.imgur.com/LpPRLWa.jpg](http://i.imgur.com/LpPRLWa.jpg)

## Testing the Webservice Created ##
To ensure that the above created service works fine, hardcode the input values and run the service in the 'debug' mode.

1. Select the webservice created. Navigate to the Variables section.
Hard code the values of input variables (Say, input1=10.0 and input2=2.0). You can do so by selecting the variable and checking the 'Has Default' checkbox seen under 'Default Value' section. Provide the value for the variable as shown here:

![http://i.imgur.com/Yv7b4Sn.jpg](http://i.imgur.com/Yv7b4Sn.jpg)

Repeat the same steps for another input variable.

2. Navigate back to 'Diagram' window and run the service in the debug mode.
Click on 'Debug Service' option seen next to 'Run Service' button.
This will take you to the debug service in the browser as seen below:
![http://i.imgur.com/9fYPOKl.jpg](http://i.imgur.com/9fYPOKl.jpg)

As seen in the screenshot, the hardcoded input variables are clearly seen. The output variable is empty. This will be populated when the service is run.

3. Click on 'Step' button to step on the next call to this service.
You will now see that the service is executed and the output field is successfully populated. The output should contain the sum of two inputs provided.
This ensures that the service created is working fine.
![http://i.imgur.com/SrIIzPh.jpg](http://i.imgur.com/SrIIzPh.jpg)

We can use this service as a part of business process.
We can also use other operations of this webservice.