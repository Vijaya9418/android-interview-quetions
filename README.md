# android-basic-quetions

1. What is android?

   Android is an operating system specifically designed for mobile and tab applications, its a kind of software stack for mobile applications which is developed by google.
   It is a linux kernel and provide a framework for devlopers to develop the android applications and softwares that can run on android powered devices.
   

3. What is android framework?

   Android framework is a key component of android operating system, which provides API (Application programming interface), and various tools which are used by developer to      build applications and to interact with various functionalities of android device.<br>

   It provides various components and services that facilitate app development such as, activity manager, content provider etc.

4. Define android architecture?

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

5. Define android components?

   There are basically 4 basic components in android:-

   Activity:- It represents the single screen of UI component and with which the user interacts with, It helps the user to navigate from one activity to another and perform some action.<br>
   
   Service:- It is used for performing the long running tasks/background tasks or which does not required intercation with UI.<br>
   
   Broadcast receivers:- It is basically used for receiving and responding to the messages or broadcasting the messages.<br>
   
   Content provider:- It is used for managing the intercation between different applications.They can be used to start activities, launch services, broadcast messages, or pass data between components.<br>

6. Define intent and its types.

   Intents are basically a messaging system that is use to interaction with components, within the application or with other applications. It can be seen as abstract discription of an operation to be performed.<br>
   
   There are two types of intents:-
   Explicit intent:- Whhich is basically use to interact with inner part of the application. for example if you want to send the data from one activity to another within the      application or you want to go from one activity to another, explicit intents are used.

   Implicit intent:- It is used to interact with outer part of the application. For example if we want to open a phone dial with from our application.or if you want to share      an image from your application.

7. Define activity Lifecycle:-

   It is several events or stages with which an activity goes through in an application. Activity lifecycle is consits of seven stages.:-

   1. OnCreate:-It is the very first stage where the activity is created.
   2. OnStart:- It is the second stage where the activity starts, when the activity becomes visible to the user.
   3. OnResume:- It is called when the activity is about to start interacting with the users.
   4. OnPause:- It is called when the activity is about to loose focus.
   5. OnStop:- It is called when the acitivity is no longer visible to the user, but there in the background.
   6. OnRestart:- It is called when the activity is restarted after being stopped.
   7. OnDestroy :- It is called when the activity is removed from the background.
  
8. What are OOPs concept?

   Object oriented programming is a software design pattern that is revlovs abround object and classes which provides the reuseability, readability to improve the performance.
   It sits on four pillars, which are :-
   
   Inheritance:- It is the ability of a class to inherit the property of its parent class.for example:- a child can inherit the property of parents. Or an activity by extending the Activity class or one of its subclasses, such as AppCompatActivity or FragmentActivity. By doing so, they inherit all the functionalities and behaviors of the base class while having the flexibility to add their specific functionality.
   
   Abstract:- It is used to hide most of the information and to show only the relevant information to the user. for example:- ATM. or a View in android
   View class is a fundamental building block for creating user interfaces. It represents UI elements such as buttons, text fields, images, and more. The View class itself is an abstract class, and developers typically use its subclasses to create specific UI elements.
   
   Encapsulation:- It is the process of bundling the data(attribute) and methods(behaviour) together and get the full access through them with the help of access modifier public, protected and private. We also use getter and setters which helps in data hiding and maintaining the inetrgrity of the data.
   he usage of private fields and public getter and setter methods to control access to the data in a data model class.
   
   PolyMorphism:- It comprises of two words poly means many and morphism means form, so it is the ability of an objcet to take multiple forms, which we can achieve by overloading and overrriding.  onClick() method in event handling for various UI elements, such as buttons. because it can be overridden in different classes to handle events for different UI elements.

10. Define overloading and overriding?
   
   Overloading:- It is also called run time polymorphism in which meathod have same name , but differ in parameters. It can be differ in the number of params or the type of params.
   
   Overriding:- It is also called compile time polymorphism in which a sub class has the same method name as that of the super class, but the implementation is differnt.

11. what are the types of service?
    
    There are two types of service:-
   
   Started Service:- this is the service which starts explicitly and which may take longer time to complete such as downloading the file from server.<br>
   It continues to run in the background until the task is completed even after the associated activity is destroyed.

   Bound Service:- this is a service when multiple component need to interact with a service, typically bindService() method.<br>
   When all the components unbind from the service, the service is destroyed and stopped.


