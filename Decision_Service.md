#Decision Service.

[Back to Table of Contents](Table_Of_Contents.md)

## Introduction ##

A decision service is built to determine which step needs to be invoked. The decision is based on a number of conditions, which are difficult to be modeled using simple if-else logic.

Say for example, a shop needs to determine how much percentage of discount has to be given to it's customers. The shop, in this scenario may have to consider various factors to determine the discount percentage to each of it's customers like - How long the customer is associated with this shop, how much of shopping he does on an average, what is the amount of profit he gives to the shop etc..

Decision Service can contain following components:

(a) Decision Table:

This component contains a table, where each row represent a rule. The rules in this table are boolean conditions. If the condition is met, then the rule action which is set in the java script section is executed.

(b) BAL Rule:

BAL stands for Business Action Logic. This component provides 'Rule Editor'.

To create rules using BAL Rule component:

http://pic.dhe.ibm.com/infocenter/dmndhelp/v7r5mx/index.jsp?topic=%2Fcom.ibm.wbpm.wle.editor.doc%2Ftopics%2Fbuilding_rule_service_C.html

(c) JRules Decision Service:

This component is used to integrate Process Manager with WebSphere ILOG JRules.

Refer to this link for creating jrule decision services:
http://pic.dhe.ibm.com/infocenter/dmndhelp/v7r5mx/index.jsp?topic=%2Fcom.ibm.wbpm.wle.editor.doc%2Ftopics%2Fbuilding_rule_service_C.html


## Tutorials ##

[Desicion Tables](TutorialDecisionServices_DecisionTables.md)


## Related topics ##
1) Creating decision services :

http://pic.dhe.ibm.com/infocenter/dmndhelp/v7r5mx/index.jsp?topic=%2Fcom.ibm.wbpm.wle.editor.doc%2Ftopics%2Fbuilding_rule_service_C.html

2) WODM :

http://en.wikipedia.org/wiki/IBM_Operational_Decision_Management