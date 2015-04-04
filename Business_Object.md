#Business Object

[Back to Table of Contents](Table_Of_Contents.md)

## Introduction ##

In the IBM Business Process Manager, Business Objects are the main vehicle to transfer and save information. To the computer programmer, they can be compared to normal variables. To the person that is more familiar with the business side of things, they are representations of actual business data.

In general, these business objects:
  * Are defined using industry standards
  * Transparently map data to database tables or enterprise information systems
  * Support remote invocation protocols
  * Provide the data programming model foundation for application programming

They are represented by XML schemas when defined but by Java Business Objects during runtime[[1](Business_Object#References.md)].

## Types of Business Objects ##

Business objects, or variables can be of different types. They can be of a simple type or a complex type. In addition, in the process, they can be declared as an input, an output, private, or as an Exposed Process Variable (EPV). They can use a predefined type. All of these variations will be explained in this section.

## Simple Types ##

Since Business Objects are based on XML schemas, the Simple Type corresponds to the XML schema simpleType[[2](Business_Object#References.md)]. It is simply composed of a single value with format variations. In IBM BPM, there are [Predefined Simple Types](Business_Object#Predefined_System_Types.md) that can be used for almost anything. However, when a custom date format or restricted integer value is needed, it can be useful to [create a custom Simple Type](Business_Object#How_to_Create_a_New_Simple_Business_Object_Type.md). Simple Types are used for things like dates or times, integer values, string values, and more specifically selection values which are used for things like dropdown lists.

## Complex Types ##

Like the Simple Type, the Complex Type is based on the XML schema complexType[[3](Business_Object#References.md)]. It basically corresponds to a hierarchical structure of Simple Business Objects to be able to represent more accurately the business data. For example, to represent a Patient, we can have a Patient Complex Type in which we would have his birth date (a Date Simple Type), his address (another Complex Type), his insurance information (a String Simple Type), etc. Complex Types can also contain lists of Simple or Complex Types.

## Inputs, Outputs, and Private Variables ##

A process can have Inputs, Outputs, and Private variables. Each of these has its use. If you need to pass data to the process, the process will have to have an Input variable. If the process needs to pass on data, the process will have an Output variable. If the process simply needs to process data inside it without receiving that specific piece of data or sending it to another process, this data can be put into a Private variable. If a piece of data needs to be sent to the process, but the process still needs to pass on that piece of data, changed or unchanged, you need to use an Input variable in addition to an Output variable, but with the _same_ name.

## Exposed Process Variables(EPVs - Advanced topic) ##

"Special type of variables that you can create to enable users to set or alter values while instances of a process are running. They need to be created before you can use them.

## Predefined System Types ##

IBM Business Process Designer comes with predefined Toolkits in which a section called "Data" can be found, like in any Process App. The types in the "Data" section can be used in the Process App being created. Information on any Business Object Type from these toolkits can be found by double-clicking on it. After double-clicking on the Business Object Type, in the main window, a general documentation on the Business Object can be found in the "Common" tab. If the Business Object Type has any parameters, more information can be found by clicking on the different parameters in the "Parameters" tab and then look in the "Parameter Properties" tab.

![https://business-process-management-uottawa.googlecode.com/git/images/SystemDataMenu.png](https://business-process-management-uottawa.googlecode.com/git/images/SystemDataMenu.png)
_Example of Data from a Toolkit_

![https://business-process-management-uottawa.googlecode.com/git/images/ExampleBDataInfo.png](https://business-process-management-uottawa.googlecode.com/git/images/ExampleBDataInfo.png)


## Tutorials ##

[How to Use a Business Object](TutorialUseDefinedBusinessObject.md)

[How to Create New Business Object Types](TutorialCreateBusinessObjectTypes.md)


## Related topics ##

`[`1`]` IBM - Business Process Manager - Library. Retrieved on 2014 April 28: http://www-01.ibm.com/software/integration/business-process-manager/library/documentation/v800/product_documentation.html

`[`2`]` `W3Schools` - XML Schema simpleType Element. Retrieved on 2014 April 29: http://www.w3schools.com/schema/el_simpletype.asp

`[`3`]` `W3Schools` - XML Schema complexType Element. Retrieved on 2014 April 29: http://www.w3schools.com/schema/el_complextype.asp

`[`4`]` IBM - Declaring variables for a BPD or a service. Retrieved on 2014 April 29: http://pic.dhe.ibm.com/infocenter/dmndhelp/v8r0mx/index.jsp?topic=%2Fcom.ibm.wbpm.wle.editor.doc%2Fmodeling%2Ftopic%2Fdeclaring_variables_B.html