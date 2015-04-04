## sp\_GetAvailableItemListReference ##

This stored procedure is used to obtain all the available items that belong to 'Reference' section from the 'Lib\_Items' table.

**Stored procedure snippet:**
![http://i.imgur.com/ngtz7ua.jpg](http://i.imgur.com/ngtz7ua.jpg)


**Lib\_Items table:**
![http://i.imgur.com/iegqD9h.jpg](http://i.imgur.com/iegqD9h.jpg)

As seen above, Lib\_Items can be books or CDs. Also, they are classified as Academic or Reference type.
The table stores the title name, item type, key id of the publisher from the Lib\_Publisher table, key id of the author from the Lib\_Author table, item cost, item status(Available/Borrowed).
