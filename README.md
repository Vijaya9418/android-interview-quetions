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
    3.Service context:-The Service Context is specific to a particular service and is tied to the lifecycle of that service.It can be accessed within a service using the this keyword or ServiceName.this.The Service Context should be used when you need a Context that is closely related to the current service, such as accessing service-specific resources, starting new activities, or accessing service-related services.

21. What is manifest?

    A manifest file is an essential file that provides an important information about your application. It contains various key components such as service and the permission which your app needs, launching configuration of your app, package name, intent filter etc.

22. What is adb?

    ADB(Android Debug Bridge) it is a command-line tool which helps to communicate between your computer and android emulator or device. It is a part of SDK(Software Development kit) used for mainly debugging and testing the android devices.
    1. Debugging and Logging:
    2. Application Installation and Management:
    3. File Transfer:

23. Difference between abstract and Interface?

    Abstract:-<br>
    An abstract class in java cannot be instantiated , it means we cannot create the object directly from it.
    It can contain both abstract and not abstract methods. Abstarct methods are declared without an implementation and must be implemented by its subclass.
    Subclasses of an abstract class must either implement all the abstract methods or be declared as abstract themselves.


    Interface:-<br>
    An interface in java is a collection of abstarct methods and constand variables.It defines a contract or rule of how a clss should behave.
    It serves a way to acheive multiple inheritance as in java a class can implement multiple interface.
    All methods in an interface are public and abstract by default.

    Differences:
    
    Implementation: A class can extend only one abstract class, but it can implement multiple interfaces.
    Abstract classes can have both abstract and non-abstract methods with complete implementations. Interfaces can only have abstract methods.
    Access Modifiers: Abstract class methods can have different access modifiers (public, private, protected), while interface methods are implicitly public.
    Variables: Abstract classes can have member variables, while interfaces can only have constant variables (static final variables).

24. Collections in java?

   In java, Collection framework provides a set of classes and interface for working with group of objects.It provides basic operations like adding, removing and queuing of elements.

25. What is an exception?
    An exception is an event that occurs during the execution of a program that disrupts the original flow of a program.Exceptions are use to handle, errors,              exception conditions. The java language provides build-in handling exception mechanism to deal with this type of situation.<br>
    
    Exception Hierarchy:
      Exceptions in Java are organized in a hierarchical structure, with the base class being java.lang.Throwable.
      Throwable has two main subclasses: Exception and Error.

    Exception Handling:

      Exception handling is the process of catching and handling exceptions to prevent program termination and provide meaningful feedback to the user.
      The try-catch-finally block is used to handle exceptions. The try block contains the code that may throw an exception, the catch block catches and handles the         exception, and the finally block is executed regardless of whether an exception occurs or not.

26. Sort the list of elements using bubble sort?
    
    import java.util.ArrayList;

    public class ArrayListSortingExample {

    public static void main(String[] args) {
    
        // Create an ArrayList of integers
        ArrayList<Integer> numbers = new ArrayList<>();

        // Add elements to the ArrayList
        numbers.add(5);
        numbers.add(2);
        numbers.add(8);
        numbers.add(1);
        numbers.add(9);

        System.out.println("Original ArrayList: " + numbers);

        // Sort the elements in the ArrayList using Bubble Sort
        bubbleSort(numbers);

        System.out.println("Sorted ArrayList: " + numbers);
    }

    public static void bubbleSort(ArrayList<Integer> list) {
    
        int n = list.size();
        boolean swapped;

        for (int i = 0; i < n - 1; i++) {
            swapped = false;
            for (int j = 0; j < n - i - 1; j++) {
                if (list.get(j) > list.get(j + 1)) {
                    // Swap the elements
                    int temp = list.get(j);
                    list.set(j, list.get(j + 1));
                    list.set(j + 1, temp);
                    swapped = true;
                }
            }
            // If no two elements were swapped in the inner loop, the list is already sorted
            if (!swapped) {
                break;
            }
        }
    }
}


