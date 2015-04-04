#Services

# Services #

Services are used to implement the business operations in the activities of the Business Process. Reusability of services is one of the major advantages that BPM provides. This can be done by implementing services first using the Bottom-up approach and then using the implemented service on different Business Processes.

Services are usually called from the _Activity_  of the Business Process Definition. The Implementation tab is used to define the type of the invoked service. BPM 8.0 defines six of service types:
  * _Human Service_: The Human Service is used to create a task for a human being to work upon. The most common component used with the Human Series is the _Coach_ component, which is used to describe the  data to be presented to users and data to be retrieved from users.

  * _Ajax Service_: Ajax (Asynchronous JavaScript and XML) service describes the constructing  of web pages that have a dynamic content with the call to external services to obtain external data. It provides the ability to update the dynamic data content without the need to render all web page contents. Ajax Service is only used by Human Service

  * _Integration Service_: The integration service allows a process to invoke an external entity such as a Web Service or a piece of Java Code.

  * _Advanced Integration Service_: The Advanced Integration Service gives us the ability to define a service that is implemented by an IBM BPM Advanced SCA (Service Component Architecture) Module.

  * _General System Service_: The general system service is used when the BPD needs to work with the data in the process but does not need to invoke either a Web Service or Java Code. The General System Service is the simplest of the service implementation environments.

  * _Decision Service_: The Decision Service defines the business rules, which are the decision points in a process where the values of variables in the process are used to determine what to do next. The business rules are defined using three components:
    * _JRules Decision Service_
    * _BAL Rule_
    * _Decision Table_



---

_Reference: Neil Kolban, "Kolban's Book on IBM Business Process management, April 2013, p.p 205-239"_