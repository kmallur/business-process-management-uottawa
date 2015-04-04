#Quick introduction to subprocesses (or linked processes). Page to be changed
##### Back to the [Table of Contents](Table_Of_Contents.md) #####
# Quick Explanation of Linked Processes and Subprocesses #

Subprocesses and linked processes are very useful to model a process for it to represent the reality of the process and to organize its complexity.

I made a very simple example that uses linked processes under Kat\_ExampleSubProcess. In that example, we have two main users. The secretary and the principal. The principal's role is simply to approve registrations and acknowledge deregistrations. The secretary's role (in this simplified process) is to register or deregister a student.

The model offers these two alternatives in the same application. To not clutter the higher level view of it, we abstract the tasks Register Student and Deregister Student in activities which are mapped to Linked Processes. However, we kept the principal's actions and the initial choice at this level because they do not contain much complexity and do not require much additional steps.

The overall thing is simplified but if Register Student was much more complicated and Deregister Student actually contained the steps needed to deregister a student, the higher view would become too complex to keep the process unidimensional. The added dimensions help hide the technicalities that might not interest the different levels of management.

IBM BPM offers two different ways to make process dimensions. One is Subprocesses and the other is Linked Processes. Subprocesses are intimately linked to the higher process and cannot be separated from it. In sum, they simply offer a different view of the process. They inherit values which means that values from the parent do not necessarily need to be passed as inputs or outputs. The Linked Processes need the inputs and outputs explicitly if they need to use of produce them. They are more flexible and can be copied elsewhere.