11. What are the types of content providers?
    
    there are two types of content providers:-

    Custom Content provider:- These are the content provider which are created by the Developers to share data between different applications or components within the application.Developers define their own Content Provider by subclassing the ContentProvider class and implementing the necessary methods to handle data operations.

    System Content provider:- These are the providers which are provided by android system.It manages and provide access to various system data such as contact, media, files      and settings.These Content Providers are part of the Android framework and are responsible for maintaining and exposing system-related data to applications.

12. What is intent filter?
    
   Intent filter is the key component which is use to declare what type of intent an application or component can handle.It is defined using intent-related attributes in the 
   AndroidManifest.xml file.
   
   Its key attribute are:-
   Action:- It provides action or actions that a component can respond to, It is basically an string representing desired operations.such as "android.intent.action.VIEW" or "android.intent.action.SEND".<br>
   Category:-Categories provide additional information about the component's purpose or behavior. such as android.intent.category.DEFAULT or "android.intent.category.BROWSABLE".<br>
   Data: Specifies the data type or scheme that the component can handle. It can include attributes like the data MIME type or a specific data scheme. For example, an activity can specify that it can handle "http" URLs or image files.<br>

13. Define fragment and its lifecycle?
14. 
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

15. What is the lifecycle of Service?

    onCreate(): This method is called when the service is first created.<br>
    onStartCommand(): This method is called when a client calls startService() to start the service.<br>
    onBind(): This method is called when a client calls bindService() to bind to the service.<br>
    onUnbind(): This method is called when all clients have disconnected from the service by calling unbindService().<br>
    onRebind(): This method is called when a new client binds to the service after onUnbind() has been called.<br>
    onDestroy(): This method is called when the service is about to be destroyed.<br>

16. A service that was initially started with onStartCommand by a calling startService can still receive a call to _____. when a client calls bindService.

    The onBind() method allows clients to bind to the service and communicate with it through an interface defined by an IBinder. By implementing onBind(), the service 
    provides a way for clients to access its functionality and establish a connection with it.
    So, even if a service is started with startService(), clients can still bind to it using bindService() and interact with it through the returned IBinder object.

17. What is anr?
    
    ANR is application not responding which is an error condition that occurs when the user interface of an application becomes unresponsive and user is not able to
    interact with it. When an ANR occurs, the system displays a dialog to the user, notifying them that the application has stopped responding and giving them the option to       close it.<br>
    It can be caused by long running tasks in the main thread, deadlocks, excessive CPU or memory usage.

18. What is a Deadlock?

    A deadklock occurs when multiple thread wait for other threads to release their resources, resulting in the deadlock state where none of them can proceed.

19. What is bundle?
    
    A bundle is acontainer that holds the key-value pairs, similar to dictionary or map. It is commonly used for passing data between different components, within
    application such as between fragment and activity.

20. what is Context in android?
    
    A Context is an essential class in android that provides access to various resources and system level operations within the application. It repeasents the current state
    and environment in which the application is running.Context is typically obtained from the Android framework and is passed to different components, such as activities,        services, and broadcast receivers, to access system resources and perform operations.

21. what are the types of context?
    
    1. Application context:- It is associated with entire life cycle of the application, which can be called useing getApplicationContext(), It should be used wherever
       the context is not tightly coupled to any specific conponent such as activity, service etc.
       
    3. Activity Lifecycle:- It is specific to particular activity and tied to the lifecycle of that service.It can be acessed within the activity using this keyword.
       The Activity Context should be used when you need a Context that is closely related to the current activity, such as creating views, inflating layouts etc.
       
    3.Service context:-The Service Context is specific to a particular service and is tied to the lifecycle of that service.It can be accessed within a service using the this keyword or ServiceName.this.The Service Context should be used when you need a Context that is closely related to the current service, such as accessing service-specific resources, starting new activities, or accessing service-related services.

22. What is manifest?

    A manifest file is an essential file that provides an important information about your application. It contains various key components such as service and the permission which your app needs, launching configuration of your app, package name, intent filter etc.

23. What is adb?

    ADB(Android Debug Bridge) it is a command-line tool which helps to communicate between your computer and android emulator or device. It is a part of SDK(Software Development kit) used for mainly debugging and testing the android devices.
    1. Debugging and Logging:
    2. Application Installation and Management:
    3. File Transfer:

