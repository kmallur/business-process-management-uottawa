#Steps to create users in BPM Process Admin Console are described here

[Back to Table of Contents](Table_Of_Contents.md)

## Creating BPM Users ##

Step 1:
Login to process Admin Console. Click on the link:
http://137.122.93.132:9080/ProcessAdmin/login.jsp#%23 and provide valid username and password

![http://i.imgur.com/zcla20X.jpg](http://i.imgur.com/zcla20X.jpg)

Step2:
Click on ‘User Management’ which is seen under “User Management” on the left hand side of the Process Admin Console.

![http://i.imgur.com/5nSZDpd.jpg](http://i.imgur.com/5nSZDpd.jpg)

Step3:
Provide %% in the ‘Retrieve Profile’ user-enterable field and click on ‘Retrieve’ button to see already existing internal IBM BPM users.

![http://i.imgur.com/2HzJ1he.jpg](http://i.imgur.com/2HzJ1he.jpg)

Step4:
To create a new user, provide valid username, Full name, Password as shown in the figure and click on ‘Add’ button. In the below figure, we have created a user account called ‘kmallur’.

Now navigate to ‘Group Management’ and provide %% in the ‘select group to modify’ section to view all the existing groups

![http://i.imgur.com/qI6cPvq.jpg](http://i.imgur.com/qI6cPvq.jpg)

Step 5:
Now navigate to ‘Group Management’ and provide %% in the ‘select group to modify’ section to view all the existing groups

![http://i.imgur.com/BqUV0bD.jpg](http://i.imgur.com/BqUV0bD.jpg)

Step 6:
Select ‘tw\_admins’ from the above displayed list and click on ‘Add Member’. ‘Add User and Groups’ window pops up. Provide the username that you want to add to ‘tw\_admins’ group and click on ‘Add Selected’ button to add the selected user.
You may add the created user to existing groups this way.

![http://i.imgur.com/7rtmtUz.jpg](http://i.imgur.com/7rtmtUz.jpg)

Step 7:
After the user is successfully added to the tw\_admins, you can login to designer using this created user and its password.

![http://i.imgur.com/jjbkRd6.jpg](http://i.imgur.com/jjbkRd6.jpg)

Step 8:
After logging into designer successfully, you need to add this use to the project that you would like to access.
So, Select a project seen in the Process Apps and open the same in Process Designer. You will see a message, which says that the user needs to be added to this project to access it. To obtain access to the project, you need to add this user to this project.

![http://i.imgur.com/R1FDHFB.jpg](http://i.imgur.com/R1FDHFB.jpg)

To add the user, click on the project itself. Under ‘Manage’ section click on “add user/groups” seen under ‘Manage Access to Process Library’. Add User and Groups window pops up. Provide the username that you want to add to that selected project and click on ’Add Selected’ button.

![http://i.imgur.com/4Bk3rRU.jpg](http://i.imgur.com/4Bk3rRU.jpg)

The user will be added with read access alone. You can select Write and Admin access to this added user by checking against those options.

![http://i.imgur.com/yQeeCUx.jpg](http://i.imgur.com/yQeeCUx.jpg)

Step 9:
Now open this project in Process Designer. You should be able to see the project and its processes successfully after adding the user to that project.

![http://i.imgur.com/wXlAIBl.jpg](http://i.imgur.com/wXlAIBl.jpg)