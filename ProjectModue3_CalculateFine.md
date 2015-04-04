# Calculation of fine #

![http://i.imgur.com/y668nxC.jpg](http://i.imgur.com/y668nxC.jpg)

As seen in the screen shot above, Calculate Fine is a system task.
As soon as the user selects the borrowed items to return and clicks on 'Return' button, the flow is given to this system task.

The task is programmed to calculate fine depending on the number of difference between the borrowed date and the returned date.

The system task is attached to a service: uOttawa Library Calculate Fine as seen here:

![http://i.imgur.com/WHUPS93.jpg](http://i.imgur.com/WHUPS93.jpg)

The variables used in this service is as seen here:

![http://i.imgur.com/mql54TP.jpg](http://i.imgur.com/mql54TP.jpg)

The service begins with initializing the count variable to 0.
The 'More Items' decision service checks if there is 0/more items selected. As long as there is at least 1 item selected by the user, the flow continues and fine is calculated. Incase no items are selected by the user, fine calculation flow is not reached.

![http://i.imgur.com/al9T6EL.jpg](http://i.imgur.com/al9T6EL.jpg)

A storedprocedure: sp\_CalculateFine is then called which calculates fine for every selected item based by the user.

![http://i.imgur.com/dSDM2In.jpg](http://i.imgur.com/dSDM2In.jpg)

![http://i.imgur.com/dLkugNj.jpg](http://i.imgur.com/dLkugNj.jpg)

![http://i.imgur.com/ImhgcMa.jpg](http://i.imgur.com/ImhgcMa.jpg)

Once the fine is successfully calculated, it is given to the next activity in the flow: Confirm Return. Fine column is added for the selected items. And the calculated fine for every item is displayed in this column.