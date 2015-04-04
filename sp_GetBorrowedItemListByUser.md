## sp\_GetBorrowedItemListByUser ##

This stored procedure is used to obtain all the items that are borrowed by a particular user.
This stored procedure accepts username as the input and identifies the userid of that user from the Lib\_User table and then fetch the item details, transaction details from the Lib\_Items and Lib\_Transaction tables.

**Stored procedure snippet:**
![http://i.imgur.com/hBN569y.jpg](http://i.imgur.com/hBN569y.jpg)


**Lib\_Item table:**

Lib\_Item can be books or CDs. Also, they are classified as Academic or Reference type.
The table stores the title name, item type, key id of the publisher from the Lib\_Publisher table, key id of the author from the Lib\_Author table, item cost, item status(Available/Borrowed).

**Lib\_Transaction table:**

It records the transactions performed by the users. The user would have borrowed the books or returned the borrowed the books. If the user has borrowed an item, the Lib\_Transaction table records the key id og the Lib\_User table, key id of the Lib\_Item table, Borrowed date and the due date(calculated field). The returned date timestamp is recorded in the table against a particular user's activity row, if the book is returned.

**Lib\_User table:**

This table has the username, email address of the users. The table has a flag field called IsBlocked. This field will be 0 if the user is not blocked by the librarian. Else will be set to 1.


![http://i.imgur.com/j92NMJs.jpg](http://i.imgur.com/j92NMJs.jpg)