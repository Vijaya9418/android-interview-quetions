# android-interview-quetions

1. What is android?

   Android is an operating system specifically designed for mobile and tab applications, its a kind of software stack for mobile applications which is developed by google.
   It is a linux kernel and provide a framework for devlopers to develop the android applications and softwares that can run on android powered devices.

2. What is android framework?

   Android framework is a key component of android operating system, which provides API (Application programming interface), and various tools which are used by developer to      build applications and to interact with various functionalities of android device.<br>

   It provides various components and services that facilitate app development such as, activity manager, content provider etc.

3. Define android architecture?

   Android follows the layered architecture that contains various components and frameworks, which are:-
   1. Linux Kernel:- It sits at the core of an android architecture which is basically provides a low-level hardware abstraction, process management and device dirvers.
      Apart from that it also manages the core functionality such as memory management and networking.

   2.Hardware Abstraction layer:- It bridges between the android framework and device specific hardware. It also provides standard interface for android frameworks to
     interact with hardware components such as camera, audio, videos etc.

   3.Android Runtime:-It is a virtual machine responsible for running the android applications.It executes the dalvik(.dex) or the newer android runtime binary(.art), which
     performs AOT(Ahead of time) which converts the byte code into machine language to improve the performance.

   4.Libraries:- Android provides various native libraries that are written in C/C++ which are used by various system components.These libraries include graphic rendering, SQLite database engine and more.

   5.Android Framework:- It is a key component of android operating system that provides Application programming interface and various libraries which are used by developers
     to build applications and interact with various functionalities of android device, it contains various key components like activity, services, broadcast receivers, 
     content providers etc.

   6.Application layer:-This layer comprises the android application with which the user interacts with. It include pre installed systems such as phone dial, messaging app,         browser, as well as third party library.

4. Define android components?

   There are basically 4 basic components in android:-

   Activity:- It represents the single screen of UI component and with which the user interacts with, It helps the user to navigate from one activity to another and perform       some action.<br>
   
   Service:- It is used for performing the long running tasks/background tasks or which does not required intercation with UI.<br>
   
   Broadcast receivers:- It is basically used for receiving and responding to the messages or broadcasting the messages.<br>
   
   Content provider:- It is used for managing the intercation between different applications.They can be used to start activities, launch services, broadcast messages, or        pass data between components.<br>

5. Define intent and its types.

   Intents are basically a messaging system that is use to interaction with components, within the application or with other applications. It can be seen as abstract discription of an operation to be performed.<br>
   
   There are two types of intents:-
   Explicit intent:- Whhich is basically use to interact with inner part of the application. for example if you want to send the data from one activity to another within the      application or you want to go from one activity to another, explicit intents are used.

   Implicit intent:- It is used to interact with outer part of the application. For example if we want to open a phone dial with from our application.or if you want to share      an image from your application.

6. Define activity Lifecycle:-

   It is several events or stages with which an activity goes through in an application. Activity lifecycle is consits of seven stages.:-

   1. OnCreate:-It is the very first stage where the activity is created.
   2. OnStart:- It is the second stage where the activity starts, when the activity becomes visible to the user.
   3. OnResume:- It is called when the activity is about to start interacting with the users.
   4. OnPause:- It is called when the activity is about to loose focus.
   5. OnStop:- It is called when the acitivity is no longer visible to the user, but there in the background.
   6. OnRestart:- It is called when the activity is restarted after being stopped.
   7. OnDestroy :- It is called when the activity is removed from the background.
  
7. What are OOPs concept?

   Object oriented programming is a software design pattern that is revlovs abround object and classes which provides the reuseability, readability to improve the performance.
   It sits on four pillars, which are :-
   
   Inheritance:- It is the ability of a class to inherit the property of its parent class.for example:- a child can inherit the property of parents.
   
   Abstract:- It is used to hide most of the information and to show only the relevant information to the user. for example:- ATM.
   
   Encapsulation:- It is the process of bundling the data(attribute) and methods(behaviour) together and get the full access through them with the help of access modifier         public, protected and private. We also use getter and setters which helps in data hiding and maintaining the inetrgrity of the data.
   
   PolyMorphism:- It comprises of two words poly means many and morphism means form, so it is the ability of an objcet to take multiple forms, which we can achieve by             overloading and overrriding.

8. Define overloading and overriding?
   
   Overloading:- It is also called run time polymorphism in which meathod have same name , but differ in parameters. It can be differ in the number of params or the type of params.
   
   Overriding:- It is also called compile time polymorphism in which a sub class has the same method name as that of the super class, but the implementation is differnt.

10. what are the types of service?
    
    There are two types of service:-
   
   Started Service:- this is the service which starts explicitly and which may take longer time to complete such as downloading the file from server.<br>
   It continues to run in the background until the task is completed even after the associated activity is destroyed.

   Bound Service:- this is a service when multiple component need to interact with a service, typically bindService() method.<br>
   When all the components unbind from the service, the service is destroyed and stopped.


