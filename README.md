# Android Interview Questions

## **The Android Ecosystem**

**What is Android?**

Android is a mobile operating system based on the Linux kernel and developed by Google. 

**What is DVM?** 

DVM stands for Dalvik Virtual Machine which was written by Dan Bornstein. DVM is an Android Virtual Machine for mobile devices. A standard Java compiler turns source code (written as text files) into Bytecode, then compiled into a .dex file that the Dalvik VM can read and use.

**What is the difference between DVM and JVM?** 

DVM in comparison to JVM (Java Virtual Machine) is faster. DVM is specifically designed for mobile devices. JVM is heavier.

**What does the Android architecture consist of?** 

The Android architecture consists of the Linux kernel, Libraries, Android Framework, Android applications.

**What are some of the components that are in the Library layer?** 

The DVM, The Media Framework, the SQLite.

**What are some of the components in the Android Framework layer?** 

The Activity Manager, The Window Manager, and The Content Providers.

**What are some of the components in the Application layer?** 

The camera, browser, contacts, and email.

**Which are the main components that can be used within and Android Application?** 

Activities, Services, Broadcast Receivers and Content Providers.

**What is AAPT (Android Asset Packaging Tool)?** 

Its part of the SDK and allows you to view, create, and update Zip-compatible archives (zip, jar, apk).

**What is APK?**

APK stands for Android Application Package. An APK file is the file format used for installing software on the Android operating system. It is a compressed package containing the whole project.

**What is the Android Context?**

It is an abstract class whose implementation is provided by the Android system. It gives the context of the current state of the application or the object.

**What is an Android App?**

It is a software application running on the Android Platform. It is a collection of different activities, services, receivers and listeners. It has a single manifest and is compiled into a single .apk file.

**What is NDK?**

NDK stands for Native Development Kit. NDK is a toolset that lets you implement parts of your app using native-code languages such as C and C++.

**When does Android App Not Responding (ANR) happen?**

ANR happens when the main thread is blocked for a few seconds. To avoid it, you should not use the main thread to read or write files, connect to the internet, and operate with databases.

**Which programming language is the Android framework written in?**

The Application and Framework layers are written in Java. The Drivers and the library layer are written in C and C++

**What devices may Android be run on?** 

Android may run on all electronic devices if the support Android hardware configurations. Example: cars, phones, laptops, watches, tvs, head phones, and so on.

## **Android Studio**

**Does Android Studio support version control Systems?**

Yes. Android Studio supports Git, GitHub, CVS, Mercurial, Subversion, and Google Cloud Source Repositories.

**What do you use the Logcat window in Android Studio for?**

The Logcat window displays system messages, such as when a garbage collection occurs, or messages that you added in your app with the Log class.

**If you want to profile your app's CPU, memory, and network performance, how can you do it inside the Android Studio?**

You can do it via the Android Profiler.

**Can you debug your app on the connected device?**

Yes, but you need to enable debugging in the device's developer options.

**What is Pixel Perfect?**

Pixel Perfect is a tool built into the Android Device Monitor that displays a magnified view of your app so you can inspect the position and properties of individual pixels in your layout, and help match your app's layout to design mockups.

**How can you capture a bug report from your device?**

You can achieve this either via the Take bug report developer option on the device, the Android Emulator menu, or the adb bug report command on your development machine.

**What is the Network Profiler used for?**

The Newtwork Profiler lets you examine how and when your app transfers data, and optimizes the underlying code appropriately.

**How can you identify memory leaks and memory churn that can lead to stutter, freezes, and even app crashes?**

Memory leaks and memory churn can be identified via the Memory Profiler, a component in the Android Profiler.

**Which tool lets you profile your battery usage?**

Batterystats, is a tool included in the Android Framework that collects battery data on your device.

**What options does the Hierarchy Viewer give you?**

The Hierarchy Viewer allows you to measure the layout speed for each view in your layout hierarchy, so you can find performance bottlenecks caused by the structure of your view hierarchy.

**Which version of Android Studio lets you add Kotlin code?**

Android Studio 3 and higher.

**What is an Android library compiled into?**

An Android library compiles into an Android Archive (AAR) file that you can use as a dependency for an Android App module.

**Why do you need to set up Continuous integration for your app?**

Continuous integration systems let you automatically build and test your app every time you check in updates to your source control system.

**Android Studio supports three types of code completion. Which are they?**

Basic, Smart, and Statement completion.

**What is Basic completion?**

Basic completion displays basic suggestions for variables, types, methods, expressions, and so on. If you call basic completion twice in a row, you see more results, including private members and non-imported static members.

**What is Smart Completion?**

Smart completion displays relevant options based on context. Smart Completion is aware of the expected type and data flows. If you call Smart Completion twice in a row, you see more results, including chains.

**What is Statement Completion?**

Statement Completion completes the current statement for you, adding missing parentheses, brackets, braces, formatting, etc.

**What is lint?**

Lint is a code scanning tool that can help you to identify and correct problems with the structural quality of your code without having to execute the app or write test cases.


**What is the Asset Studio tool used for?**

The Asset Studio tool helps you generate your own app icons from material icons, custom images, and text strings. It generates a set of icons at the appropriate resolution for each generalized screen density that your app supports.

**Android Studio can convert PNG, JPG, BMP, or static GIF images to WebP format. What is the WebP format?**

WebP is an image file from Google that provides lossy compression (like JPEG) as well as transparency (like PNG) but can provide better compression than either JPEG or PNG.

**How can you localize the UI of your app?**

The Translations Editor provides a consolidated and editable view of all of your default translated app texts, so that you can view, manage, and localize all of your string resources in one place.