28. What are the different storage options available in Android?

    There are several ways to store data locally in an Android application.
    
    1. Shared Preferences:- This is a lightweight storage option for small amounts of key-value pairs. It is commonly used for storing application settings, user preferences, or simple configuration data.
    2. Internal Storage: Each Android application has its private internal storage directory. You can use this storage to save private files that are only accessible by your application.
    3. External Storage: Android devices often have external storage options like an SD card. You can use this storage to store files that can be accessed by other applications or the user.
    4. Room Persistence Library: Room is a powerful persistence library provided by Android Jetpack. It is built on top of SQLite and provides an abstraction layer to work with databases.
    5. SQLite Database: SQLite is a lightweight relational database that is included in the Android framework. It provides a structured and efficient way to store and retrieve structured data.
   
29. Dependency Inject using koin?
    
    Dependency injection is a design pattern that provides the dependency which are required by classes and object, instead of letting them create their own, which helps to make them loosly coupled and leads to improve the code readability and testebility. As creating the stubs and mocks for testing is easy with dependency injection.<br>
    Koin is a lightweight DI framework for Kotlin that simplifies dependency injection in Android applications.<br>
    Define Dependency :- In koin dependency are registered through module which is a logical group of dependencies. for example:- we can define a dependency through network related, UI component or database.<br>
    Register dependencies: Within the module, register the dependencies using the single or factory functions. For example, you can register OkHttpClient as a singleton and Retrofit as a factory.
    Inject dependencies: In your class, declare the dependencies as constructor parameters. Koin will automatically inject the dependencies based on the registered components.

30. Explain the differences between Serializable and Parcelable interfaces in Android?

    Serializable interface: It is a standard Java interface used to serialize an object's state into a byte stream. It is relatively easy to implement but can be          slower and less efficient compared to Parcelable.<br>

   Parcelable interface: It is an Android-specific interface used to serialize an object for efficient IPC (Inter-Process Communication) and is optimized for             performance. It requires a bit more effort to implement but offers better performance.

31. What is the Model-View-Controller (MVC) pattern in Android? How does it work?

     The MVC pattern is a software architectural pattern that separates an application into three main components: Model, View, and Controller.
     Model: Represents the data and business logic of the application.
     View: Displays the user interface and interacts with the user.
     Controller: Handles user input, manipulates the model, and updates the view.
     The controller acts as an intermediary between the model and the view, facilitating communication and ensuring separation of concerns. When a user interacts           with the view, the controller handles the input, updates the model if necessary, and updates the view accordingly.
    
32. What is MVP?

   Model-View-Presenter (MVP) Pattern in Android:<br>
   The MVP pattern is another software architectural pattern used in Android development. It is an evolution of the MVC pattern and aims to separate the presentation     layer from the model and the view.<br>
   Model: Represents the data and business logic of the application.<br>
   View: Displays the user interface and notifies the presenter about user actions.<br>
   Presenter: Acts as an intermediary between the model and the view, handles user actions, updates the view, and manipulates the model.<br>

33. What is MVVM?

    Model-View-ViewModel (MVVM) Pattern in Android:<br>
    The MVVM pattern is a design pattern that separates the user interface (View) from the application logic and data (Model) using a ViewModel as an intermediary.<br>
    Model: Represents the data and business logic of the application.<br>
    View: Displays the user interface and notifies the ViewModel about user actions through data binding or event handling.<br>
    ViewModel: Exposes data and commands to the view, interacts with the model, and performs any necessary transformations or data manipulations.<br>

34. What is Gradle in android?

    A gradle is a automated tool used in android development. It provides a flexible and automated tooling system for compiling the code, updating                         dependencies,running tasks, generating apks.Gradle uses Groovy or Kotlin as its scripting language and offers extensive customization options.


35. What is Jetpack and Jetpack Compose?
    
    Jetpack:- It is a collect of librabries tools and guidelines provided by google for the android app development.It aims to simplify and accelerate android app development by offering the set of components , API that address the common challanges faced by developer.

    JetpackCompose:- It is a recommended mordern toolkit for developing the native UI for android app development provided by google . It allows developer to create user Interface by directly writing the reactive programming, in which we can write our UI hirearchy by defining vartous composable function which makes it easy to develop UI.

36. What is FastLane?
    
    Fastlane is a set of tools that automates various tasks in the mobile app development cycle.It simplifies the processes such as building, testing, deploying the iOS/android apps. It provides the command line interface to define and execute our commands. Making it easier to handle tasks such as  like building app releases, running tests, and submitting apps to app stores.

