#Coaching.

[Back to Table of Contents](Table_Of_Contents.md)

## Introduction ##

## Coaches ##

Coaches are the user interfaces for human services. There are two types of user interfaces for human services: dashboards and task completion. To build either type of user interface for human services, you use Coaches.

Coaches contain one or more Coach Views. The Coach Views provide the user interface elements and layout for the Coach. Each Coach View can contain one or more other Coach Views, which creates a parent-child relationship between these Coach Views. Each Coach View can also have a binding to a business object, CSS code to control its visual layout, and JavaScript to define its behaviour.

![http://imgur.com/WOF2N2m.png](http://imgur.com/WOF2N2m.png)

Coach Views are reusable so you can create a library of common user interfaces and behaviour. You can combine these common user interfaces to rapidly develop new Coaches.

## Heritage Coach ##

To maintain compatibility with earlier Coaches, IBM BPM supports Heritage Coaches. A Heritage Coach has the technology and architecture of a Coach in versions of IBM BPM before V8.0. A human service can have Coaches or Heritage Coaches. You can continue to use and maintain Heritage Coaches, but use Coaches for new user interfaces for services.

Visually, Coaches resemble Heritage Coaches in human service diagrams and on the palette.

![http://imgur.com/u9VvZ67.png](http://imgur.com/u9VvZ67.png)

The primary difference between Coaches and the Heritage Coaches of previous versions is that Coaches consist of one or more Coach Views. Coach Views are reusable collections of user interfaces that are frequently bound to a data type. This means that you can share common pieces of user interface between Coaches. For example, you can create a Coach that has a Coach View that contains a set of address fields. That is, the Coach View is bound to an Address business object and the individual text fields are bound to parameters of that business object. If you create a second Coach that needs address fields, you can reuse the Coach View. Conversely, with Heritage Coaches you must re-create the address fields. You can now implement your own custom controls as Coach Views and then reuse these custom controls in other Coach Views and Coaches.

Coaches support collaboration while Heritage Coaches do not. More than one person can work on the same Coach instance at the same time in their own browsers. For example, with collaboration, users can call on colleagues to help them complete a Coach instance. These users see which controls their colleagues are editing and the values that they are setting in those controls. Collaboration is available only if the service flow uses Coaches for its user interface. If the service flow contains one or more Heritage Coaches, collaboration is not available.

The control ID of a view-based Coach is different from the control ID of a Heritage Coach. The control ID of a Heritage Coach is the div node ID. This is not the case in view-based Coaches because Coach Views are reusable and you can have multiple views in a Coach.

## Human Service ##

Human service is a kind of interactive service which allows us to add a step into our business process definition(BPD) in order to create an interactive task that "process participants" can perform in a web-based interface. The main purpose of implementing human services in BPD is not only to improve the quality of service delivery systems but also to improvise on accessibility, accountability and coordination among process participants in the service delivery.

## Example Usage ##

- If an activity requires a call center employee to enter data about   customer order requests then we create a human service.So basically these are services with human interactions.

## Human services with coaches ##

When you build Human services, you include coaches, which are the web-based forms that provide process-related data to end users as well as collect input from those users. Coaches enable you to easily add standard fields and controls such as radio buttons, drop-down menus etc. This will allow the end users to participate in a business process by creating web based interface.

## Note ##

The Heritage Coaches are a part of legacy and hence we do not encourage to use them since we use the current version of BPM and they represent the version 7.5.

## Tutorials ##
[A Simple Human Service Coach](SimpleCoach.md)