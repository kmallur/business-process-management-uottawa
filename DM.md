#Data Mapping.

## Variables ##

Business objects - called variables - represent the data that provides the business context to a running process. Using variables, the process passes this data from one process step to the next.

Because the variables that you create are unique to the process or service definition (meaning that they are created at the process definition or service definition level, and are only available within that level), you can use a variable of the same name in.

The following variables can be declared in a Business Process Definition:

### Private ###
Private variables are local variables that are only seen within the process.
### Input ###
Input parameters are mapped to values that you can pass into the current process or service.
### Output ###
Output parameters are mapped to values that you can pass out from a process or service to a parent process or service.

## Data Mapping ##

Many activities have a Data Mapping section. This is the act of mapping the variables in scope in the BPD to the expected parameters of the service that is to be called by the Activity. This applies to both input parameters and output parameters.

The Data Mapping screen area is split into two columns. One for input mapping (mapping BPD variables to the parameters expected by a service) and the other is for output mapping (mapping returned values from a service to the variables in the BPD). Entry assistance is available to bring up lists of BPD scope variables which can be selected.

For example, consider that these are the input and output variables for a given process.

![http://imgur.com/rprDaom.png](http://imgur.com/rprDaom.png)

Now, in case we need to map these variables to the current or next activity, we need to go to the data mapping section of the activity and add the respective variables to the input and output.

![http://imgur.com/HBkZlBg.png](http://imgur.com/HBkZlBg.png)

Note that the variables defined in the scope of the BPD do not have to have the same names as the actual parameters of the service implementation. However their data types should be compatible with each other.

Note: The data mapping can be on the main process level as well as the at the activity level but are mainly dependent on the input and output variables which have to be mapped accordingly.

## Tutorials ##
[Create a listview on the coach from variables](ListView.md)