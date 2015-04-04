[Back to Table of Contents](Table_Of_Contents.md)

## Creation of Data Source from IBM Administrative Console ##


1)	Log into OslerBPM remote machine by providing a valid username and password.


![http://imgur.com/EIPo7jr.png](http://imgur.com/EIPo7jr.png)


2)	From the start menu, navigate to IBM Administrative console


![http://imgur.com/y1rKRbI.png](http://imgur.com/y1rKRbI.png)


In case of a security warning, please continue to proceed.


![http://imgur.com/JMOo6Rw.png](http://imgur.com/JMOo6Rw.png)



You will land at this screen:


![http://imgur.com/RdX7htR.png](http://imgur.com/RdX7htR.png)



Provide valid username/password and login. You will now see Websphere Integrated Console as in the below screenshot:


![http://imgur.com/w8dwwUx.png](http://imgur.com/w8dwwUx.png)


3)	Navigate to “Data Source” under “Resources/jdbc”, one of the options displayed on the left hand side of the page.


![http://imgur.com/lNYQK6S.png](http://imgur.com/lNYQK6S.png)





4) Creating a new Data Source:
Click on “New” seen just above the table listing. Provide a Data Source name(say, BPMTest) and the JNDI name (say, jdbc/BPMTest) as shown in the screen shot below, and click on Next:


![http://imgur.com/Vkllz34.png](http://imgur.com/Vkllz34.png)



Select JDBC provider from the list as seen below:


![http://imgur.com/JLD8vQq.png](http://imgur.com/JLD8vQq.png)



Provide the database name, to which you need to connect. Before we do this, ensure the DB User properties are set. The steps are illustrated here:
**[Setting User Properties on SQL Server DB](DataBase_Setting.md)**

5)	With the the illustrated DB settings, continue creating the data source. Now, provide DB name to which we need to connect (in this example, it is BPMPractice), port number (1433 is the default) and the ServerName (137.122.93.90) . Click on Next to proceed.


![http://imgur.com/szYsjgC.png](http://imgur.com/szYsjgC.png)




6)	Set up Security aliases. Provide ‘processDBLogon’ (for now) as shown in the screenshot. We have to change this after creating the JAAS-J2C configuration.
Click on Next. And then finish the steps.



![http://imgur.com/BlvXi9B.png](http://imgur.com/BlvXi9B.png)



![http://imgur.com/j8grvG1.png](http://imgur.com/j8grvG1.png)



7)	Now ‘save’ the data source that we just created.


![http://imgur.com/sMxCOYy.png](http://imgur.com/sMxCOYy.png)




Once the Data Source is saved, it is listed as in the screenshot:



![http://imgur.com/BDkS9Xf.png](http://imgur.com/BDkS9Xf.png)



8) Creating Jaas-J2C Authentication Data.
Select the Datasource from the listing. Click on ‘Jaas-J2C Authentication Data’, which is seen under the ‘Review’ section on the right hand side of the screen( shown in the screenshot)


![http://imgur.com/obzROMW.png](http://imgur.com/obzROMW.png)


Click on ‘New’ to create one afresh.


![http://imgur.com/AEN7jD3.png](http://imgur.com/AEN7jD3.png)



Fill the general properties as shown below.
Provide the following:
> Alias: Some alias name (say, bpmtest)

> UserId: User created in the DB (in our case, it is bpmadmin)

> Password: Password provided for this above user (in our case, it is bpmadmin)


![http://imgur.com/nYxmUad.png](http://imgur.com/nYxmUad.png)



Click on OK and then save the action performed.


![http://imgur.com/qWhBIKm.png](http://imgur.com/qWhBIKm.png)


After saving the action, the resource created above is listed as seen below:


![http://imgur.com/zNKFCrC.png](http://imgur.com/zNKFCrC.png)


9)	As said before, we will now use this Jaas-J2C Authentication data (created in Step8) in the Security Settings of the Data Source (temporary value provided was ‘processdblogon’ in step6. This will now be changed using the above created value).


![http://imgur.com/AGiIBIz.png](http://imgur.com/AGiIBIz.png)


10)	Save the above process. Select this changed Data Source and click on ‘Test Connection’ to test the data source.



![http://imgur.com/DlxhRR6.png](http://imgur.com/DlxhRR6.png)



![http://imgur.com/UGOtrKH.png](http://imgur.com/UGOtrKH.png)
