[Assignment 2](Assignment_2.md)

#summary One-sentence summary of this page.

# Assignment(2) Part(2) Linked Process #

## Question ##
Part (2) of Assignment(2) involves the use of Linked Process in designing a business process.
Design and implement a business process where both the store clerk and the customer can request for an unavailable item. The requests should be then verified by the manager. The manager can approve or reject the requested item.
The process should have four main participants: the store clerk, the customer, the manager and the system.
The workflow of the business process is as follows:
  * Select the user type, whether a store clerk or a customer (use Radio button)

**_User type: store clerk_**

  * When the user is a store clerk, he can login by typing his email to verify his identity. Use one of the records seen in the clerkTB database table.

  * If the store clerk is logged in successfully,

  * He browses the list of items that are available in the inventory. (Items seen in inventoryTB should be displayed).  The list should contain information about the material number, item description, unit price, current quantity.

  * Then, he selects 1(or more) item(s) from the list.

  * Next, he adds the new quantities of the selected items only (in a separate browser) with information about the user: clerk name and email address.

  * The store clerk finally submits a request to the manager for approval.

  * If the identification fails,

  * He should be taken to the previous step (Selection user type page).

**_User type: customer_**

  * When the user is a customer, he needs to provide his name and email address before he could browse and request for an unavailable item of his interest.

  * Similar to the store clerk, he should also be able to browse and edit the items in the inventory (same as steps 3 and 4).

  * Once the manager receives the request from the clerk/customer, he can either approve the requested item or reject the request.

  * If the item is approved, the details of the approval must be updated in the database (the record should be logged into requestItemsTB database table, shown below). The process should contain an activity to display the approved record from the database to ensure the approval is successfully written to the DB.

  * If the order is not approved by the manager, the process should successfully terminate. Do not record the rejected items to requestItemsTB database table.

  * Use the Linked process concept to capture the tasks commonly performed by the clerk and the customer (Browse inventory + Request for the unavailable item)


## Process Walkthrough ##

Screenshots of business process flow can be seen here:

[Screenshots for business process flow](Assignment2_LinkedProcess_ScreenShots.md)


## Details of Database ##

  * Data Source: jdbc/BPMCourse
  * Database: BPMCourse
  * Table1: inventoryTB
  * Description: The table displays all the items in the inventory
  * Table1 columns:  materialNumber(VARCHAR), descrip(VARCHAR), unitPrice(DECIMAL), qty(INTEGER)

![http://i.imgur.com/7qZJbQP.png](http://i.imgur.com/7qZJbQP.png)

  * Table2: clerkTB
  * description: The table displays the store clerk details in the store. The store has 4 major clerks belonging to 4 different departments.
  * Table2 columns: clerkName(VARCHAR), clerkEmailAddress(VARCHAR), clerkDepartment(VARCHAR)

![http://i.imgur.com/vWlHxqt.png](http://i.imgur.com/vWlHxqt.png)

  * Table3: requestItemsTB
  * Description: The table contains the records that are approved by the manager. This table logs all the materials that are requested by the clerk/customer and that are approved by the manager.
  * Table3 Columns: requestorName(VARCHAR), requestorEmailAddress(VARCHAR), materialNumber(VARCHAR), descrip(VARCHAR), unitPrice(DECIMAL), qty(INTEGER)

![http://i.imgur.com/0x4JgBe.jpg](http://i.imgur.com/0x4JgBe.jpg)



## Related tutorials ##

[Linked Processes](TutorialLinkedProcess.md)

[Using the created Data Source in Process Designer](Using_DataSource_In_IBM_BPM_Process_Designer.md)