24. Difference between abstract and Interface?

    Abstract:-<br>
    An abstract class in java cannot be instantiated , it means we cannot create the object directly from it.
    It can contain both abstract and not abstract methods. Abstarct methods are declared without an implementation and must be implemented by its subclass.
    Subclasses of an abstract class must either implement all the abstract methods or be declared as abstract themselves.


    Interface:-<br>
    An interface in java is a collection of abstarct methods and constand variables.It defines a contract or rule of how a clss should behave.
    It serves a way to acheive multiple inheritance as in java a class can implement multiple interface.
    All methods in an interface are public and abstract by default.

    Differences:
    
    Implementation: A class can extend only one abstract class, but it can implement multiple interfaces.<br>
    Abstract classes can have both abstract and non-abstract methods with complete implementations. Interfaces can only have abstract methods.<br>
    Access Modifiers: Abstract class methods can have different access modifiers (public, private, protected), while interface methods are implicitly public.<br>
    Variables: Abstract classes can have member variables, while interfaces can only have constant variables (static final variables).<br>

25. Collections in java?

   In java, Collection framework provides a set of classes and interface for working with group of objects.It provides basic operations like adding, removing and queuing of elements.

25. What is an exception?
    
    An exception is an event that occurs during the execution of a program that disrupts the original flow of a program.Exceptions are use to handle, errors,              exception conditions. The java language provides build-in handling exception mechanism to deal with this type of situation.<br>
    
    Exception Hierarchy:
      Exceptions in Java are organized in a hierarchical structure, with the base class being java.lang.Throwable.
      Throwable has two main subclasses: Exception and Error.

    Exception Handling:

      Exception handling is the process of catching and handling exceptions to prevent program termination and provide meaningful feedback to the user.
      The try-catch-finally block is used to handle exceptions. The try block contains the code that may throw an exception, the catch block catches and handles the         exception, and the finally block is executed regardless of whether an exception occurs or not.

27. Sort the list of elements using bubble sort?
    
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

31. Explain the differences between Serializable and Parcelable interfaces in Android?

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

    advantages:-

Testability: MVVM's separation of concerns also leads to improved testability. With clearly defined responsibilities for each component, unit testing becomes more straightforward. ViewModel, in particular, can be easily tested without the need for complex UI testing frameworks, as it does not have direct dependencies on the Android framework.