11. What are the types of content providers?
    
    there are two types of content providers:-

    Custom Content provider:- These are the content provider which are created by the Developers to share data between different applications or components within the             application.Developers define their own Content Provider by subclassing the ContentProvider class and implementing the necessary methods to handle data operations.

    System Content provider:- These are the providers which are provided by android system.It manages and provide access to various system data such as contact, media, files      and settings.These Content Providers are part of the Android framework and are responsible for maintaining and exposing system-related data to applications.

12. What is intent filter?
    
   Intent filter is the key component which is use to declare what type of intent an application or component can handle.It is defined using intent-related attributes in the 
   AndroidManifest.xml file.
   
   Its key attribute are:-
   Action:- It provides action or actions that a component can respond to, It is basically an string representing desired operations.such as "android.intent.action.VIEW" or "android.intent.action.SEND".<br>
   Category:-Categories provide additional information about the component's purpose or behavior. such as android.intent.category.DEFAULT or "android.intent.category.BROWSABLE".<br>
   Data: Specifies the data type or scheme that the component can handle. It can include attributes like the data MIME type or a specific data scheme. For example, an activity can specify that it can handle "http" URLs or image files.<br>

13. Define fragment and its lifecycle?
    Fragments:- It is modular and reuseable UI component in android that represents a piece of activity. It is designed for building responsive user interface, it has its own    lifecyle , layout, views etc.
    
    Fragment lifecycle are as follows:-
    onAttach(): This method is called when the fragment is associated with its hosting activity.<br>
    onCreate(): This method is called when the fragment is created.<br>
    onCreateView(): This method is called to create the fragment's user interface, typically by inflating a layout resource or dynamically creating UI components.<br>
    onViewCreated(): This method is called after onCreateView() and allows you to perform additional UI setup or access the inflated view hierarchy.<br>
    onStart(): This method is called when the fragment becomes visible to the user.<br>
    onResume(): This method is called when the fragment is about to start interacting with the user.<br>
    onPause(): This method is called when the fragment is about to lose focus or be partially obscured.<br>
    onStop(): This method is called when the fragment is no longer visible to the user.<br>
    onDestroyView(): This method is called when the fragment's view is being destroyed.<br>
    onDestroy(): This method is called when the fragment is being destroyed.<br>
    onDetach(): This method is called when the fragment is detached from its hosting activity.<br>

14. What is the lifecycle of Service?

    onCreate(): This method is called when the service is first created.<br>
    onStartCommand(): This method is called when a client calls startService() to start the service.<br>
    onBind(): This method is called when a client calls bindService() to bind to the service.<br>
    onUnbind(): This method is called when all clients have disconnected from the service by calling unbindService().<br>
    onRebind(): This method is called when a new client binds to the service after onUnbind() has been called.<br>
    onDestroy(): This method is called when the service is about to be destroyed.<br>

15. A service that was initially started with onStartCommand by a calling startService can still receive a call to _____. when a client calls bindService.

    The onBind() method allows clients to bind to the service and communicate with it through an interface defined by an IBinder. By implementing onBind(), the service 
    provides a way for clients to access its functionality and establish a connection with it.
    So, even if a service is started with startService(), clients can still bind to it using bindService() and interact with it through the returned IBinder object.

16. What is anr?
    
    ANR is application not responding which is an error condition that occurs when the user interface of an application becomes unresponsive and user is not able to
    interact with it. When an ANR occurs, the system displays a dialog to the user, notifying them that the application has stopped responding and giving them the option to       close it.<br>
    It can be caused by long running tasks in the main thread, deadlocks, excessive CPU or memory usage.

17. What is a Deadlock?

    A deadklock occurs when multiple thread wait for other threads to release their resources, resulting in the deadlock state where none of them can proceed.

18. What is bundle?
    
    A bundle is acontainer that holds the key-value pairs, similar to dictionary or map. It is commonly used for passing data between different components, within
    application such as between fragment and activity.

19. what is Context in android?
    
    A Context is an essential class in android that provides access to various resources and system level operations within the application. It repeasents the current state
    and environment in which the application is running.Context is typically obtained from the Android framework and is passed to different components, such as activities,        services, and broadcast receivers, to access system resources and perform operations.

20. what are the types of context?
    
    1. Application context:- It is associated with entire life cycle of the application, which can be called useing getApplicationContext(), It should be used wherever
       the context is not tightly coupled to any specific conponent such as activity, service etc.
    2. Activity Lifecycle:- It is specific to particular activity and tied to the lifecycle of that service.It can be acessed within the activity using this keyword.
       The Activity Context should be used when you need a Context that is closely related to the current activity, such as creating views, inflating layouts etc.
    3.Service context:-The Service Context is specific to a particular service and is tied to the lifecycle of that service.It can be accessed within a service using the this       keyword or ServiceName.this.The Service Context should be used when you need a Context that is closely related to the current service, such as accessing service-              specific resources, starting new activities, or accessing service-related services.

21. What is manifest?

    A manifest file is an essential file that provides an important information about your application. It contains various key components such as service and the permission      which your app needs, launching configuration of your app, package name, intent filter etc.
      
  
      
   

   
