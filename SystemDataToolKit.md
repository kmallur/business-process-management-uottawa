# System Data Toolkit #

System Data toolkit is imported into the Process Center repository during the installation of process designer.

One can only open this toolkit and view the items within but cannot edit or change the library items in the System Data toolkit

Each process application and toolkit that you create automatically includes a System Data toolkit dependency.
This will provide access to the assets that all IBM BPM projects require.
[.md](.md)

# Some commonly used System Data Integration Service #

## 1) SQL Execute Statement ##

Click on System Data under ToolKits and select 'SQL Execute Statement'. Drag and drop the service as shown in the screen shot
![http://i.imgur.com/HUQoLDj.jpg](http://i.imgur.com/HUQoLDj.jpg)

Declare a results variable of XMLElement type.
![http://i.imgur.com/QaqSbWU.jpg](http://i.imgur.com/QaqSbWU.jpg)

Under Data Mapping section, provide the datasource name and provide the sql query.The query that you want to execute can be directly provided in here or can be written in an init scrip which is called before the execution of the service.
Also, map the output variable.
![http://i.imgur.com/bw5yON3.jpg](http://i.imgur.com/bw5yON3.jpg)

Whenever a service is used, it is always recommended to run the process in debug mode to make sure, the service is behaving as expected.

So, run this service in the debug mode as shown in the screenshot:
![http://i.imgur.com/IbjZHiv.jpg](http://i.imgur.com/IbjZHiv.jpg)

![http://i.imgur.com/7iMhNOS.jpg](http://i.imgur.com/7iMhNOS.jpg)
As seen above, the sql statement is to obtain date from the DB.

The XMLElement result output is obtained
![http://i.imgur.com/RcALR3n.jpg](http://i.imgur.com/RcALR3n.jpg)

![http://i.imgur.com/2UZjMe3.jpg](http://i.imgur.com/2UZjMe3.jpg)