37. What is RxJava?
    In Android development, RxJava can be used to simplify handling asynchronous tasks such as network requests, database operations, and UI events. It provides a set of operators that allow you to transform, filter, and combine data streams, making it easier to handle complex asynchronous scenarios.<br>

It provides a reactive programming paradigm that enables developers to handle asynchronous operations and data streams in a more declarative and composable way.

38. What is a Room Database?
    
   Room is a lightweight relational database commonly used in Android app development. that provides the abstarct layer over SQLite and compile time checks,support for LiveData and RxJava for reactive programming, and easy integration with other Jetpack components like LiveData and ViewModel.It combines the benefits of SQLite, such as efficient storage and performance, with an easier-to-use interface for developers.

   Entity: An Entity represents a table in the database. It is a plain Java or Kotlin class annotated with the @Entity annotation. Each field in the entity class represents a column in the corresponding database table.

DAO (Data Access Object): The DAO is an interface that defines the database operations (such as insert, update, delete, and query) that can be performed on the entities. It is annotated with the @Dao annotation. Developers write methods in the DAO interface, and Room generates the corresponding implementation.

Database: The Database is an abstract class that represents the SQLite database. It is annotated with the @Database annotation and provides methods to obtain instances of the DAO interfaces. Developers need to define the entities, version number, and other configuration options in the Database class.

Room Database Builder: It is a class that constructs and configures the Room database instance. Developers use the Room.databaseBuilder() method to create an instance of the database by providing the context and the database class.

Type Converters: Room provides the ability to define custom type converters to store complex data types in the database. Type converters are annotated with the @TypeConverter annotation and convert non-primitive types into a format that can be stored in the database.

39. What is coroutines?
    
  Coroutine(background tasks) is a design pattern that we can use in android to simplify code that executes asynchronously(not simultaneous). Or we can say that it is a background thread that allow execution to be suspended and resumed generalizing subroutines for cooperative multitasking.<br>
  
  Coroutines help to manage long-running tasks that might otherwise block the main thread and cause your app to become unresponsive.


40. What is navigation component?

The navigation component is a collection of libraries, plugins and toolings that simplifies android navigation.<br>
when we work with our android apps, when we think about navigation , we simply thinks that navigation is going from one activity to another activity by a button click etc.

But if want to do something complex like doing navigation with bottom navigation bar, in that we need to take care of lot of things like on click of that button the correct page should open and button should get highligted and need to take care care of back- stack in a uniform way, so that pages don't get piled up again and again. so that users dont get confused.<br>
So in cases like this navigation component comes into play.

41. What is the difference between a service and a thread in Android?

A service is a component in Android that performs long-running operations in the background without a user interface. Services are designed to execute tasks that should continue even when the user switches to a different application or leaves the application altogether. They are often used for tasks such as playing music, handling network requests, or performing periodic data synchronization. Services are started by invoking startService() or bound to using bindService() methods.


A thread, on the other hand, is a basic unit of execution within a process. In Android, threads are used to perform concurrent or parallel processing. By default, Android applications have a single thread of execution called the "main" thread or UI thread, which is responsible for handling user interactions and updating the user interface.


42. Given an array of integers nums and an integer target, return indices of the two numbers such that they add up to target.

You may assume that each input would have exactly one solution, and you may not use the same element twice.

You can return the answer in any order.

 

Two Sum

Input: nums = [2,7,11,15], target = 9
Output: [0,1]
Explanation: Because nums[0] + nums[1] == 9, we return [0, 1].
Example 2:

Input: nums = [3,2,4], target = 6
Output: [1,2]
Example 3:

Input: nums = [3,3], target = 6
Output: [0,1]
 

Constraints:

2 <= nums.length <= 104
-109 <= nums[i] <= 109
-109 <= target <= 109
Only one valid answer exists.

solution:-

class Solution {

    public int[] twoSum(int[] nums, int target) {
        for(int i=0; i< nums.length; i++){
            for(int j= i+1; j<nums.length; j++){
            
            
            if(target == nums[i] + nums[j]){
                return new int []{i,j};
            }
        }
       
    }
     return new int[] {};
}
}

43. How does data binding work in Android? What are its benefits?

    DataBinding:- It is a technique that allows you to bind the UI components to the XML layout files directly with your data model, such as Live data. It reduces the manual addition of findViewById() which is a boiler code and reduces the performance of the code.



   
    
    
    
  
      
   

   