**How can you make your app content searchable by Google?**

You can use Android App Links - HTTP URLS that bring users directly to specific content in your Android App.

## **The Manifest File**

**How many manifests can an application have?**

An application can only have one manifest file. However, there is an exception in the case that a 3rd party library is added. In this case the library has a manifest file as well.

**Why is the package name of the application important?**

The package name serves as a unique identifier of the application.

**What are some of the components of the application that are identified in the manifest?**

Activities, services, broadcast receivers, and content providers.

**Why do certain permissions need to be defined in the app's manifest?**

By default, no application is allowed to perform any operations that would adversely impact other applications, the operating system, or the user. For example, reading or writing the user's private data, reading or writing another application's files, performing network access, keeping the device and so on. The permission allows access to the protected parts of the API. It also allows the application to interact with other applications.

**What are some permissions that may be included in the manifest file?**

INTERNET, READ_LOGS, CALL_EMERGENCY_NUMBERS, SET_WALLPAPER, DEVICE_POWER.

**What can be contained within the activity tag in the app's manifest?**

Information about: activities, services, receivers, providers, and used libraries.

**What are the 2 required elements within the manifest's declaration?**

Manifest and application elements.

## **Gradle**

**Does Android Studio have an integrated build system?**

No. Android Studio delegates the entire build process to Gradle. Gradle turns all your sources and resources into APK files that you can install on your device.

**Why is it not necessary to additionally install Gradle when creating an Android project?**

It is not necessary to additionally install Gradle because Android Studio provides the Gradle runtime, and the Gradle scripts are automatically created.

**What is the main purpose of the Gradle wrapper for Android Studio?**

The Gradle wrapper is responsible to the Gradle version used to build your project. The version of Gradle could be specified in the configuration file called gradle-wrapper.properties
  
**What can you run Gradle task in Android Studio?**

There are two different ways: 1. from the terminal. 2. from the Gradle pane on the right of the window.

**What is the difference between the debug and the release version of your app?**

The debug version is used for testing, whereas the release version is used for the Google Play Store.

**Give examples for product flavors that can be defined in the productFlavors script block of your app's build.gradle file**

Typical product flavors are paid and free versions of your app.

**How many build.grade do you have in a blank-generated Androi project?**

There are 2. One top-level gradle file that usually contains common configs for all modules and one on a module level (the app module, by default). This is the build file of your specific module.

**If you want to us the Retrofit library in your project, in which section of the app's build.gradle file do you need to define it?**

Any dependencies need to be defined in the dependencies block of the build.gradle file.

**Gradle is a DSL. What is a DSL?**

DSL stands for Domain Specific Language. DSL is a language that is written to deal with a specific domain or set of concerns (SQL, XML, HTML).

**Gradle is a DSL that is written on top of what languages?**

Groovy and Java.

**If you want to do customization in your gradle build file, what language do you use?**

The build file supports Groovy syntax.

## **Intents**

**What is an intent?**

An intent is an object you can use to request an action from another app component (such as Activities, Services, Broadcast Receives, and Content Providers).

**In which general cases can you use intents?**

You can use an intent when you want to start an Activity, when you want to start a service, or deliver a broadcast.

**What is the difference between an implicit and explicit intent?**

When you ask a specific component from within the app by name (explicitly), you use an explicit intent (example: starting a ne Activity). When an action is asked from another app, you don't specify it by name, so you use an implicit intent (example: loading a webpage via the Uri object or loading the Camera).

**What kind of information can be contained within an intent?**

The name of the component to start (if explicit). A string that specifies the general action to be performed. The URI that references the data to be edited, loaded and so on. A string with the category of the kind of component that should handle the intent (launcher/browsable). Extras with additional information which can be transfered from one intent to another. Additional flags with extra instructions to the Android system.

**What happens when there is more than one app that responds to your implicit intent?**

The user can select which app to use and the user may make that app the default choice for the action (always SEND via an email) or a chooser dialog can be shown for the user to specify their choice everytime of which app should be used.

**What is the intent-filter element?**

The intent-filter element is an expression in the app's manifest file that specifies the type of intents the component would like to receive. Each intent-filter specifies the type of intents it accepts based on the intent's action, data, and category.

**What is a pending intent?**

A pending intent is an object that wraps another intent. It can also be used as a token that you give to a foreign application which allows the foreign application to use you application's permissions. By giving a PendingIntent to another application, you grant it the right to perform the operation you have specified as if the other application was you initial application.

**What is meant by intent resolution?**

The handling of the implicit intent when an implicit intent to start an activity is received, the system searches for the best activity for the intent, by checking the action, the data, and the intent category. The whole process of checking is called intent resolution.

**What is sticky intent?**

A sticky intent sticks with Android for future broadcast listeners. For example, If BATTERY_LOW occurs, the intent sticks to Android. If the BATTERY_LOW occurs one more time, the intent will be triggerred.

## **Activities**

**What is an activity in an Android Application?**

An activity is an application component which is visualized in a separate screen. Usually, an application consists of several activities.

**Can you explain the "last in, first out" stack mechanism in the context of activities?**

In an application, each activity can start another activity. When the new activity is started, the old activity is stopped but is also preserved by the system so that when the user presses the back button, the LAST activity that was visible is the FIRST to appear again.

**What is the difference between startActivity() and startActivityForResult()?**

In the case of startActivityForResult() you expect something to be returned from the started activity. In order for something to be received, we need to implement the onActivityResult() callback method.

**In which phase of the Activity's lifecycle should the global state be declared (as the layout, for example)?**