Data Binding: MVVM often goes hand-in-hand with data binding frameworks (like Android's Data Binding or libraries in other platforms). Data binding allows for declarative UI updates, where the UI components automatically update themselves when underlying data changes. This reduces the need for manual UI updates and event handling, leading to more concise and readable code.

Reduced Boilerplate Code: MVVM, when combined with data binding and LiveData, significantly reduces boilerplate code. It minimizes the amount of code needed to propagate data changes to the UI, handle configuration changes, and manage UI state. This leads to more concise, maintainable, and readable codebase.

Adaptability to Reactive Programming: MVVM works well with reactive programming principles. LiveData and other reactive components enable a more reactive approach to handling data flows and UI updates, making it easier to handle complex asynchronous operations.

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


dependencies {

    implementation 'io.reactivex.rxjava3:rxandroid:3.0.0'
    implementation 'io.reactivex.rxjava3:rxjava:3.1.1'
    implementation 'com.squareup.retrofit2:retrofit:2.9.0'
    implementation 'com.squareup.retrofit2:converter-gson:2.9.0'
}

Define a data model to hold the fetched data (Same as the previous example):

data class Post(val id: Int, val title: String, val body: String)


Create a Retrofit service to make API calls (Same as the previous example):

interface ApiService {

    @GET("posts")
    fun getPosts(): Single<List<Post>>
}


Fetch the data using RxJava in your MainActivity:

class MainActivity : AppCompatActivity() {

    private val apiService: ApiService by lazy {
        Retrofit.Builder()
            .baseUrl("https://jsonplaceholder.typicode.com/")
            .addConverterFactory(GsonConverterFactory.create())
            .addCallAdapterFactory(RxJava3CallAdapterFactory.create())
            .build()
            .create(ApiService::class.java)
    }

    override fun onCreate(savedInstanceState: Bundle?) {
        super.onCreate(savedInstanceState)
        setContentView(R.layout.activity_main)

        // Use RxJava to fetch data
        apiService.getPosts()
            .subscribeOn(Schedulers.io())
            .observeOn(AndroidSchedulers.mainThread())
            .subscribe(
                { posts -> displayPosts(posts) },
                { error -> showError() }
            )
            .addTo(CompositeDisposable())
    }

    private fun displayPosts(posts: List<Post>) {
        // Update UI with fetched data
        // ...
    }

    private fun showError() {
        Toast.makeText(this, "Error fetching data", Toast.LENGTH_SHORT).show()
    }

    private val compositeDisposable = CompositeDisposable()

    override fun onDestroy() {
        super.onDestroy()
        compositeDisposable.clear()
    }
}

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


   One real-time example of using coroutines in Android is to perform asynchronous tasks, such as making network requests, without blocking the main UI thread.

   1. Set up the necessary dependencies in your project's build.gradle file:

      dependencies {
      
    implementation 'org.jetbrains.kotlinx:kotlinx-coroutines-android:1.5.1'
    implementation 'com.squareup.retrofit2:retrofit:2.9.0'
    implementation 'com.squareup.retrofit2:converter-gson:2.9.0'
}

2. Define a data model to hold the fetched data:

data class Post(val id: Int, val title: String, val body: String)

3. Create a Retrofit service to make API calls:

interface ApiService {

    @GET("posts")
    suspend fun getPosts(): List<Post>
}

4. Fetch the data using coroutines in your MainActivity:

class MainActivity : AppCompatActivity() {

    private val apiService: ApiService by lazy {
        Retrofit.Builder()
            .baseUrl("https://jsonplaceholder.typicode.com/")
            .addConverterFactory(GsonConverterFactory.create())
            .build()
            .create(ApiService::class.java)
    }

    override fun onCreate(savedInstanceState: Bundle?) {
        super.onCreate(savedInstanceState)
        setContentView(R.layout.activity_main)

        // Use coroutines to fetch data
        CoroutineScope(Dispatchers.Main).launch {
            try {
                val posts = withContext(Dispatchers.IO) {
                    apiService.getPosts()
                }
                displayPosts(posts)
            } catch (e: Exception) {
                Toast.makeText(this@MainActivity, "Error fetching data", Toast.LENGTH_SHORT).show()
            }
        }
    }

    private fun displayPosts(posts: List<Post>) {
        // Update UI with fetched data
        // ...
    }
}





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

 

Two Sum<br>

Input: nums = [2,7,11,15], target = 9<br>
Output: [0,1]<br>
Explanation: Because nums[0] + nums[1] == 9, we return [0, 1].<br>
Example 2:<br>

Input: nums = [3,2,4], target = 6<br>
Output: [1,2]<br>
Example 3:<br>

Input: nums = [3,3], target = 6<br>
Output: [0,1]<br>
 

Constraints:

2 <= nums.length <= 104<br>
-109 <= nums[i] <= 109<br>
-109 <= target <= 109<br>
Only one valid answer exists.<br>

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

44. Extention function in android?

   It is a powerful feature provided by kotlin programming language that helps the developer to add new functions to exixting classes, without modifying the source code along with android framework.It provides the convinent way to extend the functionality of classes for better readabillity and reusability.

   Example for creating an extension function for a toast message:-
   
   fun Context.showToast(message: String, duration: Int = Toast.LENGTH_SHORT) {
   
    Toast.makeText(this, message, duration).show()
    
}

class MainActivity : AppCompatActivity() {

    override fun onCreate(savedInstanceState: Bundle?) {
    
        super.onCreate(savedInstanceState)
        
        setContentView(R.layout.activity_main)

        // Calling the extension function on the Context class (in this case, the Activity)
        
        showToast("Hello, World!")
    }
    
}

45. What are high order function in kotlin?

   It is a concept in programming language that can take one or more function as its parameter or can return it as aresult. So these functions are often reffered as callback functions or a function argument.  A high-order function can generate and return a new function as its result. The returned function can be assigned to a variable or used immediately.

High-order functions provide a powerful way to abstract and encapsulate behavior in functional programming paradigms. They enable code reusability, modularity, and the creation of more expressive and flexible code structures. Common examples of high-order functions include map, filter, and reduce in functional programming languages like JavaScript and Python.

46. What is open keyword in kotlin?
      
   Open keyword is use to declare a class, function or property for extension or overriding. By default, classes and their members in Kotlin are final, meaning they cannot be inherited or overridden. However, when a class, function, or property is marked as open, it allows other classes to inherit from it or override its behavior.



   Example:-

open class Animal {

    open fun makeSound() {
    
        println("The animal makes a sound")
        
    }
}

class Cat : Animal() {

    override fun makeSound() {
    
        println("Meow!")
        
    }
}

47. What is companion object?

    Companion object acts as a container fo static members in kotlin just as the static members in other programming lanugage. A companion object is defined inside a class and is declared using the companion keyword.Members of the companion object can be accessed using the class name without creating an instance of the class.


class MyClass {

    companion object {
        const val constantValue = 42
        
        fun doSomething() {
            println("Doing something...")
        }
    }
}

// Accessing companion object members

val value = MyClass.constantValue

MyClass.doSomething()

48. What is Retain Fragment?
    
   It refers to a fragment that is reserved across configuration changes such as screenshot rotation and remains alive when the associated fragment is destroyed and recreated. It allows data and state to be retained during the recreation of the activity.


49. RestFul API's?
   
   RESTful APIs (Representational State Transfer) are commonly used to communicate with remote servers or web services. RESTful APIs follow a set of principles and conventions for creating, accessing, updating, and deleting resources over HTTP. Here's an overview of using RESTful APIs in Android:

   HTTP Client: Android provides built-in classes and libraries, such as HttpURLConnection or OkHttpClient, to make HTTP requests and interact with RESTful APIs. These classes handle establishing connections, sending requests (GET, POST, PUT, DELETE), and receiving responses.

URL Endpoints: RESTful APIs typically expose different endpoints (URLs) for different resources or actions. You need to identify the appropriate endpoint(s) for the specific operations you want to perform, such as retrieving data, submitting data, or updating resources.


50. Key Performance Indicator(KPI) definition?
    
    KPI(Key Performance Indicator) is a measurable metrics which measures or evaluate the progress of an organization, project or particular metrics. It is tried to specific objective or outcome and are use to track and monoitor the performance.
    
Example KPI: Average Order Value (AOV)

Definition: The average value of each customer order placed within a specific time period.

60. System Architecture?

System architecture refers to the structural design and organization of a software system or application. It defines the components, modules, relationships, and interactions between different parts of the system, as well as the principles and guidelines governing their design and implementation. The system architecture provides a blueprint for how the system's functionality is divided, how components communicate and interact, and how the system satisfies its requirements.


Key aspects of system architecture include:

Components:<br>
Communication and Integration:<br>
Dependencies and Relationships:<br>
Data Management:<br>
Scalability and Performance:<br>
Security and Reliability:<br>

61. how many types of dialog boxes are their in android?

   AlertDialog: This is a versatile dialog box that can display a title, message, and optional buttons for actions or choices.

   ProgressDialog: This dialog is used to show the progress of a long-running operation. It typically includes a progress bar or a spinning wheel and may display a message.

   DatePickerDialog: This dialog allows the user to select a date from a calendar-like interface.

   TimePickerDialog: This dialog enables the user to pick a specific time using a clock-like interface.

   BottomSheetDialog: This is a dialog that slides up from the bottom of the screen, typically used to display additional options or actions.

   Custom Dialogs: Android also allows developers to create custom dialog boxes by extending the Dialog class and designing a custom layout.


62. Integer starting at 0 are serialised in a sequence in the following format 0123456779..... Each digit represents a position in the sequence for example position 0: digit 0 position 5: digit 5 position position 11: digit 0 write a function that returns a digit given a position in java for all the scenarios not only for given example.





63. Difference between XML and JSON?


         1. Full Form:- XML**(Extensible Markup Language)** whereas JSON is **(Javascript Object Notation)**.<br>
         2. Syntax:- XML uses a **<tag>** format to define an element whereas JSON uses the key-value pair seperated by colon  **({ "key": "value" })**.<br>
         3. Readability:- JSON has a more compact and human-readable syntax compared to XML. JSON uses plain text and does not require closing tags, making it easier to read and write            by humans. XML, on the other hand, can be more verbose due to its tag structure.<br>
         4. Parsing and Processing:- JSON can be directly parsed into JavaScript objects, while XML requires parsing and traversal using XML parsers.<br>
         5. Usage: XML has been widely used for creating UI's in android development, document markup and data exchange, particularly in industries like publishing and finance. JSON,             originally developed for JavaScript, has become popular for web APIs and data interchange in modern web development.<br>


64. How many types of joins are their in SQL?


         Inner Join: Retrieves records that have matching values in both tables being joined. It returns only the rows where the join condition is satisfied.<br>

         Left Join (or Left Outer Join): Returns all records from the left (or first) table and the matched records from the right (or second) table. If there are no matches, it returns          NULL values for the columns of the right table.<br>

         Right Join (or Right Outer Join): Returns all records from the right (or second) table and the matched records from the left (or first) table. If there are no matches, it                returns NULL values for the columns of the left table.<br>

         Full Join (or Full Outer Join): Returns all records when there is a match in either the left or right table. If there are no matches, it returns NULL values for the columns of           the non-matching table.<br>

         Cross Join (or Cartesian Join): Produces the Cartesian product of the two tables, resulting in all possible combinations of rows from both tables. It doesn't require a join              condition.<br>

         Self Join: Joins a table with itself, treating it as two separate tables, typically using an alias to differentiate between the two instances of the same table.<br>


65. How to find any view element into your program in android?

         View View = (View) LayoutInflater.from(ctx).inflate(R.layout.preference_layout);<br>
         EdidText editText = view.findViewById(R.id.description);<br>
         builder.setView(view);<br>

66. Binary Search?


class HelloWorld {
    
       public static int search(int []nums, int target) {
        //Your code goes here
        int n = nums.length;
        int left = 0;
        int right = n-1;



    while(right>=left){
                int mid = left+(right-left)/2;
        if(target> nums[mid]){
            left = mid + 1;
        }
        else if (target < nums[mid]){
            right = mid - 1;
        }
        else{
            return mid;
        }
    }
    
return -1;

    }
    
    public static void main(String[] args) {
      int  arr[] = {1, 3, 7, 9, 11, 12, 45};
        search(arr,3);
        System.out.println(search(arr,3));
    }
    
}

67. Find the largest element in an array?

public class LargestElement {

    public static void main(String[] args) {
        int[] array = {10, 20, 30, 40, 50, 60};
        
        // Assume the first element is the largest
        int largest = array[0];
        
        // Iterate through the array to find the largest element
        for (int i = 1; i < array.length; i++) {
            if (array[i] > largest) {
                largest = array[i];
            }
        }
        
        // Print the largest element
        System.out.println("The largest element in the array is: " + largest);
    }
}

68. Find the salary of an employee whose salary is greater than 50000.

public class Salary {

    public static void main(String[] args) {

    List<Employee> emp = new ArrayList();
    emp.add(new Employee("Vijaya", 10000);
    emp.add(new Employee("Vijaya", 20000);
    emp.add(new Employee("Vijaya", 60000);
    
      emp.stream.filter( em -> em.getSalary() > 50000).foreach(System.out.println));
      
        }
}

69. What are composable funstions?

   Composable functions refers to the specific feature in jetpack compose which is used for creating the UI in android. It is basically a chain of functions, in which we can use one        function inside another function.

      1. Composable functions allow you to describe the UI components and their behavior declaratively. 
      2. UI components are defined as composable functions. Each composable function represents a self-contained UI element, such as a button, text field, or screen layout.
      3.  Composable functions can be nested and combined to create complex UI hierarchies. 


70. What are data class in android?

      Data Class in android are special feature which is use to represent and hold the data in a concise way. It is primarly use for storing the data does not contain the business 
      logic. Data classes automatically generate useful methods, such as equals(), hashCode(), toString(), and copy(), based on the properties defined in the class.


71. Write the sample code in the pattern of MVVM?

    Model(Data Layer):-

      // Assume we have a User data class representing user information
    
      data class User(val id: Int, val name: String, val email: String)

     // Assume we have a UserRepository responsible for managing user data

       class UserRepository {
    
         // Simulated database or network operations
        fun getUser(userId: Int): User {
        // Retrieve user data from the database or network
        return User(1, "John Doe", "johndoe@example.com")
    }
}


 View(UI layer):-

     import androidx.appcompat.app.AppCompatActivity
     import android.os.Bundle
     import androidx.activity.viewModels

    class MainActivity : AppCompatActivity() {

    private val viewModel: UserViewModel by viewModels()

    override fun onCreate(savedInstanceState: Bundle?) {
        super.onCreate(savedInstanceState)
        setContentView(R.layout.activity_main)

        val userId = 1
        viewModel.loadUser(userId)

        // Observe the LiveData from the ViewModel and update the UI accordingly
        viewModel.user.observe(this) { user ->
            // Update the UI with the user data
            textViewUserName.text = user.name
            textViewUserEmail.text = user.email
        }
    }
}
    

ViewModel (Presentation Layer):-

    import androidx.lifecycle.LiveData
    import androidx.lifecycle.MutableLiveData
    import androidx.lifecycle.ViewModel

    class UserViewModel(private val userRepository: UserRepository) : ViewModel() {
    
    private val _user = MutableLiveData<User>()
    val user: LiveData<User> get() = _user

    fun loadUser(userId: Int) {
        // Simulated asynchronous data retrieval
        val fetchedUser = userRepository.getUser(userId)
        _user.value = fetchedUser
    }
}


72. What is CI/CD?

    CI/CD is Contineous Integration/ Continueous Deployment, which is a set of practices and tools that automates the process of testing, debugging and deploying the software                changes to the production.
    CI/CD piplelines are implemented using various tools such as git, sourcetree, bitbucket. So it oftehn trigger the pipelines whenever there is a change done by Developers.

     CI:- CI focuses on merging code changes from multiple developers into a shared repository frequently, typically several times a day.
     CD:- CD is an extension of CI that focuses on automating the release and deployment of software changes to production environments.


73. How do you define abstract class in android?

    It is defined using abstract keyword. It allows you to define the coomon behaviour and properties that can be inherited by its subclasses, but it cannot be instantiated by its own.

          syntax:-

         abstract class AbstractClassName();

          example:-

          abstract class Shape(){
    
               abstract fun calculateArea():Double
             }
                class Rectangle(val w, val h){
                override fun calculateArea():Double{
                return w*h
             }
          }
          fun main(){
          val rec = Rectangle(5.0,3.0)
          rec.printDescription()
          val rea = rec.calculateArea();


75. What is the purpose of 'when' in kotlin?

   In kotlin the purpose of when is to replace the switch statement or keyword in other programming language such as switch keyword. It allows you to perform brancing based on the value of an expression.

   example:-

         val num = 5;
         val rsult = when(num){
            1 -> "One"
            2 -> "Two"
            3 -> "Three"
         else -> "Other"
      }
      
76. How to create a list in kotlin?

   A list in kotlin can be created using **listOf()** or **mutableListOf()** function.

   listOf() function is to create an immutable list. Once created the list cannot be added,removed or changed.

      example:- val myLis = listOf("apple","banana");

   mutableListOf() function allows you to modify the list by adding,removing or chainging elements.

     example:- val myLis = mutableListOf("apple","banana","mango");


77. What is the purpose of let keyword in kotlin?

   A let function is a scoping function that provides a concise way to perform operation on nullable objects or objects within certain scope.Its primary purpose is to avoid nullability issue and execute the block of code onl when a non-null object is encountered.

      val nullableString:String? = "Hello";
      nullableString?.let{
      val length = it.length
      println("the length is $length")
      }


78. What is the purpose of android asset studio?

    The android asset studio is a web based tool which is provided by google that helps developer to create graphic assets for their android appliaction. It basically helps you to simplify the process of generation of common app iocns,launcher icon, and other graphic resources. It helps to save time and effort in creating and managing graphical assests.


79. Which android jetpack library is used to simplify the database access?

      Room library which is a part of android jetpack component and provides the abstraction layer over a sqlite, making it easier to work with database.


80. Which library is use to manage the image loading and caching?

   Glide is a powerful and flexible library that simplifies the process of loading images from various sources such as URLs, local storage, or resources  efficirntly caching them from improved performance.

81. What is recyclerview ?

In Android, RecyclerView is a more advanced and flexible version of ListView and GridView. It's a powerful UI component used to efficiently display large lists or grids of items, providing features such as item recycling, data binding, and customizable layouts. Here's an example of how to use RecyclerView in Android.

class MyAdapter(private val dataList: List<String>) : RecyclerView.Adapter<MyAdapter.ViewHolder>() {
    
    override fun onCreateViewHolder(parent: ViewGroup, viewType: Int): ViewHolder {
        val view = LayoutInflater.from(parent.context).inflate(R.layout.item_list, parent, false)
        return ViewHolder(view)
    }

    override fun onBindViewHolder(holder: ViewHolder, position: Int) {
        val item = dataList[position]
        holder.bind(item)
    }

    override fun getItemCount(): Int {
        return dataList.size
    }

    inner class ViewHolder(itemView: View) : RecyclerView.ViewHolder(itemView) {
        private val textView: TextView = itemView.findViewById(R.id.item_text_view)

        fun bind(item: String) {
            textView.text = item
        }
    }
}
Implement the necessary methods such as onCreateViewHolder, onBindViewHolder, and getItemCount.<br>
In onCreateViewHolder, inflate the item_list.xml layout file and return a new instance of a custom ViewHolder that holds references to the UI elements.<br>
In onBindViewHolder, bind the data to the UI elements of the ViewHolder based on the item position in the data list.<br>

82. What is pending Intent ?
    
   Pending Intent in android is a token that represents the future intent. It allows you to start an operation or an activity or service at a later point of time. even if your application is not running or the component (e.g., activity, service) you want to start is not currently instantiated.

      Alarm and Notification: You can schedule an Intent to be fired at a specific time or in response to a particular event, such as a timer or an incoming notification.

      Starting Activities or Services: You can create a PendingIntent to launch an activity or start a service at a later time or in response to an external trigger, such as a user action or a system event.

      Broadcasting Intents: PendingIntent can be used to broadcast an Intent to other components or applications. This allows you to trigger actions or events across different parts of the system.

      Background Operations: PendingIntent is commonly used for performing background tasks or operations, such as downloading data or performing periodic updates, even when the application is not in the foreground.

   **   alarmIntentRTC = PendingIntent.getBroadcast(context, ALARM_TYPE_RTC, intent, PendingIntent.FLAG_MUTABLE | PendingIntent.FLAG_UPDATE_CURRENT);**
   
         context – The Context in which this PendingIntent should perform the broadcast. 
         requestCode – Private request code for the sender 
         intent – The Intent to be broadcast.


83. Dragger and Hilt?
    
**Dagger:**

Dagger is a popular dependency injection (DI) framework for Java and Android development. It helps manage the dependencies between different components in an application and promotes the principles of Inversion of Control (IoC) and Dependency Injection (DI). By using Dagger, you can create modular, maintainable, and testable code.

Real-time Example:
Let's consider an example of a simple Android application with two classes: Car and Engine. The Car class depends on the Engine class to run. Without using Dagger, you might directly instantiate the Engine class inside the Car class, leading to tight coupling between the two.

Without Dagger (Direct instantiation):


public class Car {

    private Engine engine;

    public Car() {
        engine = new Engine();
    }

    // ...rest of the Car class implementation
}


with Dagger:-

public class Car {

    private Engine engine;

    @Inject
    public Car(Engine engine) {
        this.engine = engine;
    }

    // ...rest of the Car class implementation
}

In the Dagger example, we use the @Inject annotation to tell Dagger that the Car class depends on the Engine class. With this setup, Dagger will automatically create and provide an instance of Engine when creating a Car object. This way, you decouple the Car class from directly creating the Engine instance, making the code more maintainable and easier to test.


**Hilt:-**

Hilt is a dependency injection library built on top of Dagger, specifically designed for Android development. It simplifies the process of setting up and using Dagger in Android apps by providing integration with Android components like activities, fragments, services, etc. Hilt uses annotations and code generation to create and manage dependency injection.

Step 1: Set up Hilt in your project by adding the necessary dependencies and annotations.

Step 2: Create a module that provides the dependencies (in this case, the Engine class).

@Module
@InstallIn(ApplicationComponent.class)
public class EngineModule {

    @Provides
    public Engine provideEngine() {
        return new Engine();
    }
    
}


Step 3: Annotate the Car class with @Inject, and Hilt will automatically provide the Engine dependency.

public class Car {

    private Engine engine;

    @Inject
    public Car(Engine engine) {
        this.engine = engine;
    }

    // ...rest of the Car class implementation
}

By using Hilt, you get the benefits of Dagger while reducing boilerplate code, improving readability, and simplifying the setup process for Android-specific components.


84 What is multiThreading?

Multithreading is a programming concept that allows multiple threads to execute concurrently within the same process. Threads are individual units of a program that can perform tasks independently. Multithreading enables the execution of multiple tasks simultaneously, taking advantage of modern multi-core processors and improving the overall performance and responsiveness of an application.

Java and Kotlin:

In both Java and Kotlin, multithreading is achieved through classes and interfaces provided by the Java Concurrency API. One of the most common ways to create a thread is by extending the Thread class or implementing the Runnable interface. Here's a brief example of multithreading in Java and Kotlin:

// Java
public class MyThread extends Thread {

    @Override
    public void run() {
        // Code to be executed by the thread
        for (int i = 0; i < 5; i++) {
            System.out.println("Thread " + Thread.currentThread().getId() + ": " + i);
        }
    }
}

// Kotlin

class MyRunnable : Runnable {

    override fun run() {
        // Code to be executed by the thread
        for (i in 0 until 5) {
            println("Thread ${Thread.currentThread().id}: $i")
        }
    }
}

fun main() {

    // Java
    MyThread().start(); // Start a new thread

    // Kotlin
    val myRunnable = MyRunnable()
    Thread(myRunnable).start() // Start a new thread using the Runnable interface
}

Android provides several mechanisms to achieve multithreading, such as using Thread, AsyncTask, HandlerThread, and more recently, ExecutorService or Kotlin coroutines.




   









 
   
    


   



   
    
    
    
  
      
   

   
