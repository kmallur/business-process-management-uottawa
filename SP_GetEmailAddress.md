## sp\_GetEmailAddress ##

This stored procedure is used to obtain email address of a particular user from Lib\_User table. The stored procedure accepts username as the input and provides email address as the output.

**Stored procedure snippet:**
![http://i.imgur.com/7FHN2iY.jpg](http://i.imgur.com/7FHN2iY.jpg)


**Lib\_User table:**

This table has the username, email address of the users. The table has a flag field called IsBlocked. This field will be 0 if the user is not blocked by the librarian. Else will be set to 1.

![http://i.imgur.com/naqOq3H.jpg](http://i.imgur.com/naqOq3H.jpg)