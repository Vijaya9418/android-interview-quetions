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
   
   Content provider:- It is used for managing the intercation between different applications.They can be used to start activities, launch services, broadcast messages, or pass    data between components.<br>

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
  
      
   

   
