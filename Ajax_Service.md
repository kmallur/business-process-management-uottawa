#Ajax Service.

# Tutorial (2) #

> Ajax Service is used to update the dynamic data content of a webpage without the need to render all web page contents.In this tutorial, we will create an Ajax service to update the data inputtext component of a Human Service.

![http://i.imgur.com/kZH63n7.png](http://i.imgur.com/kZH63n7.png)

  * From the Designer menu, select User interface -> Ajax Service
  * Name the new Ajax Service, such as "AS01".
  * The diagram of the new Ajax service shows a start and end. Drag and drop Server Script from the component panel and name it "Say Hello"

![http://i.imgur.com/eSkGTQ1.png](http://i.imgur.com/eSkGTQ1.png)

  * Select the Variables tab, and add an input String variable "pName" and an output String variable "greeting".
  * From the Property view, select implementation and type the following JS code in the script block:
```
  tw.local.greeting= "Hello "+tw.local.pName;
```
![http://i.imgur.com/8PxDGo0.png](http://i.imgur.com/8PxDGo0.png)

  * From the Designer menu, select User interface -> Human Service
  * Name the new Ajax Service, such as "HS01".
  * The diagram of the new Human service shows a start and end. Drag and drop Heritage coach from the component panel and name it "Say Hello"
![http://i.imgur.com/LZfRADg.png](http://i.imgur.com/LZfRADg.png)

  * Open the coach and add two Text Area and a Button Group. You can rearrange the added components.
![http://i.imgur.com/WLI2Dpe.png](http://i.imgur.com/WLI2Dpe.png)

  * Change the Label and Control Id of the text areas into "Person Name", "pId", "Greeting" and "gId" respectively.
![http://i.imgur.com/oLvTHdd.png](http://i.imgur.com/oLvTHdd.png)

  * Select the new button and name it "Say Hello".
  * In the Property view, click on Presentation and type the following in the Validation Script block:
```
var pName= dojo.byId("pID").value;
var vars= "<inputs><variable name='pName'>"+pName+"</variable></inputs>";
tw.coach.callService("AS01",vars, function(myGreeting)
{
  dojo.byId("gID").value= myGreeting.greeting;
});
```

![http://i.imgur.com/VzeCAKO.png](http://i.imgur.com/VzeCAKO.png)

  * You are done. Run the Human Service "HS01" and Type and name. Figure below describe the output.
![http://i.imgur.com/rizZfPW.png](http://i.imgur.com/rizZfPW.png)