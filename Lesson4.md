Tuesday, June 14, 2016
### An Object-Oriented Approach to Programming Logic and Design
#### Programming Logic and Design
###### Lesson 4
###### Understanding Web Applications

ASP (active server page) .NET building out of Visual Studio

###### HTML
- Hypertext Markup language
- Header and body tags `<head></head> <body></body>`

Rapid Application Development (RAD)

###### CSS

###### Javascript
- Client-side scripting language
- Runs inside web browsers
- jQuery or AJAX (Asynchronous Javascript an XML) to call to the server
- ASP .NET an AJAX framework lets you implement ajax Functionality on .NET

###### Client-side v. Server-side Programming
- Execute completing on user's local computer
- Executes completely on a server and make use of the server resources
- Hybrid applications use both client and server-side

2-tier or multi-tier
web server => app server => db server

###### ASP .NET
- is part of the .NET framework that enables you to develop web applications and web services
- 2 Main parts
  - classes and interfaces that communicate between web browser and web server. Organized in the System.Web namespace
  - runtime process  known as ASP .NET work process, handles the web request

- ASP .NET  worker process fulfills the ASP .NET
- compiles a .aspx file into an assembly and instructs the common language runtime (CLR) to execute the assembly
- The assembly executes, it takes the services of various classes in the .NET framework class library to accomplish its work and generate response messages to the requesting Client-side

- ASP .NET Page Life Cycle (events)
  - PreInt (page properties such as Request, Response, IsPostBack, and UICulture)
  - Init (all controls on the page are initialized and made available)
  - Load (if the request is a postback, the load stage is used to restore control properties with information from the )
  - PreRender
  - Unload

###### State Management
- state of the values of variables on a web page
- process of preserving the state of a web page across multiple tripos between browsers and server
- State management techniques:
  - Client-side technique
  - Sever-side management

- Common client-side state management techniques
  - query string
  - cookies (4k)
  - hidden fields
  - view state

- Query Strings (not recommended)
  - property of the Request object, and it gets the collection of all the query-string
- Cookies
  - is an object, instantiates with `new`
- Hidden fields
- View State
  - ASP .NET uses `View State` to maintain the state of controls across page post backs
  - collects values of all non post back controls that are modified in the code and formats them into a single encoded encoded string. String stored in a hidden field in a control named `_VIEWSTATE`
  - View State may increase the size of your page
  - View State is enabled by default by you can disable it either at the control level or at the page level

###### Server-side State management
- users server resources to store state information
- storing and processing session information on a server increases the server's load and requires additional server resources to serve the Web page
- ASP .NET supports server-side state management at two levels:
  - Session state
  - Application state

Session State
- unique session for each users
- can store temp user data such as shopping cart information

Application State
- used throughout an app
- is not user- specific
- accessed through app property of the Page class

`NOTE: Internet Information Servers (IIS) is a web server for hosting web applications on the Windows system
`
###### Web site and virtual directories
- sites, applications, and virtual directories
- web site is a container of applications and virtual directories
- virtual directory is an alias that maps to a physical directory on the Web server

Deploying Web applications
- Xcopy or FTP
- Windows Installer - can create virtual directories, restart services, register components, etc.

###### Web services
-  provide a way to interact with programming objects located on remote computers
- web services based on stardard technology an d are interoperable
  - XML (portability - any system can read it)
  - SOAP - protocol that defines how remote computers exchange


WSDL - Web Services Description Language
  - public interface of a web service and includes the following information
    - the data types it can process
    - the methods it exposes
    - the URL's through which those methods can be accessed

Creating Web Services
  - inherit from System.Web.Services.WebService
  - Mark the class with WebService attribute
  - Mark the methods with WebMethod attribute

Consuming Web Services
  - Add a reference to the Web service by using the Add web reference name.
  - the proxy object allows you to invoke Web service methods

`NOTE: protected - only the inherited classes can see it`
