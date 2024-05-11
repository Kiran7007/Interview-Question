# Interview-Question

## Contents
 * [Data Structures And Algorithms](#data-structures-and-algorithms)
 * [Core Java](#core-java)
 * [Core Android](#core-android)
 * [Architecture](#architecture)
 * [Design Problem](#design-problem)
 * [Tools And Technologies](#tools-and-technologies)
 * [Android Test Driven Development](#android-test-driven-development)
 * [Others](#others)
    
* **What is `Application` class?**
    - The Application class in Android is the base class within an Android app that contains all other components such as activities and services. The Application class, or any subclass of the Application class, is instantiated before any other class when the process for your application/package is created.

#### Activity and Fragment
* **What is onSavedInstanceState() and onRestoreInstanceState() in activity?**
    - onSavedInstanceState() - This method is used to store data before pausing the activity.
    - onRestoreInstanceState() - This method is used to recover the saved state of an activity when the activity is recreated after destruction. So, the onRestoreInstanceState() receive the bundle that contains the instance state information.

* **When should you use a Fragment rather than an Activity?**
    - When you have some UI components to be used across various activities
    - When multiple view can be displayed side by side just like viewPager

* **What is the difference between FragmentPagerAdapter vs FragmentStatePagerAdapter?**
    - FragmentPagerAdapter: Each fragment visited by the user will be stored in the memory but the view will be destroyed. When the page is revisited, then the view will be created not the instance of the fragment.
    - FragmentStatePagerAdapter: Here, the fragment instance will be destroyed when it is not visible to the user, except the saved state of the fragment.

* **What is the difference between adding/replacing fragment in backstack?**
    ![image](https://user-images.githubusercontent.com/18071333/109423939-88001a80-7a07-11eb-995e-b7d16c5e51bb.png)
    ![image](https://user-images.githubusercontent.com/18071333/109423948-95b5a000-7a07-11eb-8aa6-840f01beb236.png)
    ![image](https://user-images.githubusercontent.com/18071333/109423954-9d754480-7a07-11eb-9e45-ea95fa038feb.png)
    <br>
    <p align="center">
        <img src="https://user-images.githubusercontent.com/18071333/109424405-7ae42b00-7a09-11eb-94b1-a2d648d7d33e.png" width="400">
        <img src="https://user-images.githubusercontent.com/18071333/109424414-86cfed00-7a09-11eb-848c-0948dc8fceab.png" width="400">
    </p>
    <br>

* **View & ViewGroup**
   - ConstraintLayout combines a simple, expressive and flexible layout system with the powerful features built into the Android Studio Designer tool.
   - It makes it easier to create responsive user interface layouts that adapt automatically to different screen sizes and changing device orientations.
   - This has the benefit of avoiding many problems inherent in nesting layouts. It allows designing so-called flat or shallow layout hierarchies. This leads to less complex layouts and improved user interface rendering performance at runtime.

* **SSL Pinning**
   - When an client application such as mobile app or web browser begins secure session with the server there is the 3 things client and server must be agree on.
        - How will the key exchanged
        - How will be the data encrypted
        - How will messages marked as authentic

    - The server may decide AES256 encrypted data, SHA1 to sign messages. if client can support this messages the client request for the the certificate exchange from the server once client has validate the certificate chainning the public key is extracked from the server.

    - Developer can compile the public key into the application code this is essecially pins the key into the appliction. when client receives the public key from the server, it compare this key with the pinned key in apllciation. the key should should match. if the key dont match. the client terminates the session.

    - Types of SSL Pinning
        - Public key pinning
        - Certificate pinning
            - https://dzone.com/articles/encryption-and-signing
            - https://www.netguru.com/codestories/3-ways-how-to-implement-certificate-pinning-on-android
            - https://www.raywenderlich.com/10056112-securing-network-data-tutorial-for-android
        - SPKI pinning

* **Design Pattern**
   - https://www.journaldev.com/1827/java-design-patterns-example-tutorial#singleton-pattern
   - https://blog.mindorks.com/mastering-design-patterns-in-android-with-kotlin

* **Java Try with Resources**
   - http://tutorials.jenkov.com/java-exception-handling/try-with-resources.html

* **Java 8 Interface changes**
   - https://beginnersbook.com/2017/10/java-8-interface-changes-default-method-and-static-method/

* **Function Interface**
   - https://www.geeksforgeeks.org/functional-interfaces-java/

* **Types of Observable in Rx-Java**
   - https://blog.mindorks.com/understanding-types-of-observables-in-rxjava-6c3a2d0819c8

* **Rx-Java Scheduler what, when, how?**
   - https://medium.com/android-news/rxjava-schedulers-what-when-and-how-to-use-it-6cfc27293add

* **Executor Service**
   - https://www.javatpoint.com/java-executorservice

* **Kotlin interview Questions**
   - https://blog.mindorks.com/kotlin-android-interview-questions
   - https://www.ubuntupit.com/frequently-asked-kotlin-interview-questions-and-answers/

* **Kotlin Collection Functions**
   - https://blog.mindorks.com/kotlin-collection-functions

* **Map vs Flatmap**
   - https://www.linkedin.com/feed/update/urn:li:activity:6770786744422998017/
 
* **Stateflow vs LiveData**
   - https://scalereal.com/android/2020/05/22/stateflow-end-of-livedata.html

* **Livedata vs ObservableField**
   - https://blog.mindorks.com/livedata-vs-observable-in-android

* **ViewPager vs ViewPager2**
   - https://developer.android.com/training/animation/vp2-migration

* **Understanding Suspend function**
   - https://medium.com/mobile-app-development-publication/understanding-suspend-function-of-coroutines-de26b070c5ed

* **Coroutine runblocking**
   - https://www.geeksforgeeks.org/runblocking-in-kotlin-coroutines-with-example

* **Thread Safe mthods and blocks**
   - https://proandroiddev.com/synchronization-and-thread-safety-techniques-in-java-and-kotlin-f63506370e6d

* **App Data encryption**
   - https://blog.mindorks.com/how-to-encrypt-data-safely-on-device-and-use-the-androidkeystore

* **Data Structure and Algorithms**
   - https://www.tutorialspoint.com/data_structures_algorithms/shell_sort_algorithm.htm

* **Understanding scope storage in android**
   - https://blog.mindorks.com/understanding-the-scoped-storage-in-android

* **Solve out of memory error**
   - https://blog.mindorks.com/practical-guide-to-solve-out-of-memory-error-in-android-application

* **Battery optimizationn for Android**
   - https://blog.mindorks.com/battery-optimization-for-android-apps-f4ef6170ff70
   
* **Android Jetpack component**
   - https://blog.mindorks.com/what-is-android-jetpack-and-why-should-we-use-it

* **Android ViewModel under the hood**
   - https://blog.mindorks.com/android-viewmodels-under-the-hood

* **Workmanager**
   - https://blog.mindorks.com/integrating-work-manager-in-android

* **Arraymap vs Sparsh Array**
   - https://blog.mindorks.com/android-app-optimization-using-arraymap-and-sparsearray-f2b4e2e3dc47

* **Java Android Multithreading programming**
   - https://blog.mindorks.com/java-android-multithreaded-programming-runnable-callable-future-executor

* **Understanding Open keyword in Kotlin**
   - https://blog.mindorks.com/understanding-open-keyword-in-kotlin

<p align="center">
<img alt="AndroidInterviewQuestions" src="https://raw.githubusercontent.com/MindorksOpenSource/android-interview-questions/master/assets/android_interview_questions.png">
</p>

### Data Structures And Algorithms

> The level of questions asked on Data Structures And Algorithms totally depends on the company for which you are applying.

* Array
* LinkedList
    - A LinkedList, just like a tree and unlike an array, consists of a group of nodes which 
    together represent a sequence. Each node contains data and a pointer. The data in a node can be 
    anything, but the pointer is a reference to the next item in the LinkedList. A LinkedList 
    contains both a head and a tail. The Head is the first item in the LinkedList, and the Tail is 
    the last item. A LinkedList is not a circular data structure, so the tail does not have its 
    pointer pointing at the Head, the pointer is just null. The run time complexity for each of 
    the base methods are as follows:

        | Algorithm | Average | Worst Case |
        |:---------:|:-------:|:----------:|
        | Space     | O(n)    | O(n)       |
        | Search    | O(n)    | O(n)       |
        | Insert    | O(1)    | O(1)       |
        | Delete    | O(1)    | O(1)       |
* DoublyLinkedList
* Stack
    - A Stack is a basic data structure with a "Last-in-First-out" methodology. Which means that 
    the last item that was added to the stack, is the first item that comes out of the stack. A 
    Stack is like a stack of books. In order to get to the first book that was added in the stack 
    (the bottom book), all of the books that were added after need to be removed first. Adding to a 
    Stack is called a Push, removing from a stack is called a Pop, and getting the last item 
    inserted into the stack without removing it is called Top. [The most common way to implement a
     stack is by using a LinkedList, but there are also StackArray (implemented with an array) 
     which does not replace null entries, and there is also a Vector implementation that does 
     replace null entries.](https://en.wikibooks.org/wiki/Data_Structures/Stacks_and_Queues#Performance_Analysis)
     
        <table>
            <tr>
                <th>Algorithm</th>
                <th>Average</th>
                <th>Worst Case</th>
                <th>Image representation</th>
            </tr>
            <tr>
                <td>Space</td>
                <td>O(n)</td>
                <td>O(n)</td>
                <td rowspan="5">
                    <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/2/29/Data_stack.svg/250px-Data_stack.svg.png"/>
                </td>
            </tr>
            <tr>
                <td>Search</td>
                <td>O(n)</td>
                <td>O(n)</td>
            </tr>
            <tr>
                <td>Insert (Push)</td>
                <td>O(1)</td>
                <td>O(1)</td>
            </tr>
            <tr>
                <td>Delete (Pop)</td>
                <td>O(1)</td>
                <td>O(1)</td>
            </tr>
            <tr>
              <td>Top</td>
              <td>O(1)</td>
              <td>O(1)</td>
            </tr>
        </table>
* Queue
* PriorityQueue
* Dynamic Programming
* String Manipulation
* Binary Tree
* Binary Search Tree
* Sorting Algorithms
* Hash Table or Hash Map
* Breadth First Search
* Depth First Search
* Greedy Algorithm


### Core Java

* Explain OOP Concept.
    - Object-Oriented Programming is a methodology to design a program using classes, objects, 
    [inheritance](https://en.wikipedia.org/wiki/Inheritance_(object-oriented_programming)),
    [polymorphism](https://en.wikipedia.org/wiki/Polymorphism_(computer_science)),
    [abstraction](https://en.wikipedia.org/wiki/Abstraction_(software_engineering)), and
    [encapsulation](https://en.wikipedia.org/wiki/Encapsulation_(computer_programming)).
* Differences between abstract classes and interfaces? [link](https://arjun-sna.github.io/java/2017/02/02/abstractvsinterface/)
    - An abstract class, is a class that contains both concrete and abstract methods 
    (methods without implementations). An abstract method must be implemented by the abstract class
     sub-classes. Abstract classes are extended.
    - An interface is like a blueprint/contract of a class. It contains empty methods that 
    represent what all of its subclasses should have in common. The subclasses provide the 
    implementation for each of these methods. Interfaces are implemented.
* What is serialization? How do you implement it?
    - Serialization is the process of converting an object into a stream of bytes in order to store 
    an object into memory so that it can be recreated at a later time while still keeping the 
    objects original state and data. In Java there are two methods of doing this, one is by 
    implementing Serializable or Parcelable. In Android, however, Serializable should never be used 
    in Android. Parcelable was created to be more efficient then Serializable, and performs about 
    10x faster then Serializable because Serializable uses reflection which is a slow process and 
    tends to create a lot of temporary objects which may cause garbage collection to occur more often.
* What is Singleton class?
    - A singleton is a class that can only be instantiated once.[This singleton pattern restricts 
    the instantiation of a class to one object. This is useful when exactly one object is needed 
    to coordinate actions across the system. The concept is sometimes generalized to systems 
    that operate more efficiently when only one object exists, or that restrict the instantiation 
    to a certain number of objects.](https://en.wikipedia.org/wiki/Singleton_pattern)
* What are anonymous classes?
* What is the difference between using `==` and `.equals` on a string?
* What is the `hashCode()` and `equals()` used for?
* What are these `final`, `finally` and `finalize`?
* What is memory leak and how does Java handle it?
* What is garbage collector? How it works?
  -All objects are allocated on the heap area managed by the JVM. 
  As long as an object is being referenced, the JVM considers it  alive. 
  Once an object is no longer referenced and therefore is not reachable by the application code,
  the garbage collector removes it and reclaims the unused memory.
* `Arrays` vs `ArrayLists`.
* `HashSet` vs `TreeSet`.
* Typecast in Java.
* Difference between method overloading and overriding.
<p align="center">
<img alt="Overloading and Overriding" src="https://github.com/codeshef/android-interview-questions/blob/master/assets/overloading-vs-overriding.png">
</p>

Overloading happens at compile-time while Overriding happens at runtime: The binding of overloaded method call to its definition has happens at compile-time however binding of overridden method call to its definition happens at runtime.

Static methods can be overloaded which means a class can have more than one static method of same name. Static methods cannot be overridden, even if you declare a same static method in child class it has nothing to do with the same method of parent class.

The most basic difference is that overloading is being done in the same class while for overriding base and child classes are required. Overriding is all about giving a specific implementation to the inherited method of parent class.

Static binding is being used for overloaded methods and dynamic binding is being used for overridden/overriding methods.
Performance: Overloading gives better performance compared to overriding. The reason is that the binding of overridden methods is being done at runtime.

Private and final methods can be overloaded but they cannot be overridden. It means a class can have more than one private/final methods of same name but a child class cannot override the private/final methods of their base class.

Return type of method does not matter in case of method overloading, it can be same or different. However in case of method overriding the overriding method can have more specific return type (refer this).

Argument list should be different while doing method overloading. Argument list should be same in method Overriding.

* What are the access modifiers you know? What does each one do?
* Can an Interface extend another Interface?
* What does the `static` word mean in Java?
* Can a `static` method be overridden in Java?
* What is Polymorphism? What about Inheritance?
* What is the difference between an Integer and int?
* Do objects get passed by reference or value in Java? Elaborate on that.
* What is a ThreadPoolExecutor? [Link](https://blog.mindorks.com/threadpoolexecutor-in-android-8e9d22330ee3)
* What the difference between local, instance and class variables?
* What is reflection? [Link](http://tutorials.jenkov.com/java-reflection/index.html)
* What are strong, soft and weak references in Java?
* What is dependency injection? Can you name few libraries? Have you used any?
* What does the keyword `synchronized` mean?
* What does it means to say that a `String` is immutable?
* What are `transient` and `volatile` modifiers?
* What is the `finalize()` method?
* How does the `try{}finally{}` works?
* What is the difference between instantiation and initialization of an object?
* When is a `static` block run?
* Explain Generics in Java?
* Difference between `StringBuffer` and `StringBuilder`?
* How is a `StringBuilder` implemented to avoid the immutable string allocation problem?
* What is Autoboxing and Unboxing?
* What’s the difference between an Enumeration and an Iterator?
* What is the difference between fail-fast and fail safe in Java?
* What is Java priority queue?
* What are the design patterns? [Link](https://github.com/iluwatar/java-design-patterns)


### Core Android

* Explain activity lifecycle.
* Tell all the Android application components.
* Service vs IntentService. [Link](https://stackoverflow.com/a/15772151/5153275)
* What is the structure of an Android Application?
* How to persist data in an Android app?
* How would you perform a long-running operation in an application?
* How would you communicate between two Fragments?
* Explain Android notification system?
* How can two distinct Android apps interact?
* What is Fragment?
* Why is it recommended to use only the default constructor to create a fragment? [Link](https://stackoverflow.com/a/16042750/2809326)
* Why Bundle class is used for data passing and why cannot we use simple Map data structure
* Explain the lifecycle of a Fragment. [Link](https://www.techsfo.com/blog/wp-content/uploads/2014/08/complete_android_fragment_lifecycle.png)
* What is Dialog in Android?
* What is View in Android?
* Can you create custom views? How?
* What are ViewGroups and how they are different from the views?
* What is the difference between a fragment and an activity? Explain the relationship between the two.
* What is the difference between Serializable and Parcelable? Which is the best approach in Android?
* What are "launch modes"? [Link](https://blog.mindorks.com/android-activity-launchmode-explained-cbc6cf996802)
* What are Intents? [Link](https://stackoverflow.com/questions/6578051/what-is-an-intent-in-android)
* What is an Implicit Intent?
* What is an Explicit Intent?
* What is an AsyncTask?
* What is a BroadcastReceiver? [Link](https://stackoverflow.com/questions/5296987/what-is-broadcastreceiver-and-when-we-use-it)
* What is a LocalBroadcastManager? [Link](https://developer.android.com/reference/android/support/v4/content/LocalBroadcastManager.html)
* What is a JobScheduler? [Link](http://www.vogella.com/tutorials/AndroidTaskScheduling/article.html)
* What is DDMS and what can you do with it?
* What is the support library? Why was it introduced?[Link](http://martiancraft.com/blog/2015/06/android-support-library/)
* What is a ContentProvider and what is it typically used for?
* What is Android Data Binding? [Link](https://developer.android.com/topic/libraries/data-binding/index.html)
* What are Android Architecture Components? [Link](https://developer.android.com/topic/libraries/architecture/index.html)
* What is ADB?
* What is ANR? How can the ANR be prevented?
* What is `AndroidManifest.xml`?
* Describe how broadcasts and intents work to be able to pass messages around your app?
* How do you handle `Bitmaps` in Android as it takes too much memory?
* What are different ways to store data in your Android app?
* What is the Dalvik Virtual Machine?
* What is the relationship between the life cycle of an AsyncTask and an Activity? What problems can this result in? How can these problems be avoided?
* What is the function of an intent filter?
* What is a Sticky Intent? [Link](http://www.androidinterview.com/what-is-a-sticky-intent/)
* What is AIDL? Enumerate the steps in creating a bounded service through AIDL.
* What are the different protection levels in permission?
* How would you preserve Activity state during a screen rotation? [Link](https://stackoverflow.com/questions/3915952/how-to-save-state-during-orientation-change-in-android-if-the-state-is-made-of-m)
* Relative Layout vs Linear Layout.
* How to implement XML namespaces?
* Difference between `View.GONE` and `View.INVISIBLE`?
* What is the difference between a regular bitmap and a nine-patch image?
* Tell about the bitmap pool. [Link](https://blog.mindorks.com/how-to-use-bitmap-pool-in-android-56c71a55533c)
* How to avoid memory leaks in Android?
* What are widgets on Home-Screen in Android?
* What is AAPT?
* How do you find memory leaks in Android applications?
* How do you troubleshoot a crashing application?
* Why should you avoid to run non-ui code on the main thread?
* How did you support different types of resolutions?
* What is Doze? What about App Standby?
* What can you use for background processing in Android?
* What is ORM? How does it work?
* What is a Loader?
* What is the NDK and why is it useful?
* What is the StrictMode? [Link](https://blog.mindorks.com/use-strictmode-to-find-things-you-did-by-accident-in-android-development-4cf0e7c8d997)
* What is Lint? What is it used for?
* What is a `SurfaceView`?
* What is the difference between `ListView` and `RecyclerView`?
* What is the ViewHolder pattern? Why should we use it?
* What is a PendingIntent?
* Can you manually call the Garbage collector?
* What is the best way to update the screen periodically?
* What are the different types of Broadcasts?
* Have you developed widgets? Describe. [Link](https://blog.mindorks.com/android-widgets-ad3d166458d3)
* What is Context? How is it used? [Link](https://medium.com/p/understanding-context-in-android-application-330913e32514)
* Do you know what is the view tree? How can you optimize its depth?
* What is the `onTrimMemory` method?
* Is it possible to run an Android app in multiple processes? How?
* How does the OutOfMemory happens?
* What is a `spannable`?
* What is renderscript? [Link](https://blog.mindorks.com/comparing-android-ndk-and-renderscript-1a718c01f6fe)
* What are the differences between Dalvik and ART?
* FlatBuffers vs JSON. [Link](https://blog.mindorks.com/why-consider-flatbuffer-over-json-2e4aa8d4ed07)
* What are Annotations? [Link](https://blog.mindorks.com/creating-custom-annotations-in-android-a855c5b43ed9), [Link](https://blog.mindorks.com/improve-your-android-coding-through-annotations-26b3273c137a)
* Tell about Constraint Layout [Link](https://blog.mindorks.com/using-constraint-layout-in-android-531e68019cd)
* `HashMap`, `ArrayMap` and `SparseArray` [Link](https://blog.mindorks.com/android-app-optimization-using-arraymap-and-sparsearray-f2b4e2e3dc47)
* Explain Looper, Handler and HandlerThread. [Link](https://blog.mindorks.com/android-core-looper-handler-and-handlerthread-bd54d69fe91a)
* How to reduce battery usage in an android application? [Link](https://blog.mindorks.com/battery-optimization-for-android-apps-f4ef6170ff70)
* What is `SnapHelper`? [Link](https://blog.mindorks.com/using-snaphelper-in-recyclerview-fc616b6833e8)
* How to handle multi-touch in android [link](https://arjun-sna.github.io/android/2016/07/20/multi-touch-android/)


### Architecture

* Describe the architecture of your last app.
* Describe MVP. [Link](https://blog.mindorks.com/essential-guide-for-designing-your-android-app-architecture-mvp-part-1-74efaf1cda40)
* What is presenter?
* What is model?
* Describe MVC.
* What is controller?
* Describe MVVM. [Link](https://github.com/MindorksOpenSource/android-mvvm-architecture)
* Tell something about clean code [Link](https://blog.mindorks.com/every-programmer-should-read-this-book-6755dedec78d)


### Design Problem

* Design Uber App.
* Design Facebook App.
* Design Facebook Near-By Friends App.
* Design WhatsApp.
* Design SnapChat.
* Design problems based on location based app.


### Tools And Technologies

* Git. [Link](https://github.com/git-tips/tips)
* RxJava. [Link](https://blog.mindorks.com/a-complete-guide-to-learn-rxjava-b55c0cea3631)
* Dagger 2. [Link](https://medium.com/p/a-complete-guide-to-learn-dagger-2-b4c7a570d99c)
* Android Development Useful Tools. [Link](https://blog.mindorks.com/android-development-useful-tools-fd73283e82e3)
* Firebase. [Link](https://firebase.google.com/)


### Android Test Driven Development

* What is Espresso? [Link](https://developer.android.com/training/testing/ui-testing/espresso-testing.html)
* What is Robolectric? [Link](http://robolectric.org/)
* What is UI-Automator? [Link](https://developer.android.com/training/testing/ui-testing/uiautomator-testing.html)
* Explain unit test.
* Explain instrumented test.
* Have you done unit testing or automatic testing?
* Why Mockito is used? [Link](http://site.mockito.org/)
* Describe JUnit test.


### Others

* Describe how REST APIs work.
* Describe SQLite.
* Describe database.
* Project Management tool - trello, basecamp, kanban, jira, asana.
* About build System - gradle, ant, buck. 
* Reverse Engineering an APK.
* What is proguard used for?
* What is obfuscation? What is it used for? What about minification?
* How do you build your apps for release?
* How do you control the application version update to specific number of users?
* Can we identify users who have uninstalled our application?
* APK Size Reduction. [Link](https://blog.mindorks.com/how-to-reduce-apk-size-in-android-2f3713d2d662)
* Android Development Best Practices. [Link](https://blog.mindorks.com/android-development-best-practices-83c94b027fd3)
* Android Code Style And Guidelines. [Link](https://blog.mindorks.com/android-code-style-and-guidelines-d5f80453d5c7)
* Have you tried Kotlin? [Link](https://medium.com/p/why-you-must-try-kotlin-for-android-development-e14d00c8084b)
* What are the metrics that you should measure continuously while android application development? [Link](https://blog.mindorks.com/android-app-performance-metrics-a1176334186e)

### 1. Object-Oriented

- **What is an Object?**

  An object is an instance of a class that has states and behaviors. A Class
  can be defined as a template that describes the behavior/state that the object
  of its type support.

<br>

- **What is the main feature of OOP ?**

    `Encapsulation`, `Polymorphism`, `Inheritance`, `Abstraction`

<br>

- **What is encapsulation?**

  Encapsulation is one of the four fundamental OOP concepts. It is a mechanism of wrapping the data (variables) and code acting on the data (methods) together as a single unit. In encapsulation, the variables of a class will be hidden from other classes, and can be accessed only through the methods of their current class. Therefore, it is also known as *data hiding*. To achieve encapsulation in Java:
    - Declare the variables of a class as private.
    - Provide public setter and getter methods to modify and view the variables values.

  Benefits of Encapsulation:
    - The fields of a class can be made read-only or write-only.
    - A class can have total control over what is stored in its fields.

<br>


- **Difference between abstract and interface?**

  | Interface     | Abstract class     |
  | :------------- | :------------- |
  | Support multiple inheritances | Does not support multiple inheritances |
  | Can extends another interfaces only | Can extends another class and implement multiple interfaces |
  | Does not contain data member | Contains data member |
  | Does not contains constructors | contains constructors  |
  | In Java Contains only incomplete member (signature of member) | Contains both signature (abstract) of method and member functions |
  | Cannot have access modifiers by default and everything is assumed as public | Can has access modifiers for subs, methods and fields |


- **What is Polymorphism?**

  The word polymorphism means having many forms. In simple words, we can define polymorphism as the ability of a message to be displayed in more than one form. In Java polymorphism is mainly divided into two types: compile-time and runtime polymorphism.

- **What is the difference between static and dynamic Polymorphism?**

  *method overloading* represents a *static* form of polymorphism. method overloading means using two or more functions with same name but with the different parameters. Static polymorphism is resolved on compile-time and that is why it's called static. An example of this would be as follow:

  ```java
    class StaticPolymorphismTest {

      public int multiply(int a, int b) {
        return a * b;
      }

      public double multiply(double a, double b) {
        return a * b;
      }

    }
  ```

  *method overriding* represents a *dynamic* form of polymorphism. It is a process in which a function call to the overridden method is resolved at Runtime. It is also known as *Dynamic Method Dispatch*. dynamic polymorphism is resolved at runtime. An example of this would be as follow:

  ```java
  class Parent {

    void Print()
    {
        System.out.println("parent class");
    }
  }

  class subclass1 extends Parent {

    void Print()
    {
        System.out.println("subclass1");
    }
  }

  class subclass2 extends Parent {

    void Print()
    {
        System.out.println("subclass2");
    }
  }

  class TestPolymorphism3 {

    public static void main(String[] args){

        Parent a;

        a = new subclass1();
        a.Print();

        a = new subclass2();
        a.Print();
    }
  }
  ```

  Output:
  ```
  subclass1
  subclass2
  ```

- **Can Interfaces to be extended?**

  Yes, an interface can extend other interfaces. it supports multiple
  inheritances, which means it can extend more than one interface. But every
  class which wants to use an interface must add it by keyword `implements`
  and using the keyword `extends` for interfaces in classes is illegal and
  cause compile error.

- **What is the difference between overriding and overloading?**

  | Method Overloading      | Method Overriding     |
  | :-------------   | :------------- |
  | Method overloading is a compile time polymorphism.         | Method overriding is a run time polymorphism.       |
  | It help to rise the readability of the program. | While it is used to grant the specific implementation of the method which is already provided by its parent class or super class. |
  | It is occur within the class.	 | 	While it is performed in two classes with inheritance relationship. |
  | Method overloading may or may not require inheritance. | While method overriding always needs inheritance. |
  | In this, methods must have same name and different signature. | While in this, methods must have same name and same signature. |
  | In method overloading, return type can or can not be be same, but we must have to change the parameter. | While in this, return type must be same or co-variant. |

<br>



<br>

### 2. JAVA

- **How to prevent a class to be extended?**

  simply use keyword `final` in definition of class or methods. for example:
  ```java
  final public class CantOverrideClass {

    public final void cantOverrideMethod(){

    }

  }
  ```  

- **What is the use of the finalize method?**

  `finalize()` method is a protected and non-static method of java.lang.Object
  class. This method will be available in all objects you create in java. This
  method is used to perform some final operations or clean up operations on an
  object before it is removed from the memory. you can override the `finalize()`
  method to keep those operations you want to perform before an object is
  destroyed. Here is the general form of `finalize()` method.

  ```java
  protected void finalize() throws Throwable {
    //Keep some resource closing operations here
  }
  ```

- **What is a static variables in Java?**

  static is a non-access modifier in Java which is applicable for the following:
    - blocks
    - variables
    - methods
    - nested classes

  When a variable is declared as static, then a single copy of variable is created and shared among all objects at class level. Static variables are, essentially, global variables. All instances of the class share the same static variable.

  Important points for static variables:
    - We can create static variables at class-level only. See [here](https://www.geeksforgeeks.org/g-fact-47/)
    - static block and static variables are executed in order they are present in a program.

- **Overriding for static method, possible?**

  quick response: no!

  Inheritance comes from object-oriented principles, all of OOP principles needs
  objects to apply on. when we talk about inheritance, it means we deal with some
  objects which have relationships with each other. Besides, "overriding" is a
  feature of OOP principle which is related to run-time polymorphism. The
  implementation to be executed is decided at run-time and the decision is made
  according to the object used for the call.

  On the other hand, static methods belong to the class not object. So we use
  static methods without the need for creating an instance of a class. Besides,
  static methods are resolved in compile-time. Hence the answer is 'NO'.


- **What is an abstract class? Benefits?**

  According to the official document, An abstract class is a class that is declared `abstract`. It may or may not include abstract methods. Abstract classes cannot be instantiated, but they can be subclassed. Also, An abstract method is a method that is declared without an implementation (without braces, and followed by a semicolon), If a class includes abstract methods, then the class itself must be declared `abstract`.
  ```java
  public abstract class GraphicObject {
    // declare fields
    // declare nonabstract methods
    abstract void draw();
  }
  ```
  We use abstraction when we want to enforce base functions a have base
  properties. Although we could use an interface for this, sometimes the
  functionality of such classes may overlap or it needs some objects which
  are shared in whole class scope, then we use abstraction.

- **What is an object cloning? can you use clone() method of every object ?**

  Object cloning refers to creation of exact copy of an object. It creates a new instance of the class of current object and initializes all its fields with exactly the contents of the corresponding fields of this object. Every class that implements `clone()` methods should call super.clone() to obtain the cloned object reference. Also it must implement java.lang.Cloneable interface otherwise it will throw CloneNotSupportedException when clone method is called on that class’s object.
  ```java
  protected Object clone() throws CloneNotSupportedException
  ```

- **What is the difference between Shallow copy and deep copy?**

  - **Shallow copy**: is method of copying an object and is followed by default in cloning. In this method the fields of an old object X are copied to the new object Y. While copying the object type field the reference is copied to Y i.e object Y will point to same location as pointed out by X. If the field value is a primitive type it copies the value of the primitive type.
  Therefore, any changes made in referenced objects in object X or Y will be reflected in other object.
  ```java
  class Test  {
      int x, y;
  }   
  // Contains a reference of Test and implements
  // clone with shallow copy.
  class Test2 implements Cloneable {
      int a;
      int b;
      Test c = new Test();

      public Object clone() throws CloneNotSupportedException {
        return super.clone();
      }
  }  
  public class Main {

      public static void main(String args[]) throws CloneNotSupportedException {
        Test2 t1 = new Test2();
        t1.a = 10;
        t1.b = 20;
        t1.c.x = 30;
        t1.c.y = 40;

        Test2 t2 = (Test2)t1.clone();

        // Creating a copy of object t1 and passing
        //  it to t2
        t2.a = 100;

        // Change in primitive type of t2 will not
        // be reflected in t1 field
        t2.c.x = 300;

        // Change in object type field will be
        // reflected in both t2 and t1(shallow copy)
        System.out.println(t1.a + " " + t1.b + " " +
                          t1.c.x + " " + t1.c.y);
        System.out.println(t2.a + " " + t2.b + " " +
                          t2.c.x + " " + t2.c.y);
      }
  }
  ```
  Output:
  ```
  10 20 300 40
  100 20 300 40
  ```

  - **Deep Copy**: If we want to create a deep copy of object X and place it in a new object Y then new copy of any referenced objects fields are created and these references are placed in object Y. This means any changes made in referenced object fields in object X or Y will be reflected only in that object and not in the other.

    A deep copy copies all fields, and makes copies of dynamically allocated memory pointed to by the fields. A deep copy occurs when an object is copied along with the objects to which it refers.

    ```java
    class Test {
      int x, y;
    }   
    // Contains a reference of Test and implements
    // clone with deep copy.
    class Test2 implements Cloneable {
      int a, b;

      Test c = new Test();

      public Object clone() throws CloneNotSupportedException {
        // Assign the shallow copy to new reference variable t
        Test2 t = (Test2)super.clone();

        t.c = new Test();

        // Create a new object for the field c
        // and assign it to shallow copy obtained,
        // to make it a deep copy
        return t;
      }
    }

    public class Main {

      public static void main(String args[]) throws CloneNotSupportedException {
        Test2 t1 = new Test2();
        t1.a = 10;
        t1.b = 20;
        t1.c.x = 30;
        t1.c.y = 40;

        Test2 t3 = (Test2)t1.clone();
        t3.a = 100;

        // Change in primitive type of t2 will not
        // be reflected in t1 field
        t3.c.x = 300;

        // Change in object type field of t2 will not
        // be reflected in t1(deep copy)
        System.out.println(t1.a + " " + t1.b + " " +
                          t1.c.x + " " + t1.c.y);
        System.out.println(t3.a + " " + t3.b + " " +
                          t3.c.x + " " + t3.c.y);
      }
    }

    ```
    Output:
    ```
    10 20 30 40
    100 20 300 0
    ```

- **Multiple inheritances? Possible? How can we do that?**

  Multiple inheritance in Java programming is achieved or implemented using interfaces. Java does not support multiple inheritance using classes. In simple term, a class can inherit only one class and multiple interfaces in a java programs.

- **Object scopes?**

  `public` , `protected` , default (no modifier) , `private`

  | Modifier     | Package     | Subclass     | World     |
  | :------------- | :------------- | :------------- | :------------- |
  | Public       | Yes       | Yes       | Yes       |
  | protected       | Yes      | Yes       | No       |
  | Default (no modifier)       | Yes       | No       | No       |
  | private       | No       | No       | No       |


- **Override private methods, possible?**

  No, a private method cannot be overridden since it is not visible from any other class.

- **why access to the non-static variable is not allowed from static method in Java?**

  because non-static variable are associated with a specific instance of an object while static is not associated with any instance.

- **Java reference types?** [*geeksforgeeks*]("https://www.geeksforgeeks.org/types-references-java/")

- **What is Generic in Java?**

  Generics enable types (classes and interfaces) to be parameters when defining classes, interfaces and methods. Type parameters provide a way for you to re-use the same code with different inputs. The difference is that the inputs to formal parameters are values, while the inputs to type parameters are types. [more details](https://www.geeksforgeeks.org/generics-in-java/)

- **What is the difference between int and Integer?**

  `int` is a primitive type, while `Integer` is class with a single field of type `int`. Variables of type `int` store the avtual binary value for the integer. Variables of type `Integer` store references to `Integer` objects, just as with any other reference (object) type. The `Integer` class is used where you need an `int` to be treated like any other object, such as in generic types or situations where you need nullability.

- **What are Autoboxing and unboxing?**

  - **Autoboxing:** Converting a primitive value into an object of the corresponding wrapper class is called autoboxing. For example, converting `int` to `Integer` class.
  - **Unboxing:**  Converting an object of a wrapper type to its corresponding primitive value is called unboxing. For example conversion of `Integer` to `int`.

- **What is the difference between initialization and instantiation?**

  - **Instantiation** is when memory is allocated for an object. This is what the `new` keyword is doing. A reference to the object that was created is returned from the `new` keyword.

  - **Initialization** is when values are put into the memory that was allocated. This is what the Constructor of a class does when using the `new` keyword. A variable must also be initialized by having the reference to some object in memory passed to it.


- **How does a static block work?**

  Run once when class is loaded, used for initializing static members. [read more](https://www.geeksforgeeks.org/g-fact-79/)

- **What does the keyword `synchronized` mean?**

  A `synchronized` block in Java is synchronized on some object. All synchronized blocks synchronized on the same object can only have one thread executing inside them at a time. All other threads attempting to enter the synchronized block are blocked until the thread inside the synchronized block exits the block.

- **What is the memory leak? How to handle it?**
- **What is `transient` modifier? What does it come for?** [complete explanation](https://www.geeksforgeeks.org/transient-keyword-java/)

- **What is the difference between `==` and `.equal`?**
  - The `equals()` method compares two strings, character by character, to determine equality.
  - The `==` operator checks to see whether two object references refer to the same instance of an object

- **What is `reflection`?** [geeksforgeeks](https://www.geeksforgeeks.org/reflection-in-java/)
- **What is the `volatile` modifier?**

  In multi-threading apps where the threads operate on non-volatile variables, each thread may copy variables from main memory into a CPU cache, for performance reason. If your app run on more than one thread, each thread may copy the variable and cache it. So This keyword is used to mark a variable as "being stored in main memory". Note that reading from and writing to main memory is more expensive than accessing the CPU cache. Thus, you should only use volatile variables when you really need to enforce visibility of variables.

  ![](/assets/images/volatile-preview.png)

- **What is the `hashCode()` used for?**

  `hashcode()` returns the hashcode value as an Integer. Hashcode value is mostly used in hashing based collections like HashMap, HashSet, HashTable….etc. According to the official documentation, The general contract of `hashCode()` is:
    - Whenever it is invoked on the same object more than once during an execution of a Java application, the hashCode method must consistently return the same integer, provided no information used in equals comparisons on the object is modified. This integer need not remain consistent from one execution of an application to another execution of the same application.
    - If two objects are equal according to the equals(Object) method, then calling the hashCode method on each of the two objects must produce the same integer result.

    - It is not required that if two objects are unequal according to the equals(java.lang.Object) method, then calling the hashCode method on each of the two objects must produce distinct integer results. However, the programmer should be aware that producing distinct integer results for unequal objects may improve the performance of hashtables.


- **What are "annotations"?**

  Java annotations are used to provide meta data for your Java code. Being meta data, Java annotations do not directly affect the execution of your code, although some types of annotations can actually be used for that purpose. [read more](http://tutorials.jenkov.com/java/annotations.html)

- **What is thread-safe mean? How we can make our code thread-safe?**

  Thread safety in java is the process to make our program safe to use in multithreaded environment, there are different ways through which we can make our program thread safe.
    - Synchronization
    - Use of Atomic Wrapper, For example AtomicInteger.
    - Use of locks from java.util.concurrent.locks package.
    - Using thread safe collection classes
    - Using volatile keyword.

  Note that if two threads are both reading and writing to a shared variable, then using the volatile keyword for that is not enough. You need to use a synchronized in that case to guarantee that the reading and writing of the variable is atomic. Reading or writing a volatile variable does not block threads reading or writing. For this to happen you must use the synchronized keyword around critical sections.

- **what is the difference between `throw` and `throws`?**

  Keyword `throw` is used to explicitly throw as an exception in the body of function, while `throws` is utilized to handle checked exceptions for re-intimating the compiler that exceptions are being handled. The throws need to be used in the function’s signature and also while invoking the method that raises checked exceptions.

<br>

### 3. Kotlin

- **What are the benefits of Kotlin?**

- **What does "Null safety" meaning?**
- **Why Kotlin does not support primitive type?**
- **What is Lazy initialization?**
- **What is the data class?**
- **Is it possible to inherit a class/method/property by default?**
- **Difference between apply, also?**
- **What `==` exactly do in Kotlin in comparison to Java?**
- **What is the difference between parameter and argument?**
- **What is the difference between function and method?**
- **What is the "receiver" in the extension function?**
- **What is operator overloading?**
- **Is it possible to write a static method as java as has?**
- **What is a sealed class?**
- **How does an extension function work?**
- **What is `reified` keyword?**
- **What is an inline function?**
- **What are the cons of using an inline function?**
- **What is the best practice of using an inline function?**
- **How does the `companion object` block work?**
- **Is it possible to create an extension function on the `companion object` of a class?**
- **Extension function as a member, possible? What are the benefits of declaring an extension function as a member?**
- **What is a spread operator? What is the recommended place to use it?**
- **What is the producer’s function? how to demonstrate it in Kotlin?**
- **What is the consumer’s function? how to demonstrate it in Kotlin?**
- **What is the higher-order function?**
- **How to compare two Strings in Kotlin?**
- **What is the difference between `==` and `===` ?**

<br>

### 4. Android

- **What is `Application` class?**

  The `Application` class in Android is the base class within an Android app that contains all other components such as activities and services. The Application class, or any subclass of the Application class, is instantiated before any other class when the process for your application/package is created.

- **Difference between `Activity` and `Service`?**

  - **Activity:** An activity is the entry point for interacting with the user. It represents a single screen with a user interface.

  - **Service:** A service is a general-purpose entry point for keeping an app running in the background for all kinds of reasons. It is a component that runs in the background to perform long-running operations or to perform work for remote processes. A service does not provide a user interface.

- **Why do android apps need to ask permission like `INTERNET` or `LOCATION`?**

  The Android platform takes advantage of the Linux user-based protection to identify and isolate app resources called sandbox. This isolates apps from each other and protects apps and the system from malicious apps. If an app needs to use some system resources (like internet, or location sensor,..) or needs to connect other apps (like IAB library), it should request this access. Then android OS give this request and get permission to access the resource. If you want to use system resources, request the permission under the `<uses-permission>` tag in the `android-manifest.xml` file.

- **Differences between `serializable` and `Parcelable`?**

  Serializable is a standard java interface but not a part of the Android SDK. Just by implementating this interface your POJO will be ready to jump from one activity to another. So what's the problem with Serializable? Serializable use reflection during the process and lots of additional temp objects created along the way and it may cause garbage collection to occue more often. That is why the serializable is more than 10x slower than Parcelable.

- **Why `serializable` body is empty? How is it doing?**

  Yes, It's empty because the Java reflection API is performed for marshaling operations (by JVM). This helps identify the Java object's member and behavior but also ends up creating a lot of garbage objects.

- **Which method in `fragment` runs only once?**

  According to the [documentation](https://developer.android.com/guide/components/fragments#Creating), the `onCreate()` method is called once a fragment is created. Within your implementation, you should initialize essential components of the fragment that you want to retain when the fragment is paused or stopped, then resumed.

- **How does the activity respond when orientation is changed?**

  According to the [documentation](https://developer.android.com/guide/topics/resources/runtime-changes), Some device configurations can change during runtime (such as screen orientation, keyboard availability, and when the user enables multi-window mode). When such a change occurs, Android restarts the running `Activity` ( `onDestroy()` is called, followed by `onCreate()`). The restart behavior is designed to help your application adapt to new configurations by automatically reloading your application with alternative resources that match the new device configuration.

- **How to know `configChange` happens in `onDestroy()` function?**

  Once an activity is in the process of finishing then `isFinishing()` method is returned `true` value, otherwise `false` when the system is temporarily destroying the instance of the activity.

- **How to prevent the data from reloading when orientation is changed?**

  The most basic approach would be to use a combination of `ViewModels` and `onSaveInstanceState()`. A `ViewModel` is LifeCycle-Aware. In other words,
  a `ViewModel` will not be destroyed if its owner is destroyed for a
  configuration change (e.g. rotation). The new instance of the owner will
  just re-connected to the existing `ViewModel`. So if you rotate an `Activity`
  three times, you have just created three different `Activity` instances, but
  you only have one `ViewModel`. So the common practice is to store data in the
  `ViewModel` class (since it persists data during configuration changes) and
  use `OnSaveInstanceState()` to store small amounts of UI data.

- **How to handle multiple screen sizes?**

  It's a long debate but in a very nutshell, you can do it in these ways:
    - Use flexible layout like `ConstraintLayout` unless create alternative layout in different layout folders. (e.g. layout-sw480, layout-sw600, layout-sw720 ...)    
    - Provide different bitmap drawables for different screen densities or use vector assets.
    - Be aware of the screen orientation change approach in your application.
      If you don't want to handle it enforce to use just one orientation (portrait or landscape) through declaring it in the manifest file.

 for complete reading, see the [official documentation](https://developer.android.com/training/multiscreen/screensizes).

- **What is the difference between margin and padding?**

   - **Padding** will be space added inside the container, for instance,
    if it is a button, padding will be added inside the button.       

  - **Margin** will be space added outside the container.

- **What is `sw` keyword in `layout-sw600` folder meaning?**

  The `sw` keywrod which stands on "smallest width" is an screen size qualifier that allow you to provide alternative layouts for screens that have a minimum width measured in dp.
  The smallest width qualifier specifies the smallest of the screen's two sides, regardless of the device's current orientation, so it's a simple way to specify the overall screen size available for your layout. Here is some useful values:

    - **320dp:** a typical phone screen (240x320 ldpi, 320x480 mdpi, 480x800 hdpi, etc).
    - **480dp:** a large phone screen ~5" (480x800 mdpi).
    - **600dp:** a 7” tablet (600x1024 mdpi).
    - **720dp:** a 10” tablet (720x1280 mdpi, 800x1280 mdpi, etc).

  Figure below provides a more detailed view of how different screen dp widths generally correspond to different screen sizes and orientations.

  ![](/assets/images/layout-adaptive-breakpoints_2x.png)

- **What is the difference between `sw` and `w` and `h` as postfix in order to define the resources folder?**

    - `sw`: The smallest width qualifier specifies the smallest of the screen's two sides, regardless of the device's current orientation,
    - `w`: The width qualifier specifies the available width. For example, if you have a two-pane layout, you might want to use that whenever the screen provides at least 600dp of width, which might change depending on whether the device is in landscape or portrait orientation. Notice that this qualifier is orientation related.
    - `h`: The height qualifier specifies the available height. This is equivalent to `w` qualifier but is used when the available height is a concern.

  The major difference between these qualifiers is responding to orientation change. The `sw` isn't orientation sensitive but the two others are orientation sensitive. It means that if the screen is 480*800 in dp, then in `sw` always `layout-sw480` folder is loaded but in `w`, for portrait mode, `layout-w480`, and landscape mode, `layout-w800` folder is loaded.

- **What are the major differences between `ListView` and `RecyclerView`?**

  - **ViewHolder Pattern**: `Recyclerview` implements the ViewHolders pattern
    whereas it is not mandatory in a ListView. A `ViewHolder` object stores
    each of the component views inside the tag field of the Layout, so you can
    immediately access them without the need to look them up repeatedly.
    In `ListView`, the code might call `findViewById()` frequently during the
    scrolling of `ListView`, which can slow down performance. Even when the
    `Adapter` returns an inflated view for recycling, you still need to look up
    the elements and update them. A way around repeated use of `findViewById()`
     is to use the "view holder" design pattern.

  - **LayoutManager**: In a `ListView`, the only type of view available is
    the `vertical` ListView. A `RecyclerView` decouples list from its container
    so we can put list items easily at run time in the different containers
    (linearLayout, gridLayout) by setting LayoutManager.

  - **Item Animator**: `ListViews` are lacking in support of good animations,
    but the `RecyclerView` brings a whole new dimension to it.

- **Difference between `Intent` and `IntentService`?**
  - `Service` is the base class for Android services that can be extended to
    create any service. A class that directly extends `Service` runs on the main
    thread so it will block the UI (if there is one) and should therefore either
    be used only for short tasks or should make use of other threads for longer
    tasks.

  - `IntentService` is a subclass of `Service` that handles asynchronous requests
   (expressed as `Intents`) on demand. Clients send requests through
   `startService(Intent)` calls. The service is started as needed, handles each
   `Intent` in turn using a worker thread, and stops itself when it runs out of
   work. [Read More on Mindorks's blog]("https://blog.mindorks.com/service-vs-intentservice-in-android")

- **What is `Fragment`?**

  A `Fragment` is a piece of an activity which enable more modular activity design. A fragment has its layout, its behavior, and its life cycle callbacks. You can add or remove fragments in an activity while the activity is running. You can combine multiple fragments in a single activity to build a multi-pane UI. A fragment can also be used in multiple activities. The fragment life cycle is closely related to its host activity which means when the activity is paused, all the fragments available in the activity will also be stopped.

- **How to pass items to `fragment`?**

  Using `Bundle` you can pass items to the fragment.

- **How would you communicate between two `fragments`?**

  There are several ways to communicate two fragments. Using `interfaces` are a common way to do that. You can connect two fragments through interfaces that are implemented in the parent activity.

- **Difference between adding/replacing `fragment` in `backstack`?**
  - `replace` removes the existing `fragment` and adds a new `fragment`.
    This means when you press back button the fragment that got replaced will
    be created with its onCreateView being invoked.

  - `add` retains the existing fragments and adds a new `fragment` that means
    existing fragment  will be active and they wont be in 'paused' state hence
    when a back button is pressed onCreateView is not called for the existing
    fragment(the fragment which was there before new fragment was added).

    In terms of fragment’s life cycle events `onPause()`, `onResume()`,
    `onCreateView()` and other life cycle events will be invoked in case of
    `replace` but they wont be invoked in case of `add`.

- **What is the difference between `dialog` and `dialogFragment`?**

  THe `dialog` is a small window that prompts the user to make a decision or enter additional information. Instead, `dialogFragment` is a fragment that displays a dialog windows and contains a dialog object.

  DialogFragment does various things to keep the fragment's lifecycle driving it, instead of the Dialog. Dialogs are generally autonomous entities -- they are their own window, receiving their own input events, and often deciding on their own when to disappear. DialogFragment needs to ensure that what is happening with the Fragment and Dialog states remains consistent. To do this, it watches for dismiss events from the dialog and takes care of removing its own state when they happen.

- **What is the difference between `Thread` and `AsyncTask`?**

- **What is the relationship between the life cycle of an `AsyncTask` and an `Activity`? What problems can this result in? How can these problems be avoided?**

  An AsyncTask is not tied to the life cycle of the Activity that contains it.
  So, for example, if you start an AsyncTask inside an Activity and the user
  rotates the device, the Activity will be destroyed (and a new Activity
  instance will be created) but the AsyncTask will not die but instead goes
  on living until it completes.

  Then, when the AsyncTask does complete, rather than updating the UI of the
  new Activity, it updates the former instance of the Activity (i.e., the one
  in which it was created but that is not displayed anymore!). This can lead to
  an Exception (of the type java.lang.IllegalArgumentException: View not attached
  to window manager if you use, for instance, findViewById to retrieve a view
  inside the Activity).

  There’s also the potential for this to result in a memory leak since the
  AsyncTask maintains a reference to the Activity, which prevents the Activity
  from being garbage collected as long as the AsyncTask remains alive.

  For these reasons, using AsyncTasks for long-running background tasks is
  generally a bad idea . Rather, for long-running background tasks, a different
  mechanism (such as a service) should be employed.

- **What is `Lopper` and how it works?**
- **What are Handlers?**

    Handlers are objects for managing threads. It receives messages and writes
    code on how to handle the message. They run outside of the activity’s
    lifecycle, so they need to be cleaned up properly or else you will have
    thread leaks. Handlers allow communicating between the background thread
    and the main thread.

- **What is the difference between `Foreground` and `Background` and `Bounded` service?**
  - __Foreground Service:__ A foreground `service` performs some operation that
  is noticeable to the user. For example, we can use a foreground service to
  play an audio track. A `Notification` must be displayed to the user.

  - __Background Service:__ A background `service` performs an operation that
  isn’t directly noticed by the user. In Android API level 26 and above, there
  are restrictions to using background services and it is recommended to use
  WorkManager in these cases

  - __Bound Service:__ A `service` is bound when an application component binds
  to it by calling `bindService()`. A bound service offers a client-server
  interface that allows components to interact with the `service`, send requests,
  receive results. A bound service runs only as long as another application
  component is bound to it. [Read More](https://developer.android.com/guide/components/services)

- **What are the limitations of using `Services` in android 8 and higher?**
- **What is `JobScheduling`?**
- **What is `contentProvider` and what is typically used for?**

  A `ContentProvider` provides data from one application to another, when
  requested. It manages access to a structured set of data. It provides mechanisms for defining data security. [Learn more]("https://medium.com/@sanjeevy133/an-idiots-guide-to-android-content-providers-part-1-970cba5d7b42" "An idiot guide to android content providers").
  For further reading see the [official android documentation]("https://developer.android.com/guide/topics/providers/content-provider-basics" "Android official documentation")

  ![Conent Provider diagram](/assets/images/content-provider-diagram.png)

- **What is the difference between `apply()` and `commit()` in `sharedPreferences`?**
  - `commit()` writes the data **synchronously** and returns a boolean value of
    success or failure depending on the result immediately.

  - `apply()` is **asynchronous** and it won’t return any boolean response. Also
    if there is an `apply()` outstanding and we perform another `commit()`,
    The `commit()` will be blocked until the `apply()` is not completed.

- **How you load your `Bitmaps`? What do you do for loading large bitmaps?**
[Loading Large Bitmaps Efficiently in Android](https://android.jlelse.eu/loading-large-bitmaps-efficiently-in-android-66826cd4ad53 "Loading Large Bitmaps Efficiently in Android")

- **How Android apps compiled and run?**
  1. First step involves compiling the resources folder (/res) using the aapt
    (android asset packaging tool) tool. These are compiled to a single class
    file called R.java. This is a class that just contains constants.

  2. Second step involves the java source code being compiled to .class files
    by javac, and then the class files are converted to Dalvik bytecode by the
    “dx” tool, which is included in the sdk ‘tools’. The output is classes.dex.

  3. The final step involves the android apkbuilder which takes all the input
    and builds the apk (android packaging key) file.

- **Do you know any about how `Dalvik` is working?**
- **What are the benefits of `ART` in comparison to `Dalvik`?**
- **What is `AAPT` ?**
- **What is Doze mode?**

<br>

### 5. Architecture And Coding

- **What is MVVM stands for?**

- **What are the differences between MVP and MVVM?**
- **Explain SOLID programming principle?**
- **What is Dependency Inversion?**
- **What is Dependency Injection?**
- **What is repository pattern?**
- **What is android clean architecture?**


<br>

### 6. Tools and libraries

- **What is android DataBinding?**

- **Explain `scope` concept in dagger2**
- **What is marble diagram?**
- **Explain different types of Observables**
- **How to implement instant search with RxJava?**


<br>

### 7. Gradle

- **What is buildType?**

- **What do you do if you want to publish different versions of an APK with the same codabase?**

    *using product flavor.* [What is flavor?]("https://android.jlelse.eu/product-flavors-for-android-library-d3b2d240fca2")

- **How to add a dependency only on a certain build of the app?**

  Flavor dependency. What? don't worry, [read this link]("https://developer.android.com/studio/build/dependencies#dependency-configurations")

- **What is the difference between `implementation` and `api`?**

  These two keywords work the same when you want to add a new library but the main difference occurs when using it in the internal library. Let's explain it with an example. Consider your app has a library called 'libraryA'. This library is also dependant on another library called 'libraryB'. the dependency flow will be : `app -> libraryA -> libraryB` . If the libraryB is declared in libraryA with keyword `implementation`, so your app module does not know anything about the classes of libraryB. So you can't access and use any classes of libraryB. If you want to do that, you must declare libraryB in the libraryA Gradle file with keyword `api`. For more information read [this medium link]("https://medium.com/mindorks/implementation-vs-api-in-gradle-3-0-494c817a6fa").


- **What do you mean by Gradle wrapper?**

  The Gradle wrapper is the most suitable way to initiate a Gradle build. A Gradle wrapper is a Window’s batch script which has a shell script for the OS (operating system). Once you start the Gradle build via the wrapper, you will see an auto download which runs the build.

<br>

### 8. Design patterns

According to a report by [codespaghetti]("http://www.codespaghetti.com/java-design-pattern-interview-questions/"), The most design patterns that you must to know are **Singleton**, **Factory**, and **Builder**. I didn't bring the typical questions like what is a singleton, factory, and... . I imagine you fluent on these patterns and instead, I will focus on the other side of questions that may asked in the interview meeting.

![Top 5 java design pattern interview questions](/assets/images/design-patterns-report.png)

- **When to use Adapter pattern? (Not for RecyclerView or ListView)**

  Use Adapter pattern when you need to make two class work with incompatible interfaces. Adapter pattern can also be used to encapsulate third party code so that your application only depends upon Adapter, which can adapt itself when third party code changes or you moved to a different third party library.

- **In singleton pattern whether it is better to make the whole `getInstance()` method synchronized or just critical section is enough? Which one is preferable?**

  Synchronization of whole `getInstance()` method is costly and is only needed during the initialization on singleton instance, to stop creating another instance of Singleton.  Therefore it is better to only synchronize critical section and not the whole method.

- **How many ways can you write singleton class in Java?**

  One can write singleton class in Java in five ways

    - Classic Java Singleton pattern
    ```java
    Public class Singleton{

        private static Singleton instance;

        private Singleton(){          
        }

        public static Singleton getInstance(){
          if(instance == null)
            instance = new Singleton();
          return instance;
        }

    }

    ```

    - A thread-safe singleton pattern in java using Synchronization

    ```java
    public class Singleton{

        private static final Singleton instance = null;

        private Singleton(){}

        public synchronized static Singleton getInstance(){
            if(instance == null)
                instance = new Singleton();

            return instance;
        }
    }
    ```

    - Double-checked locking with volatile keyword

    ```java
    public class Singleton {

        private volatile static Singleton instance;

        private Singleton (){}

        public static Singleton getSingleton() {          
          if (instance == null) {                                     
            synchronized (Singleton.class) {              
                if (instance == null)                    
                    instance = new Singleton();                                    
                }            
          }          
          return instance;        
        }

    }    
    ```

    - Initialization-on-demand with singleton holder

    ```java
    // Correct lazy initialization in Java
    @ThreadSafe
    class Singleton {

        private Singleton() {}

        private static class SingletonHolder {
            public static Singleton instance = new Singleton();
        }

        public static Singleton getInstance() {
            return SingletonHolder.instance;
        }
    }
    ```

    - Using Enum

    ```java
    enum Color {

        RED(1), GREEN(2), YELLOW(3);

        private int nCode ;

        private Color( int _nCode) {
          this.nCode = _nCode;
        }

        @Override
        public String toString() {
          return String.valueOf ( this . nCode );
        }

    }

    public class ColorTest {
        public static void main(String[] args) {
            Color red = Color.RED;
            Color red2 = Color.RED;

            System.out.println(red == red2); // return true
        }
    }
    ```
<br>
- **What are the drawbacks of using singleton design pattern?**

  - **Testability issue:** The bad thing with singletons is that the
  `getInstance()` method is globally accessible. That means that you usually
  call it from within a class, instead of depending on an interface you can
  later mock. That's why it's impossible to replace it when you want to test
  the method or the class.

  - **Tight Coupling:** The singleton object is exposed globally and is
  available to a whole application. Thus, classes using this object become
  tightly coupled. So any change in the global object will impact all other
  classes using it.

  - **Violation issues:** Singleton principle can be violated by techniques such
  as cloning. If an application is running on multiple JVM’s, then, in this case,
  Singleton might be broken.

- **How can you prevent creating another instance of singleton using `clone()` method?**

  The preferred way to prevent creating another instance of a singleton is by not implementing Cloneable interface and if you do just throw an exception from `clone()` method "_not to create a clone of singleton class_".

- **When will you prefer to use a Factory Pattern?**

  The factory pattern is preferred in the following cases:
    - A class does not know which class of objects it must create

    - Factory pattern can be used where we need to create an object of any one of sub-classes depending on the data provided

    - you can use factory pattern where you have to create an object of any one of sub-classes depending on the given data


- **Why use a factory class to instantiate a class when we can use new operator?**

  Factory classes provide flexibility in terms of design. Below are some of the
  benefits of factory class:

    - Factory design pattern results in more decoupled code as it allows us to
      hide creational logic from dependent code
    - It allows us to introduce an [Inversion of Control]("https://www.codeproject.com/Articles/592372/Dependency-Injection-DI-vs-Inversion-of-Control-IO" "What is IoC?") container
    - It gives you a lot more flexibility when it comes time to change the
      application as our creational logic is hidden from dependant code

- **What is the difference between factory and abstract factory design pattern?**

  Both factory and abstract factory are creational design patterns. The major
  difference between these two is, a factory pattern creates an object through
  inheritance and produces only one Product. On the other hand, an abstract
  factory pattern creates the object through composition and produce families
  of products. In other word an abstract factory is "factory of factories". You can find an example [___here___]("https://www.journaldev.com/1418/abstract-factory-design-pattern-in-java").

- **(My Favorite question!) Suppose we are building an application for a pizza
store and we need to model their pizza classes. Assume they offer four types
of pizzas namely Peppy Paneer, Farmhouse, Margherita and Chicken Fiesta. Each
pizza has a different cost. We have overridden the getCost() in the subclasses
to find the appropriate cost. Now let's become it more interesting! suppose a
new requirement, in addition to a pizza, customer can also ask for several
toppings such as Fresh Tomato, Paneer, Jalapeno, Capsicum, Barbeque, etc.
Toppings may be redundant and it's OK. (It means a customer may choose double
jalapeno or three-time barbeque). Each topping has its price and by adding
each one the total cost of the pizza will be increased. If you have to suggest
only one design pattern to solve this problem, choose which one? why? and
How you implement it?**

- **If you couldn't find a solution to the previous question, don't worry and
follow this one. It can help you to find out how to solve it. The question is,
Which design pattern allows you to implement the inheritance approach at the
runtime?**

- **which pattern is used when we need to decouple an abstraction from its implementation?**

  When we want to decouple an abstraction from its implementation in order that two can vary independently we use **bridge pattern**.



<br>

### 9. Data structure and algoritms

_NOTICE: For D.S. questions, the responses will not be added_ \^\_\^

- **What are the differences between Array and linkedList?**
- **What are the differences between Array and ArrayList?**

- **Find duplicate an item in a non-sorted list?**
- **How to implement a stack using queue?**

- **How do you find the largest and smallest number in an unsorted integer array?**
- **Given an array of size n with range of numbers from 1 to n+1. The array doesn’t contain any duplicate, one number is missing, find the missing number.**
- **A sorted array is rotated at some unknown point, how to efficiently search an element in it.**
- **How to find if two given rectangles overlap?**
- **How to swap two integers without swapping the temporary variable in Java?**
- **How do you check if a string contains only digits?**
- **How to sort a list?**

### Core Android

-   **What are SOLID Principles? How they are applicable in Android?**<br/>
    A) SOLID unites all the best practices of software development over the years to deliver good quality apps. Understanding SOLID Principles will help us write clean and elegant code. It helps us write the code with SOC (Separation of Concerns).
    SOLID Principles is an acronym for:
    1. S stands for Single Responsibility Principle(SRP) - A class should have only one reason to change
    2. O stands for Open Closed Principle - Software entities such as classes, functions, modules should be open for extension but closed for modification.
    3. L stands for Liskov Substitution Principle - Derived class must be usable through the base class interface, without the need for user to know the difference.
    4. I stands for Interface Segregation - No client should be forced to depend on methods that it doesn't use.
    5. D stands for Dependency Inversion - 
       1. High Level Modules should not directly depend on Low level modules. Instead both should depend on abstractions.
       2. Abstractions should not depend on details. Details should depend on abstractions.

    [Learn More about SOLID principles with Android Examples Here.](https://www.coderefer.com/blog/solid-principles-in-android-with-kotlin-examples/)

-   **Android Architecture**<br/>
    A) <br/>
    ![Android Architecture Image](/assets/android-architecture.png)

-   **What are Android Components?**<br/>
    A) 1) Activities,
    2) Intent and broadcast receivers,
    3) Services,
    4) Content Providers,
    5) Widgets and Notifications

-   **What is an Application class?**<br/>
    A) An Application class is a base class in your Application that starts before all other classes like Activities or services are called. You can maintain your application's global state here. While it is NOT mandatory that you need to extend Application class, you can do so by providing your own implementation by creating a subclass and specifying the fully-qualified name of this subclass as the "android:name" attribute in your AndroidManifest.xml's <application> tag.

-   **What is a Context? What are different types of Contexts?**<br/>
    A) As the name says, its the context of the current application or object. Context is like a handle to the environment your application is currently running in.
    We mainly use two types of context. Application context - whose scope is throughout the application and Activity Context - whose scope depends on the Activity Lifecycle.

-   **What is an Activity?**<br/>
    A) An activity provides the window in which the app draws its UI. This window typically fills the screen, but may be smaller than the screen and float on top of other windows. Generally, one activity implements one screen in an app. For instance, one of an app’s activities may implement a Preferences screen, while another activity implements a Select Photo screen.

-   **Activity Lifecycle**<br/>
    A)<br/>
    ![Activity Lifecycle Image](/assets/activity_lifecycle.png)

-   **Fragment Lifecycle**<br/>
    A)<br/>
    ![Fragment Lifecycle Image](/assets/fragment_lifecycle.png)

-   **Service Lifecycle**<br/>
    A)<br/>
    ![Fragment Lifecycle Image](/assets/service_lifecycle.png)

-   **What is the correlation between activity and fragment life cycle?**<br/>
-   A) <br/>
    Here is how Activity's and Fragment's lifecyle are called together:
    ![Activity Fragment Lifecycle](/assets/activity-fragment-lifecycles.png)

-   **Is there any scenario where onDestoy() will be called without calling onPause() and onStop()?**<br/>
    A) If we call finish() method inside onCreate() of our Activity, then onDestroy() will be called directly.

-   **What are Processes in Android?**<br/>
    A) Everytime an Android App starts, the Android System creates a New Process for this Application with a Single thread of Execution. By default all the components of the same application runs in the same process. While most apps donot change this behavior, some apps like games, might want to run in different processes. Then we can use *android:process* attribute in our AndroidManifest.xml to specify the process name.

-   **How do we save and restore an activity's state during screen screen rotation?**<br/>
    A) We can use onSavedInstanceState(bundle:Bundle) to save the activity's state inside a bundle. Then we can use onRestoreInstanceState(bundle) to restore the state of activity.

-   **What is a Loader in Android?**<br/>
    A) Note: (Loader is Deprecated. We Have to use combination of ViewModels and LiveData instead of using Loaders) A Loader is used to fetch the data from a Content provider and cache the results across the configuration changes to avoid duplicate queries. Loader does it by running on separate threads and handling the lifecycle changes (so no need of asynctasks or new thread creations or manual handling of life cycle changes). Few implementations of Loaders like CursorLoader can implement an observer (called ContentObserver) to monitor any data changes and can then trigger a reload.

-   **What is an Intent Filter?**<br/>
    A) Intent filters are a very powerful feature of the Android platform. They provide the ability to launch an activity based not only on an explicit request, but also an implicit one. For example, an explicit request might tell the system to “Start the Send Email activity in the Gmail app". By contrast, an implicit request tells the system to “Start a Send Email screen in any activity that can do the job." When the system UI asks a user which app to use in performing a task, that’s an intent filter at work. Here's an example of how to declare Intent Filter in AndroidManifest:
    ```xml
    <activity android:name=".ExampleActivity" android:icon="@drawable/app_icon">
      <intent-filter>
          <action android:name="android.intent.action.SEND" />
          <category android:name="android.intent.category.DEFAULT" />
          <data android:mimeType="text/plain" />
      </intent-filter>
    </activity>
    ```


-   **What is an Intent?**<br/>
    A) It is a kind of message or information that is passed to the components. It is used to launch an activity, display a web page, send SMS, send email, etc. There are two types of intents in android:
    a)Implicit Intent
    b)Explicit Intent

-   **What is AAPT?**<br/>
    A) AAPT2 (Android Asset Packaging Tool) is a build tool that Android Studio and Android Gradle Plugin use to compile and package your app’s resources. AAPT2 parses, indexes, and compiles the resources into a binary format that is optimized for the Android platform.

-   **What is an Intent?**<br/>
    A) Intent is basically a message passing mechanism between different components of Android, except for Content Provider. You can use intent to start any component in Android.

-   **What are the different types of Intents?**<br/>
    A) There are two types of intents:

    Explicit intents specify which application will satisfy the intent, by supplying either the target app's package name or a fully-qualified component class name. You'll typically use an explicit intent to start a component in your own app, because you know the class name of the activity or service you want to start. For example, you might start a new activity within your app in response to a user action, or start a service to download a file in the background.
    Implicit intents do not name a specific component, but instead declare a general action to perform, which allows a component from another app to handle it. For example, if you want to show the user a location on a map, you can use an implicit intent to request that another capable app show a specified location on a map.

-   **What is HandlerThread?**<br/>
    A) HandlerThread is a Handy class to start a thread that has a Looper.

-   **What is a Looper?**<br/>
    A) A Looper is a class used to loop through the Message Queue attached to the Thread. Any thread consists of only one looper.
    
    You can access message queue of current thread by using **Looper.myQueue()**.
    
    By default, a thread halts when the execution completes. But, for Example, if we take Android's Main thread, it should not halt upon execution.

    Normally thread cannot be reused once its job is completed. But thread with Looper is kept alive until you call quit method so you don’t need to create a new instance each time you want to run a job in background.

    Rather it should loop through the runnables(Messages) that its assigned in order to work properly. For more info, refer to this [link](https://stackoverflow.com/a/34522758/3424919).

-   **What is a Message Queue?**<br/>
    A) MessageQueue is a queue that has list of messages which should be processed. Android maintains a MessageQueue on the main thread.
    [More Info](https://medium.com/@ankit.sinhal/messagequeue-and-looper-in-android-3a18c7fc9181)

-   **What is a Message ?**<br/>
    A) Message contains a description and arbitrary data object that can be sent to a Handler. Basically its used to process / send some data across threads.

-   **What is a Service?**<br/>
    A) A service is a component which doesn't have UI and can perform long running operations like downloading stuff, playing music etc.. which can run even exiting the application. By default service runs on main thread. This might cause ANR errors. To avoid this, we can Start service by creating a new background thread or use an IntentService that can do work in background. [Read More.](https://developer.android.com/guide/components/services)

-   **How to Stop a Service?**<br/>
    A) To stop a service from an activity we can call stopService(Intent intent) method. To Stop a service from itself, we can call stopSelf() method.

-   **What are different types of services?**<br/>
    A) These are the three different types of services:

    **Foreground Service:**
    A foreground service performs some operation that is noticeable to the user. For example, an audio app would use a foreground service to play an audio track. Foreground services must display a Notification. Foreground services continue running even when the user isn't interacting with the app. <br/>
    **Background Service:**
    A background service performs an operation that isn't directly noticed by the user. For example, if an app used a service to compact its storage, that would usually be a background service. However there are restrictions to use background services from Android API 26 and above. We can use WorkManager to defer these background tasks.<br/>
    **Bound Service:**
    A service is bound when an application component binds to it by calling bindService(). A bound service offers a client-server interface that allows components to interact with the service, send requests, receive results, and even do so across processes with interprocess communication (IPC). A bound service runs only as long as another application component is bound to it. Multiple components can bind to the service at once, but when all of them unbind, the service is destroyed by the system.
    [Read More](https://developer.android.com/guide/components/services#Types-of-services)

-   **Bound Service vs UnBounded service?**<br/>
    A) A Bound service is started by using method bindService(). As mentioned above system destroys bound service when no application component is accessing it.
    Unbounded service (started service) is started by using a method called startService(). Once started, it will run indefinitely even if the application component that started it is destroyed.

-   **When does a Bound Service stops?**<br/>
    A) A Bound Service will stop automatically by the system when all the Application Components bound to it are unbinded.
    
-   **How to start a Foreground Service?**

    A) We can start a foreground service by using startForegroundService(Intent intent) or by internally calling startForeground() on the service.

    For Example, [Click Here](https://github.com/vamsitallapudi/Coderefer-Android-Projects/tree/main/ServicesExample)

-   **What is Sticky Intent in Android?**  
    
    A) Sticks with Android, for future broadcast listeners. For example if BATTERY_LOW event occurs then that Intent will stick with Android so that any future requests for BATTERY_LOW, will return the Intent.

-   **What is Pending Intent in Android?**<br>
    A) Pending Intent is an intent which you want to trigger at some time in future, even when your application is not alive. This intent can be used by other application which allows it to execute that intent with the same permissions as of our application.

    ```java
    Intent intent = new Intent(this, AnyActivity.class);

    // Creating a pending intent and wrapping our intent
    PendingIntent pendingIntent = PendingIntent.getActivity(this, 1, intent, PendingIntent.FLAG_UPDATE_CURRENT);
    try {
        // Perform the operation associated with our pendingIntent
        pendingIntent.send();
    } catch (PendingIntent.CanceledException e) {
        e.printStackTrace();
    }
    ```

    PendingIntent uses the following methods to handle the different types of intents:

    ```java
    PendingIntent.getActivity();//Retrieves a PendingIntent to start an Activity
    PendingIntent.getBroadcast();// Retrieves a PendingIntent to perform a Broadcast
    PendingIntent.getService();// Retrieves a PendingIntent to start a Service
    ```


-   **What is the difference between START_NOT_STICKY, START_STICKY AND START_REDELIVER_INTENT?**
-   
    A) **START_NOT_STICKY:**<br>
    If the system kills the service after onStartCommand() returns, do not recreate the service unless there are pending intents to deliver. This is the safest option to avoid running your service when not necessary and when your application can simply restart any unfinished jobs.
    
    **START_STICKY:**<br>
    If the system kills the service after onStartCommand() returns, recreate the service and call onStartCommand(), but do not redeliver the last intent. Instead, the system calls onStartCommand() with a null intent unless there are pending intents to start the service. In that case, those intents are delivered. This is suitable for media players (or similar services) that are not executing commands but are running indefinitely and waiting for a job.

    **START_REDELIVER_INTENT:**<br>
    If the system kills the service after onStartCommand() returns, recreate the service and call onStartCommand() with the last intent that was delivered to the service. Any pending intents are delivered in turn. This is *suitable for services that are actively performing a job that should be immediately resumed, such as downloading a file.*

-   **What is Pending Intent?**
   
    A)A PendingIntent is a token that you give to a foreign application (e.g. NotificationManager, AlarmManager, Home Screen AppWidgetManager, or other 3rd party applications), which allows the foreign application to use your application's permissions to execute a predefined piece of code. It specifies a task that requires to be performed in future.

-   **What is an Intent Service? What is the method that differentiates it to make Service run in background?**

    A) IntentService is a subclass of Service that can perform tasks using worker thread unlike service that blocks main thread. The additional method of IntentService is -
    **<i>onHandleIntent(Intent)</i>** which helps the IntentService to run a particular code block declared inside it, in worker/background thread. The speciality of Intent Service is if there are more tasks given to it, IntentService will pass those intents one by one to the Worker thread. So if there are multiple download operations to be handled, They will be performed in a sequential order. Only one request will be processed at a time.

    **Note:** IntentService is deprecated from API 30. This is due to background restrictions imposed from API level 26. It is now recommended to use WorkManager or JobIntentService. For more Info, [Click Here](https://developer.android.com/reference/android/app/IntentService)

-   **How to Stop an IntentService?**<br/>
    A) An IntentService automatically stops itself after its job is done. We do not need to explicitly call any methods to stop an IntentService unlike Service which requires stopSelf() or StopService(intent:Intent).

-   **When Intent Service is Useful?**<br/>
    A) The IntentService can be used in long tasks usually with no communication to Main Thread. If communication is required, can use Main Thread handler or broadcast intents. Another case of use is when callbacks are needed (Intent triggered tasks).

-   **Advantage of Retrofit over Volley?**<br/>
    A) Retrofit is type-safe. Type safety means that the compiler will validate request and response objects' variable types while compiling, and throw an error if you try to assign the wrong type to a variable.

-   **Advantage of Volley over Retrofit?**<br/>
    A) Android Volley has a very elaborate and flexible cache mechanism. When a request is made through Volley, first the cache is checked for Response. If it is found, then it is fetched and parsed, else, it will hit Network to fetch the data. Retrofit does not support cache by default.

-   **What are different launch modes available in Android?**<br/>
    A) There are four launch modes for an Activity in Android as follows:

    1) <b>standard</b> : Creates a new instance of an activity in the task from which it is started every single time. It is the default mode if not declared. 
    <br/>Eg: If we have an activity stack of A->B->C, If we launch Activity C again using standard Mode, the activity stack will now be A->B->C->C. We can see that two instances of C are present in the activity stack.

    1) <b>singleTop</b> : Same as standard except that if the activity is at the top of the stack, then the same instance will be used. Now the existing Activity at the top will receive the intent through a call to its onNewIntent() method.
     <br/>Eg: If we have an activity stack of A->B->C, If we launch Activity C again using singleTop Mode, the activity stack remains to be A->B->C. However if we launch B, then B will be added as new Instance to the stack (A->B->C->B).

    2) <b>singleTask</b> : A new task will be created and activity will be created at the root of this new task whenever we use launch mode as singleTask. However, if there is already a separate task with same instance, the system will call that activity's onNewIntent() method to route the intent. There can only be one instance of activity existing at a time.
    <br/>Eg: If our activity stack is A->B->C and if we launch D using singleTask, it will be A->B->C->[D]. Here braces represents the stack in separate task. If we call E using standard mode, then it will be A->B->C->[D->E].<br/>
    If we have A->B->C and if we call B again using singleTask launch Mode, the stack will now be A->[B] with B in a separate task. Activity C will be destroyed.

    1) <b>singleInstance</b> : Same as Single Task except it creates a new activity in a task and no other activities can then launched into that task. That task will forever contains only that activity. If we use standard or singleTop to launch another activities, they are launched into another tasks.
    <br/>Eg: if the Activity stack is A->B and now we launched C using singleInstance Launch Mode, the new stack will be A->B->[C]. Now if we call a new activity D from C, it will be launched into separate task. Now the new stack will be A->B->[C]->[D].  Now if we launch E from activity B, Then new stack will be A->B->E [C]->[D]. If we call C again, onNewIntent() of C will be called and new stack will be A->B->E->[C] [D].

    You can read more about them [here](https://developer.android.com/guide/components/activities/tasks-and-back-stack#ManifestForTasks).

-   **How do you declare the launch mode in your application?**<br/>
    A) via manifest, in activity's tag. For Eg., -> android:launchMode="singleTask"


-   **How to handle crashing of AsyncTask during screen rotation?**<br/>
    A) 
    One way is by cancelling the AsyncTask by using cancel() method on its instance. It will call onCancelled() method of AsyncTask where we can do some clean-up activities like hiding progress bar etc.
    The best way to handle AsyncTask crash is to create a RetainFragment, i.e., a fragment without UI as shown in the gist below: https://gist.github.com/vamsitallapudi/26030c15829d7be8118e42b1fcd0fa42
    We can also avoid this crash by using 2 Alternatives -  1) Using RxJava by subscribing and unsubscribing at onResume() and onPause() methods respectively, 2) Using LiveData - lifecycle aware component.

-  **What is a RetainFragment / Headless Fragment?**<br/>
    Generally, Fragments are destroyed and recreated along with their parent Activity’s whenever a configuration change occurs. Calling setRetainInstance(true) allows us to bypass this destroy-and-recreate cycle, notifying the system to retain the current instance of the fragment when the activity is recreated.

-  **Difference between serializable and parcelable? Why android introduced Parcelable?**<br/>
    A) Serializable uses reflection while for parcelable, developers from android team wrote custom code that performs manual marshalling(converting data into byte stream) and unmarshalling(converting the byte stream back to their original data). Usually Parcelable is considered faster than Serializable.

-  **What is Reflection?**<br/>
    A) Reflection is an API that is used to examine or modify the behaviour of methods, classes and interfaces at runtime. The required classes for reflection are present in java.lang.reflect package.

-  **How to reduce your app size?**<br/>
    A)
    1. setting minifyEnabled to true
    2. setting shrinkResources to true
    3. using bundle instead of apk in developer console
    4. converting the images to vector drawables.

-   **What is the advantage of using Retrofit over AsyncTask?**<br/>
    A) Retrofit reduces boiler plate code by internally using GSON library which helps parsing the json file automatically.
    Retrofit is a type safe library. This means - it checks if wrong data type is assigned to variables at compilation time itself.
    More use-cases at: https://stackoverflow.com/a/16903205/3424919

-   **How to handle multiple network calls using Retrofit?**<br/>
      A) In Retrofit, we can call the operations asynchronously by using enqueue() method where as to call operations synchronously, we can use execute() method. In addition, we can use zip() operator from RxJava to perform multiple network calls using Retrofit library.

-   **What is the role of Presenter in MVP?**<br/>
    A) The Presenter is responsible to act as the middle man between View and Model. It retrieves data from the Model and returns it formatted to the View. But unlike the typical MVC, it also decides what happens when you interact with the View.

-   **What is the advantage of MVVM over MVP?**<br/>
    A) In MVP, Presenter is responsible for view data updates as well as data operations where as in MVVM, ViewModel does not hold any reference to View. It is the View's responsibility to pick the changes from ViewModel. This helps in writing more maintainable test cases since ViewModel does not depend upon View.

-    **When to use AsyncTask and when to use services?**<br/>
    A) Services are useful when you want to run code even when your application's Activity isn't open. AsyncTask is a helper class used to run some code in a separate thread and publish results in main thread. Usually AsyncTask is used for small operations and services are used for long running operations.

-    **When to use a service and when to use a thread?**<br/>
    A) We will use a Thread when we want to perform background operations when application is running in foreground. We will use a service even when the application is not running.

-   **What is a Handler?**<br/>
    A) A Handler allows you to send and process Message and Runnable objects associated with a thread's MessageQueue. Each Handler instance is associated with a single thread and that thread's message queue. When you create a new Handler, it is bound to the thread / message queue of the thread that is creating it -- from that point on, it will deliver messages and runnables to that message queue and execute them as they come out of the message queue. We will generally use handler class when we want to repeat task every few seconds.

-   **How to save password safely in Android?**<br/>
    A) Using Android Keystore<br/>
    <https://medium.com/@josiassena/using-the-android-keystore-system-to-store-sensitive-information-3a56175a454b>

-  **What is Alarm Manager?**<br/>
    A) AlarmManager is a class which helps scheduling your Application code to run at some point of time or at particular time intervals in future. When an alarm goes off, the Intent that had been registered for it is broadcast by the system, automatically starting the target application if it is not already running. Registered alarms are retained while the device is asleep (and can optionally wake the device up if they go off during that time), but will be cleared if it is turned off and rebooted.

-   **How can I get continuous location updates in android like in Google Maps?**<br/>
    A) We can use Fused location provider in Android set our interval in that.
    https://stackoverflow.com/a/41500910/3424919


### Android Security Related
-   **How do you know if the device is rooted?**<br/>
    A) We can check if superUser apk is installed in the device or if it contains su file or xbin folder. Alternatively you can use [RootBeer](https://github.com/scottyab/rootbeer) library available in GitHub.
    <br/>
    For code part, click [Here](https://stackoverflow.com/a/35628977/3424919).
-   **What is Symmetric Encryption?**

    A) Symmetric encryption deals with creating a passphrase and encrypting the file with it. Then the server needs to send this passphrase(key) to the client so that the client can decrypt. Here the problem is sending that key to decrypt the file. If Hackers can access that key, they can misuse the data.

-   **What is Asymmetric Encryption?**

    A) Using algorithms like RSA, AES256, etc., the server generates 2 keys - public key and private key. The server then gives public key to clients. Client then encrypts the sensitive data with that public key and send it back to server. Now as the server alone has the private key, only it can decrypt the data. This is the most efficient way of sending data across the client and server.
    
    Example of this Asymmetric encryption are HTTPS using SSL certificate, Blockchain technologies like Bitcoin, etc.

    For more info, refer to this [video](https://youtu.be/AQDCe585Lnc)

-   **How do you encrypt the Data in Java?**
  
    A) Using javax.crypto package's Cipher class. We can call the methods such as encrypt() or decrypt() from the Cipher class to encode or decode our data.

    To see Cipher in action, see the following [code commit](https://github.com/vamsitallapudi/Coderefer-Java-Projects/commit/443c4f7700fd68391da2ccf40f85a7e3bccd573d#diff-25a6634263c1b1f6fc4697a04e2b9904ea4b042a89af59dc93ec1f5d44848a26).

-   **What is SSL Pinning?**

    A)Generally SSL Certificates are issued by CAs (Certificate Authorities). SSL Certificates are used to secure a connection between a Client and a Server. But there might be some chances that if any CA is breached, our app becomes vulnerable to MITM (Man in the Middle Attack). To mitigate this problem, we can pin our Server's SSL Certificate in our Application as an additional security layer so that we can check if the certificate is really from our server or not. In few words, SSL Pinning is to increase security. Disadvantages is if the server changes the certificate, Client app needs a software update.

-   **How do you implement it in Android?**
    
    A) SSL Pinning can be done using OkHttpClient's Builder methods as follows:
    ```Kotlin
        val certificatePinner = CertificatePinner.Builder()
        .add(
            "www.coderefer.com",
    "sha256/ZCOF65ADBWPDK8P2V7+mqodtvbsTRR/D74FCU+CEEA="
        )
        .build()
    val okHttpClient = OkHttpClient.Builder()
        .certificatePinner(certificatePinner)
        .build()
    ```

    Then you supply this generated okHttpClient object to Retrofit.
    
    For more info, click on this [link](https://appmattus.medium.com/android-security-ssl-pinning-1db8acb6621e).

### Android Memory Related

-   **How do you create a Memory Leak in Android?**<br/>
    A) By passing the context to static block (class or method), we can create a Memory Leak.

-   **How do you avoid a Memory Leak in Android?**<br/>
    A) By making the objects eligible for GC (Garbage Collection) after a class (Activity or Fragment) is destroyed. We can also use Weak References like WeakHashMaps to loosely hold the data and make it easily available to GC.

-   **How do you identify a Memory Leak in Android?**<br/>
    A) By using Profiler in Android Studio or by using LeakCanary Library in Android.

### Android Battery Related
-   **How do you reduce battery consumption?**<br/>
    A) 
    1. Never poll the server for updates.
    2. Sync only when required. Ideally, sync when phone is on Wi-Fi and plugged in.
    3. Defer your work using WorkManager.
    4. Compress your data
    5. Defer non immediate requests until the phone is plugged in or wifi is turned on. The Wi-Fi radio uses significantly less battery than the mobile radio.


-   **How do you improve battery while fetching location for an app?**<br/>
    A) 
    1. By changing Accuracy -> we can use setPriority() to PRIORITY_LOW_POWER
    2. By changing Frequency of fetching location -> we can use setInterval() to specify the time interval
    3. By increasing latency -> After our call, we can wait for longer time - we can use setMaxWaitTime() to set large timeout.
   


### Dagger 2 Related Questions:

-   **What is Dependency Injection Pattern?**<br/>
    A) Dependency Injection pattern is where if our object requires other object, it will be passed to our object instead of us having to create that object. This other object is called as dependency.

-   **What is Service Locator Pattern?**<br/>
    A) Service Locator Pattern uses central Registry known as Service Locator which upon request provides objects for our class. This pattern has severe criticism that its an Anti-Pattern.

-   **What is Anti-Pattern?**<br/>
    A) An anti-pattern are certain patterns in software development that are considered bad programming practices.<br/>
    For more, click [Here](https://stackoverflow.com/a/980616/3424919).

-   **What is the use-case of @BindsInstance Annotation?**<br/>
    A) @BindsInstance is used to bind the available data at the time of building the Component. For example, while I needed to build dagger graph and username is already available to me, then I can bind that username to that dagger dependency graph as follows:
    
    ```java
        @Component.Builder
        interface Builder {
            @BindsInstance Builder userName(@UserName String userName);
            AppComponent build();
        }
    ```


-   **What is the use-case of @Module Annotation?**<br/>
    A) @Module is the Annotation used on the class for the Dagger to look inside it, to provide dependencies. We may be declaring methods inside the module class that are enclosed with @Provides annotation.

-   **What is the use-case of @Provides Annotation?**<br/>
    A) @Provides annotation is used on a method in Module class and can return / provide a Dependency object.

-   **What is the use-case of @Component Annotation?**<br/>
    A) @Component is used on Interface or abstract class. Dagger uses this interface to generate an implementation class with fully formed, dependency injected implementation, using the modules declared along with it. This generated class will be preceded by Dagger. For example if i create an interface named ProgramComponent with @Component annotation, Dagger will generate a Class named 'DaggerProgramComponent' implementing the  ProgramComponent interface.

-   **What is the use-case of @Scope Annotation?**<br/>
    A) @Scope is an annotation used on Interface to create a new Custom Scope. A Scope declaration helps to keep single instance of a class as long as its scope exists. For example, in Android, we can use @ApplicationScope for the object to live as long as the Application is live or @ActivityScope for the object to be available till the activity is killed.

-   **What is the use of Qualifier in Dagger?**<br/>
    A) We are often in a situation where we will be needing multiple objects with different instance values. For example, we need declare Student("Vamsi") and Student("Krishna"). In such case we can use a Qualifier to tell Dagger that we need multiple instances of same class. The default implementation of Qualifier is using @Named annotation, for eg., @Named("student_vamsi") and @Named("student_krishna")
    If we want to create a Custom Qualifier we would be using @Qualifier to declare a custom Qualifier interface.

-   **What is the use-case of @Inject Annotation in Dagger?**<br/>
    A) @Inject annotation is used to request dagger to provide the respective Object. We use @Inject on Constructor, Fields (mostly where constructor is not accessible like Activities, Fragments, etc.) and Methods.

