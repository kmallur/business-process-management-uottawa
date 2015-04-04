## sp\_SetBorrowedItemList ##

This stored procedure is used to update Lib\_Item and insert transaction details to the Lib\_Transaction tables. The stored procedure accepts username and the title id of the borrowed item and updates the status to 'Borrowed' in the Lib\_Item table. It then inserts the transaction details to Lib\_Transaction table.

If more than 1 item is borrowed, then the Lib\_Transaction table contains two record for this activity performed by the user

**Stored procedure snippet:**
![http://i.imgur.com/cFA39dH.jpg](http://i.imgur.com/cFA39dH.jpg)
![http://i.imgur.com/fdkB2X2.jpg](http://i.imgur.com/fdkB2X2.jpg)


**Lib\_Item table:**

Lib\_Item can be books or CDs. Also, they are classified as Academic or Reference type.
The table stores the title name, item type, key id of the publisher from the Lib\_Publisher table, key id of the author from the Lib\_Author table, item cost, item status(Available/Borrowed).

**Lib\_Transaction table:**

It records the transactions performed by the users. The user would have borrowed the books or returned the borrowed the books. If the user has borrowed an item, the Lib\_Transaction table records the key id og the Lib\_User table, key id of the Lib\_Item table, Borrowed date and the due date(calculated field). The returned date timestamp is recorded in the table against a particular user's activity row, if the book is returned.

![http://i.imgur.com/5KC1Mmo.jpg](http://i.imgur.com/5KC1Mmo.jpg)