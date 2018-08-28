**layers**

3 layer model vs 3 tier model

_Horizontal layers:_

Presentation: Every enterprise application has a UI, in fact graphical UI. This UI can be web or desktop based, which doesn't matter. The rule is simple. UI takes user action and sends it to the controller. And at the end it shows result taken from controller to the user. UI can be implemented according to MVC, MVP, MVVM or another approach.

Control: Handles business logic of the application. Takes info from user and sends it to DB layer (DAO or ORM framework) and vice versa. Abstraction type of controller may vary (a separate control and business layers for example)  according to the application parameters or development patterns (MVC, MVP, MVVM, ...) but the main idea remains the same.

Data Access: Database handling layer of the application. It may contain entity definitions, ORM framework or DB connection codes having SQL sentences, according to the abstraction decision. Its role is getting data from controller, performing data operation on database and sending results again to controller (if result exists). Database independence is a very important plus for this layer, which brings flexibility.

_Vertical layers:_

Security: Security is a general concept, which includes user authorization, user authentication, user role management, network or SQL injection attack prevention, data recovery etc but we grouped that items generally as "Security". Those issues must be handled for each horizontal layer if you want to have a fully secure software.

Logging: Logging is very important for maintenance and reporting in enterprise applications. An easily configurable, parameterized, readable, flexible and correctly implemented logging layer for all horizontal layers is very useful for both developers and users. 

i18n: i18n (internationalization) brings multiple language support and user interface text changing capability without rebuilding code. It may also have localization property which can handle number, currency and date formatting. So i18n provides flexibility on appliations and should not be ignored.

Exception Handling: Exception handling may also be included in "Security" or "Logging" layers. We should not use only general exception classes or absorb all exceptions if we want to develop a quality software. We sometimes need our special exception classes with their specific behaviours for better security, logging and application performance.

**service**
A Service is an application component representing either an application's 
desire to perform a longer-running operation while not interacting with the user 
or to supply functionality for other applications to use.  
Each service class must have a corresponding declaration in its package.  
Services, like other application objects, run in the main thread of their hosting process.  
This means that, if your service is going to do any CPU intensive (such as MP3 playback) 
or blocking (such as networking) operations, it should spawn its own thread 
in which to do that work.

**MVC**
Model - Model represents an object or JAVA POJO carrying data. It can also have logic to update controller if its data changes.

View - View represents the visualization of the data that model contains.

Controller - Controller acts on both model and view. It controls the data flow into model object 
and updates the view whenever data changes. It keeps view and model separate.



**components**
AWT. >> button, Jpanel, JFrame, textpane, label, list, menus, lists... 
@Component >> /Service, Repository/ Controller, Model

Reusable chunks of code

**communication between layers and components**
Dependency Injection
@Autowired


**Examples:**
???

**Expected skills (2/3)**
- Able to identify separate responsibilities of the application
- Able to explain how data is stored and used over the application
- Able to demonstrate how to add new property to a model 
(parent class or interface - socket, state or proxy design pattern)
