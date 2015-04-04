## sp\_UpdateReturnedItemListToAvailable ##

This stored procedure is used to update status of the returned items to 'Available' in the Lib\_Item table.
It also updates the return time stamp in the Lib\_Transaction for that particular user-transaction to the current date(on which the item is returned).
The stored procedure accepts username and title id as the inputs and updates the tables suitably.

If more than 1 item is returned, then the stored procedure updates two transaction in the Lib\_Transaction table.

**Stored procedure snippet:**
![http://i.imgur.com/XLc9F9m.jpg](http://i.imgur.com/XLc9F9m.jpg)
![http://i.imgur.com/pwj9jZt.jpg](http://i.imgur.com/pwj9jZt.jpg)


**Lib\_Item table:**

Lib\_Item can be books or CDs. Also, they are classified as Academic or Reference type.
The table stores the title name, item type, key id of the publisher from the Lib\_Publisher table, key id of the author from the Lib\_Author table, item cost, item status(Available/Borrowed).

**Lib\_Transaction table:**

It records the transactions performed by the users. The user would have borrowed the books or returned the borrowed the books. If the user has borrowed an item, the Lib\_Transaction table records the key id og the Lib\_User table, key id of the Lib\_Item table, Borrowed date and the due date(calculated field). The returned date timestamp is recorded in the table against a particular user's activity row, if the book is returned.

![http://i.imgur.com/5KC1Mmo.jpg](http://i.imgur.com/5KC1Mmo.jpg)