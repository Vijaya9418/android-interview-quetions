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
  
      
   

   
