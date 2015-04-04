## Introduction ##

A Stored Procedure is a set of logic statements that are compiled into a single execution plan. Stored procedures assist in achieving a consistent implementation of logic across applications.

The SQL statements and logic needed to perform a commonly performed task can be designed, coded, and tested once in a stored procedure. Each application needing to perform that task can then simply execute the stored procedure.


## Stored Procedures for the project ##

Following stored procedures are to be used in your Library Management project:

[Stored Procedure to display the items borrowed by a particular user](sp_GetBorrowedItemListByUser.md)

[Stored Procedure to obtain available reference books that can be borrowed](sp_GetAvailableItemListReference.md)

[Stored Procedure to obtain available academic books that can be borrowed](sp_GetAvailableItemListAcademic.md)

[Stored Procedure to obtain email address of an user](SP_GetEmailAddress.md)

[Stored Procedure to indicate that the item borrowed is no longer available to others](sp_SetBorrowedItemList.md)

[Stored Procedure to make the returned items available to other users](sp_UpdateReturnedItemListToAvailable.md)

[Stored Procedure to calculate fine](sp_CalculateFine.md)

[Stored Procedure to block the user](sp_BlockUnBlockUsers.md)