### RxJava Related Questions:

More additional info to get started with RxJava is available at:
[Getting Started with RxJava2](https://www.coderefer.com/blog/rxandroid-tutorial-getting-started/)

-   **What is an Observable in RXJava2?**<br/>
    A) An Observable  simply emits the data to those which subscribed to it. All the emission is done asynchronously to the subscribers. A simple Observable can be created as follows:

    ```java
    // RxAndroid Tutorial - Adding Observable
    Observable<String> stringObservable = Observable.just("Hello Reactive Programming!");
    ```
-   **What is an Observer in RXJava2?**<br/>
    A) Observer consumes the data emitted by the Observable. To do this, Observer needs to subscribe to the Observable. Example shows how to create an Observable in RxJava2.
    ```java
    // RxAndroid Tutorial - Adding observer
    Observer<String> stringObserver = new Observer<String>() {
            @Override
            public void onSubscribe(Disposable d) {
            }

            @Override
            public void onNext(String s) {
                Toast.makeText(MainActivity.this, s, Toast.LENGTH_SHORT).show();
            }

            @Override
            public void onError(Throwable e) {
            }

            @Override
            public void onComplete() {
            }
        };
    ```

-   **How to Subscribe / Unsubscribe in RXJava?**<br/>
    A) We can make an Observer to subscribe to Observable as follows:
    ```java
    // RxAndroid tutorial - observer subscribing to observable
    stringObservable.subscribe(stringObserver);
    ```

