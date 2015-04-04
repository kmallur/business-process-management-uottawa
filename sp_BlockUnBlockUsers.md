## sp\_BlockUnBlockUsers ##

This stored procedure is used to block and unblock users.
The users who have crossed the due date+tolerance is blocked by the librarian. Once the user has settled the billed fine and has replaced the lost book, the librarian unblocks the user.

The stored procedure accepts username as the input and updates the 'IsBlocked' column of the Lib\_User table. The column is updated to 'True' if the user is blocked. Else, the column remains 'False'.

Once the user is blocked, he will not be able to perform any activity(borrow/return) from the home screen. He is asked to contact the university department to settle the billed fine.


**Stored procedure snippet:**
![http://i.imgur.com/rtrMbrK.jpg](http://i.imgur.com/rtrMbrK.jpg)
![http://i.imgur.com/VUsh69h.jpg](http://i.imgur.com/VUsh69h.jpg)