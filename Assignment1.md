[Back to Table of Contents](Table_Of_Contents.md)

## Assignment 1 ##

## Part (1): (Simple Business Process) ##
Use the IBM Process Designer to Design, implement and run the Business Process of a purchasing approval.
In this process the Store Clerk sends an approval request  to the Store Manager to order a material item. The request form must contain information like: name of the person who is placing the order, material number, description of the item, unit price, quantity and the total price.
The Store Manager will review the request and then he can either approve it or reject the request. The review form contains the same information of the request form plus a section to approve the request.



## Part (2): (Webservice) ##
Modify part (1) to automatically calculate the total price, once the requester provides the quantity of items and unit price of the item. Implement this using an outbound webservice that provides multiplication operation.
Use the following WSDL:
  * WSDL URI: http://137.122.93.142/CalculatorWSApplication/CalculatorWS?wsdl

Note: There are several websites which provide free web services, such as:
  * http://www.xmethods.net/ve2/Directory.po;jsessionid=uMmue9Wtt4z5CFPSbnwUYz_T
  * http://www.service-repository.com/
  * http://soaptest.parasoft.com/calculator.wsdl



## Part (3): (Data Source) ##
Modify part (2) by allowing the Store manager to save the approved details of an item in the database. Also, update the status of the record to 'Approved' in the database table against the added record.
Don't record to DB if the manager rejects the request.

Use the following information:

**Data Source:**
jdbc/BPMCourse

**Database:**
BPMCourse

**Table:**
purchasingTB

**Table columns:**
buyerName(VARCHAR), materialNumber(VARCHAR), descrip(VARCHAR), unitPrice(DECIMAL), qty(DECIMAL), totalPrice(DECIMAL), status(VARCHAR)

**Sample table values with header:**
![http://i.imgur.com/qdLJPUu.jpg](http://i.imgur.com/qdLJPUu.jpg)


## Part (4): (Verification of Part3) ##
Extend Part(3) to retrieve the populated entry from the Database table and display the same to the user in a coach.
This is to ensure that the record is successfully added to the table. And the status of that added record should be seen as 'APPROVED' in the DB(as seen in the screen shot, above) which is approved in Part(3).


## Process Walkthrough ##
[Process Walkthrough](Assignment1_screenshots.md)


## Related tutorials ##
[A Simple Business Process Definition ](SimpleBPD.md)

[A Simple Human Service Coach](SimpleCoach.md)

[Integrating web services](IntegratingWebServices.md)

[Using the created Data Source in Process Designer](Using_DataSource_In_IBM_BPM_Process_Designer.md)

Creation of Webservice:
https://docs.google.com/file/d/0B0yI-z4SR6HwU0dVM0lyWVlUaHM/edit