#Simple Business Process Definition.

[Back to Table of Contents](Table_Of_Contents.md)

## A Simple Business Process Definition ##
> We are designing in the first tutorial a simple business process where an employee is sending a Request Resource Form to his manager for his approval.

  * From the Designer menu, select Processes -> Business Process Definition.
  * Name the new Business Process Definition, such as "BPD01".
  * The diagram of the BPD01 shows two lanes with a start and end events. Drag and drop a lane from the palette on the top of the "Participant" lane.
  * Name the top lane as "Employee" and the other lane as "Manager". (Leave the system lane without changes).
  * Drag and drop two activities: an activity in the "Employee" lane and name it "Request Resource; a second activity in the "Manager" lane and name it "Review Resource".
  * Select the Sequence flow in the palette and connect the notations (Start event, "Request Resource" activity, "Review Resource" activity and End event).
![http://i.imgur.com/OxZIrXk.png](http://i.imgur.com/OxZIrXk.png)

  * Select the Variables tab and define five Private variables:
    1. "EmployeeName" of type String
    1. "ResourceType" of type String
    1. "BudgetAmount" of type Decimal
    1. "RequiredDate" of type Date
    1. "Approved" of type Boolean

![http://i.imgur.com/BE0M4lo.png](http://i.imgur.com/BE0M4lo.png)

  * Select the Diagram tab and from the main canvas, right click the "Request Resource" activity and select Activity Wizard.
  * An Activity Wizard window open, as in figure below, make the Activity Type Selection as "User Task". Select Next.
![http://i.imgur.com/LL57b5t.png](http://i.imgur.com/LL57b5t.png)

  * From the Activity Wizard - Parameters window, as in the figure below, select the output of the "Approved" variable into "false". This is because the "Manager" is the one who approve or disapprove the request. Click Finish.
  * Do the same Activity Wizard procedures with the "Review Request". The only difference is that the "Approved" variable is "True" for both the input and the output.
![http://i.imgur.com/YM4n2BN.png](http://i.imgur.com/YM4n2BN.png)

  * From the main canvas of BPD, double click on the "Request Resource" activity and select the Coaches tab.
  * The Coaches tab presents the Request Resource Form which contains the modeling controls of the variables.
  * You can change the captions of the controls and re-arrange them in different way. The figure below presents the Form of the "Request Resource".
![http://i.imgur.com/wEUUTh0.png](http://i.imgur.com/wEUUTh0.png)

  * You are done. So you can run the process by clicking on the "Run Process" icon at the right top.
  * The figures below show the sending the "Request Resource" form and submitting the approval of "Review Request" form.
![http://i.imgur.com/qM26ns8.png](http://i.imgur.com/qM26ns8.png)

![http://i.imgur.com/RVcQmru.png](http://i.imgur.com/RVcQmru.png)