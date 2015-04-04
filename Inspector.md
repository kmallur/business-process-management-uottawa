[Back to Table of Contents](Table_Of_Contents.md)

## Introduction (In Progress\_Sonia) ##

The following image shows the Inspector interface and each major functional area:

![http://imgur.com/m5zX6Km.png](http://imgur.com/m5zX6Km.png)

1. Shows the currently active and previously run process instances on the Process Center Server or connected Process Server in the Process Instances tab. The highlighted instance is the currently selected instance, which means any action you perform or any data shown in the other areas of the Inspector apply to this instance. (The Services in Debug tab becomes active only if you select the Debug icon for a particular task.)

2. Use the Instance Name field and the Status drop-down menu to control the list of instances displayed in the Process Instances tab.

3. Use the drop-down lists to choose a different server on which to run the current BPD. You can also choose a different snapshot if you want to run a different version of the BPD. The Process Instances tab includes a Snapshot column so that you know which version of a process the currently displayed instances are running.

4. Use the icons in the toolbar to manage process instances, run tasks, or debug services.

5. Shows the current task for the selected process instance. In the preceding example, the current task is the first task in the BPD called Submit job requisition. You can click on the task to select it and then use the toolbar icon to run the task so that you can step through the entire BPD.

6. Shows the BPD diagram for the selected instance and highlights the current task so you know where you are in the execution of the process for this instance. In the preceding example, the red token above and the yellow halo around the Submit job requisition task indicate the active step. If you want to view other information about the BPD for the selected instance, you can click the other available tabs such as Overview and Variables.

7. Shows a tree view of the execution progress for the selected instance. In the preceding example, you can see the first step in the instance (the start of the process) and you can see the active second step, indicated by the red token. The tree view continues to expand if you decide to run the task and step through the entire process in the Inspector.

8. Shows the variables used in the current step. In the preceding example, we can see that the requisition variable is used in the active step. You can select a variable, right-click, and then select Show In Execution Evaluator to view and manipulate the variable values.

## Inspector Toolbar Options ##

When viewing instances of processes in the Process Instances tab of the Inspector, the following toolbar icons are available to help you manage those instances.

![http://imgur.com/UTXPr5i.png](http://imgur.com/UTXPr5i.png)
