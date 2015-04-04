# Display only borrowed items to the user and to select 1/all those displayed items #

![http://i.imgur.com/wgSETem.jpg](http://i.imgur.com/wgSETem.jpg)
The 'Return Item' transaction begins by displaying 'only borrowed items' to the user.

This activity has an human service attached:uOttawa Display Borrowed Items By Users as shown in the screen shot:
![http://i.imgur.com/u2sfTP4.jpg](http://i.imgur.com/u2sfTP4.jpg).

This process also makes use of a general system service: uOttawa Display Get Borrowed Items By Users. This calls the stored procedure: sp\_GetBorrowedItemListByUser, which retrieves and displays only the items borrowed by the user using the BPM service.
These items obtained from the stored procedure are then displayed onto the coach.

![http://i.imgur.com/ohqk4cj.jpg](http://i.imgur.com/ohqk4cj.jpg)

Sample variables used in this service is shown in the below screenshot:

![http://i.imgur.com/QE5cfdC.jpg](http://i.imgur.com/QE5cfdC.jpg)

The user at this point, can select 1/more items from the displayed borrowed items and click on 'Return'.
The items that are selected alone are screened out using a server script: Remove Unselected Items as shown in the screenshot:

![http://i.imgur.com/einkgmY.jpg](http://i.imgur.com/einkgmY.jpg)

This screened selected items are displayed on the 'confirm return items' coach as seen below:

![http://i.imgur.com/8m8Prj2.jpg](http://i.imgur.com/8m8Prj2.jpg)

This time, the 'confirmed Return Coach' shows an extra column called 'Fine' against each of the selected borrowed items to be returned.
The fine is calculated by the library system and is explained in the FineCalculation section.

Note: For viewing the output of this transaction, visit page: [ProjectModule1\_HomePage](ProjectModule1_HomePage.md)