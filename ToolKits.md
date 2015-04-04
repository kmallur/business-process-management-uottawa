# Introduction #

Toolkits are useful when many applications use common process or service components. Components of one toolkit can be shared with other toolkits.
The figure below gives an overview of "Toolkits" concept.

![http://i.imgur.com/YehPzUG.jpg](http://i.imgur.com/YehPzUG.jpg)

As seen above, toolkit's components are shared among several applications or another toolkit.

So, in general, toolkits are used to create components that can be reused in more than 1 project.
Example: In an health care scenario, a service to obtain patient demographics would be useful in every project.

So, creation of a toolkit should always be considered when common patterns are identified across multiple process apps. These common patterns might be specific to the business processes or  the coaches or to the data models.

System Toolkit is the default ToolKit provided by BPM. And contains , for example services to execute a SQL query, Service to send an email etc.
For a toolkit to be used, a snapshot of it must be taken and this snapshot must be referenced in a project that uses this toolkit.

![http://i.imgur.com/1Z8hTJQ.jpg](http://i.imgur.com/1Z8hTJQ.jpg)