-   **What are the different types of Observables in RxJava?**<br/>
    A)1) single
    2) Maybe
    3) Completable
    4) Observable
    5) Flowable

-   **What is a Single in RxJava?**<br/>
    A) A Single in RxJava is an Observable which emits only one item if completed or returns error.

-   **What is Maybe in RxJava?** <br/>
    A) A Maybe in RxJava is used when the Observable needs to emit a value or a no value or an error.

-   **What is Completable in RxJava?** <br/>
    A) A Completable in RxJava is an Observable which just completes the task and does not emit anything if completed. It returns an error if anything fails.
    It is similar to reactive concept of runnable.

-   **What is Back Pressure in RxJava?**<br/>
    A) Back Pressure is the state where your observable (publisher) is creating more events than your subscriber can handle.

-   **What is Flowable in RxJava?** <br/>
    A) A Flowable in RxJava is used when the Observable emits more data than the Observer can consume. In Other words, Flowable can handle back pressure where as an Observable cannot.

-   **What is a Cold Observable?**<br/>
    A) A Cold Observable is an Observable that does not emit items until a Subscriber subscribes. If we have more than one Subscriber, then the Cold Observable will emit each sequence of items to all Subscribers one by one.

-   **What is a Hot Observable?**<br/>
    A) A Hot observable is an Observer that will emit items

-   **Hot Observables vs Cold Observables**<br/>



-   **Explain about reactive programming?**<br/>

### Contributing to Android Interview Questions
Just make pull request. You are in!


