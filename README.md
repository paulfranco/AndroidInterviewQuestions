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

**What is Armv7?**

There are 3 CPU architectures in Android. ARMv7 is the most common as it is optimised for battery consumption. ARM64 is an evolved version of that which supports 64-bit processing for more powerful computing. ARMx86, is the least used for these three, since it is not battery friendly. It is more powerful than the other two.

**Why bytecode cannot be run in Android?**

Android uses DVM (Dalvik Virtual Machine ) rather using JVM(Java Virtual Machine).

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

The essential components of the activity need to be initialized in the onCreate() callback. We define the layout withing the setContentView().

**What are the phases of an Activity's lifecyscle?**

onCreate(), onStart(), onRestart(), onResume(), onPause(), onStop(), and onDestroy().

**Between which calls does the entire cycle of the Activity happen?**

The entire cycle of the Activity happens between onCreate(), where the resources are created, and onDestroy() where the resources are released.

**Between which calls can the user see and interact with the activity?**

The user can see and interact with the activity between onStart(), which is the visible phase afte the activity has been created and onStop() when a new activity is started.

**How can a destroyed activitiy's state be saved?**

We can achieve this within the onSavedInstanceState() where we can use a Bundle to store certain information.

**If nothing is specified, what happens when some of the device's configurations are changed at runtime?**

In the event that the screen orientation is changed the activity is recreated. onDestroy() is called followed by onCreate(). A way to handle this is by including the configChanges attribute to the certain activity.

**Which method is called to shut down an activity?**

There are 2 methods that may be called: finish() which is called to finish the activity itself, and finishActivity() to allow others to kill the activity.

**What is seamlessness? How is it applicable in Android?**

Seamlessness refers to non-interrupted flow of the application. It is up to the developer to handle all possible hinderances for the user, like low battery, configuration changes, and permissions needed.

## **Fragments**

**What are Fragments?**

Fragments are two or more activitives on the screen at the same time. Fragments have their own layout. Fragments can be added/removed from the Activity at run time. Fragments have their own lifecycle which are dependent of the Activity's lifecycle. Fragments must be embedded in an Activity. Fragments can be re-used in multiple activities.

**What is the difference between DialogFragment, ListFragment, and PreferenceFragment?**

All of them are subclasses that extend the basic Fragment class. PreferenceFragment displays a hierarchy of Preference objects as a list. ListFragment displays a list of item that are managed by an adapter. DialogFragment displays a floating dialog.

**Which is the interface for interacting with Fragment objects inside of an Activity?**

Fragment Manager.

**What is Fragment Transaction?**

The ability to add, romove, replace, and perform other actions with fragments on user's interaction. Each of these changes is called a transaction. In order to achieve it, you need the API's in FragmentTransaction.

**Can the fragment be accessed with the Activity it is in?**

Yes. You can access the fragment using getActivity().

**Which are the states in which a fragment can exist?**

Resumed, Paused, and Stopped.

**What is the difference between a fragment and an activity in terms of their lifecycle?**

The difference between a fragment and an activity is the way they are stored in the back stack. By default, the Activity is added at the top of the back stack, in order to be able to be called by the user on back press. If we want the same behavior by the fragment, we need to explicitly call addToBackStack().

**Is there a correlation between the activity's and the fragment's lifecycle?**

Yes. Each lifecysle callback for the activity results in a similar callback for each fragment.

**In comparison to an activity, are there additional lifecysle callbacks for the fragment? If so, what shich are they?**

Yes. They are onAttach(), onCreateView(), onActivityCreated(), onDestroyView(), and onDetach().

## **Services**

**What is a Service?**

A Service is a component of the application that lets you handle long-term operations in the background. A Service does not have a user interface. A Service is NOT a thread, and does not run on a separate thread. Services are Android Framework Components meant for running background tasks that don't need a visual component.

**Which are the basic forms a service takes?**

The basic forms a service takes are started and bound. Started wthin an activity, for example, via startService(). A service may continue running even after the component it started from is destroyed. Bound allows application components to bind to it. The bound service is dependent of the component it is in.

**How long does a bound service run for?**

A bound service runs for as long as there is a component bound to it.

**Should a service be declared in order to be used?**

Yes, in the manifest, within the service element, a child of application.

**What is the difference between stopSelf() and stopService() in a service's context?**

stopSelf() is called by the service itself when the job it was created for is done. stopService() is called by another component, in order to to stop the service.

**Does the service run in a thread separated from the UI?**

No, by default it runs in the main thread of that application.

**When a service is created, why is it better to extend IntentService rather than Service?**

Because IntentService creates a default worker thread that executes all the intents, whereas in the Service you create a new thread in which to do all the services' work slowing the work done in the main thread.

## **Broadcast Receivers**

**What is a Brodacast Receiver?**

A Broadcast Receiver is an Android component which allows yo to register for system or application events. All registered receivers for an event are notified by the Android runtime once this event happens.

**What is an implicit broadcast?**

An implicit broadcast is a trigger that declares an event instead of calling a specific app. This causes memory-thrashing.

**What is a system broadcast?**

A system . broadcast is a broadcast sent automatically to all apps thats are subscribed to receive the event.

**How do you register a receiver?**

You register a receiver with Static Registration in the manifest file and you can also do it with Dynamic Registration  wia the Context.registerReceiver() method.

**Which method is called by the Android System id the event for which the broadcast receiver has registered happens?**

The onReceive() methos is called.

**How can you perform a broadcast via a pending intent?**

You need to get a PendingIntent via the getBroadcst() method of the PendingIntent class.

**Which object wraps the broadcast message?**

The message is wrapped by the Intent object.

**How can you restrict a broadcast?**

You can restrict a broadcast with a permission. You can enforce restrictions on either the sender or the receiver of a broadcast.

**Is it a good idea to broadcast sensitive information using an implicit intent?**

No. Information broadcasted using an implicit intent can be read by any app that registers to receive the broadcast.

**Is it a good idea to start activities from broadcast receivers?**

No, because in such way the user experience is jarring, specially if there is more than one receiver. It is better to display a notification.

## **Content Providers**

**What does a Content Provider manage?**

Access to data.

**How is is the data in a relational database presented?**

In rows (each row is an instance of some type of data the provider collects) and columns (each column in the row represents an individual piece of data collected for an instance).

**Which application layer does a content provider coordinate access to?**

To the data layer of your application.

**Which object in your application' context is used when you want to access data in a content provider?**

The ContentResoluver object.

**How is data identified in a provider?**

With a content URI (Uniform Resource Identifier).

**What kind of permissions does your application need in order to retrieve data from the provider?**

Your application needs read access permission.

**Which object contains the columns specified by the query's projection for the rows that match the query's selection criteria?**

The Cursor object returned from the ContentResolver.query() client method.

**When is batch access to a provider useful?**

It is useful for inserting a large number of rows, or for inserting rows in multiple tables in the same method call.

**Where are the URI permissions defined?**

In the manifest, using the android.grantPermission attribute of the provider element.

**What is a class that defines constants which help applications work with content URIs, column names, intent actions, and other features of a content provider called?

Such a class is called a Contract Class.

**Which database is used by Android's own providers to store table-oriented data?**

The SQLite database API. The SQLiteOpenHelper class helpd you create databases, and the SQLiteDatabase class is the base class for accessing databases.

**What does the Storage Access Framework do?**

The SAF makes it simple for users to browse and open documents, images, and other files accross all of their preferred document storage providers.

## **Permanent Data Storage**

**Which are the ways to store data permanently in Android?**

Using Shared Preferences, Internal Storage, External Storage, SQLite Databases, and via Network Connection.

**What type of data can be saved via Shared Preferences?**

Primative data types (booleans, floats, ints, longs, and strings). The data is stored as key-value pairs. In order to use shared preferences, you have to call the method getSharedPreferences() which returns a SharedPreference intance.

**By default, what is the status of the files that are saved directly in the device's internal storage?**

By default these files are private to the application which means that other applications cannot access them. When the application is uninstalled, the file are removed as well.

**What is specific for the External Storage option?**

You need to acquire the respective permission (to be declared in the manifest). For example READ_EXTERNAL_STORAGE and WRITE_EXTERNAL_STORAGE (implicitly acquires the READ permission as well). Files can be stored on the SD card. Files can be stored in an internal (but not removable) storage. Before going for a particular media, you need to check if it is available. By default, the files can be accessed from other apps.

**What is the object that is always returned by an executed SQLite Query?**

A Cursor that points to all the rows found by the query.

**Can an SQLite database be debugged in Android?**

Yes. It can be debugged via an sqlite3 database tool.

## **Resources**

**Why do the resource need to be internalized?**

Alternative resource may be provided for different devices. They can be maintained independently, and different languages may be implemented.

**Where are the element's IDs stored?**

They are stored in the projects R class.

**Enumerate some of the sub-directories within the res directory**

Color, Drawable, Layout, Values, Raw, and Mipmap.

**What are 9 patch images?**

They are a stretchable bitmap image that are automatically resized to fit the contents of the View. They are usually used for the background of Buttons.

**What alternative resources can be provided for the screen orientation?**

Port: when the device is in portrait orientation. Land: when the device is in landscape orientation.

**What is an alias resource?**

This is the case when we have a resource we wanto use for more than one device configuration and at the same time not to set it as a default one. An alias of an existing drawable file is created via the <bimap> element. An alias of an existing layout file via the <merge> element.
  
**What is the R class in your application?**

It is generated by the aapt tool once the application is compiled. Here are generated IDs for all of the defined reources withinthe res/ directory. For each type of resource there is a subclass in the R file: R.drawable, R.values, R.mipmap.
For each resource of the particular type is stored a static integer - the unique ID of the resource in question.

**How can a resource be accessed?**

In the class's code, using the R-reference: R.string.appname. In the xml file with a different syntax: "@string/appname"

**When dealing with multiple resources, which one takes precedence?**

the 'local" qualifier almost always takes the highest precedence.

## **Layouts**

**How can a layout be declared?**

A layout can be declared in the xml file or programmatically at runtime.

**How many root elements can an xml file have?**

Only one. The type must be other View or ViewGroup object.

**What do the at- symbol and the plus sign mean in the element's ID declaration?**

Example: android:id="@+id/btnNext". The at-symbol: The xml parse is indicated that an id string is defined. The plus-sign: "please add the new resource reference to the resource file".

**What is the difference between Margin and Padding?**

Margin is the space left between the elements. Padding is the space between the content and the outside border.

**How should a layout whose content is dynamic be built?**

The layout can be populated with view at runtime, using an Adapter. The Adapter binds data to the view.

**What is a ViewGroup?**

A ViewGroup is the base class for Layouts. It can be defined as an invisible container. It holds Views and ViewGroups. Example: RelativeLayout is the ViewGroup that contains Button(which are Views), and other Layouts.

**How are the children within the Linear Layout aligned?**

All of them are defined and located in a single direction. The direction can either be Vertical or Horizontal. The oriantation can be set via the "orientation" attribute.

**What is the purpose of the layout weight attribute?**

It specifies how much of the extra space in the layout to be allocated to the View. It assigns an "importance" value to a view. Example: Space assigned to child = (child's individual weight)/(sum of weight of every child in Linear Layout)

**What is the default position of the children within the RelativeLayout?**

Top-Left of the layout.

**How are the elements visualized within a List View?**

The List View elements look like a list of scrollable elements. The design of each row is achieved via the implementation of an adapter.

**What is the difference between a ListView and a RecyclerView?**

The RecyclerView is described as an advanced ListView. As a matter of usage, the RecyclerView implementation is easier tp be achieved. For example: The ViewHolder is the default behavior of the RecyclerView. The items from the list can be easily contolled at runtime (with LayoutManager). The ItemAnimator holds the set of options for adding effects to each of the list items.

**How are the elements visualized within a GridView?**

Here the elements are within a 2-dimensional scrollable grid (as the default way icons are located on the start screen of any device). Most often it is used when we want to build an application as image viewer, ausio or video player.

**What is an Adapter?**

It helps data be transmitted and visualized within a view. Example: ListAdapter defines the layout for individual row of the list and provides data to the ListView via setAdapter() method of the ListView.

## **Input Controls**

**What can a button consist of?**

Text, Icon, or Text and Icon.

**What is the alternative of android:onClick attribute?**

The alternative is to set an OnClickListener programmatically. 

**How can you make a borderless button?**

In the xml of the control when adding style="?android:attr/borderlessButtonStyle".

**If you want to store the user's input in a field, what type of Input Control is used?**

EditText

**How can the data entered in the EditText be restricted and required?**

When specifying the android:inputType, we predefine what keyboard can be used by the user.

**How can the user be provided with input auto complete suggestions?**

We can use AutoCompleteTextView which is a subclass of EditText. The suggestions we want to be visualized need to be defined in a string array as different items. Then we need to set the adapter matching each line of the string array with a line in the field.

**What is the difference in the visualization between the Radio Buttons and the Spinner?**

The Radio Buttons shows options one to another. The Spinner shows the options one under another.

**What is the Toggle Button usually used for?**

The Toggle Button is usually used to provide the user with an option to set a particualar setting ON or OFF.

**When are pickers typically used?**

In the context of dates - when the user is provided with the opportunity to choose a particular time or date.

## **Menu, Settings, Dialogs**

**What collection holds the menu items for an activity?**

The options menu.

**How are the different menu items stored?**

As different item elements within the menu element.

**What is the Options Menu used for?**

Here we can add actions and other options that are relevant to the current activity context (For Example: search, share, star).

**What is a contextual menu?**

The actions specified within the Contextual Menu are connected to specific items, no to the whole activity.

**What is a popup menu?**

It is a type of Menu that appears below the clicked/hovered element (when there is enough space) or above it (when there isn't enough space).

**What object is used in order to specify a particular setting to the User?**

The Preference object.

**What is a dialog?**

A dialog is a small window that prompts the user to make a decision (yes/no) or enter additional information (example: set time).

**How many buttons can be added in an Alert Dialog?**

Up to 3.

**How are the buttons in the Alert Dialog ordered?**

Positive, Neutral, Negative.

**What dialog boxes are supported in Android?**

Alert Dialog, Progress Dialog, Date Picker Dialog, and the Time Picker Dialog.

## **Threads**

**Describe the "Main" thread**

The Main thread is created when the application is launched and is usually referred to as the UI thread. All components, running in the same process, are instantiated in the UI thread. The Android Ui toolkit may be accessed only from the Main thread.

**When may the UI thread be blocked?**

When all of the processes in an application happen on one thread or when long operations are performed on the UI thread (example: DB queries and Network access).

**What are the "Background" or "Worker" threads?

They are extra threads, different from the UI thread, wheere time-consuming operations can be ran.

**How can you start a new thread?**

You can start a new thread by creating a new instance of Runable or using AsyncTask.

**How does AsyncTask work?**

It is defined by a computation that runs on a background thread. Its result is published on the UI thread.

**How is AsyncTask defined?**

Via 3 types: Params - what is going to be sent when the execution is started. Progress - the way the progress is to be stored during the execution. Result - the result expected from the whole computation itself.

**Which phases does an execution go through when implementing AsyncTask?**

onPreExecute(), doInBackground(params...), onProgressUpdate(Progress...), onPostExecute(Result).

## **Notifications and Search Interface**

**What is a notification?**

A notification is a message that appears on the User's screen. It is not part of the basic UI design of the application. The issued notification appears first in the notification area and when it is chosen it goes to the notification drawer.

**What are the obligatory parts that each notification object should have?**

A small icon, a title, and a detailed text.

**How many actions should be added to a notification?**

At least one, in order for the user to be redirected to the corresponsing activity.

**Can you control how a set of notifications are going to be shown?**

Yes, you can control them by adding priority.

**What are the options to add a search input in the app?**

You can add a serach input in the app by adding a search dialog at the top of the screen or by adding a search widget.

**How can you grant the user the opportunity to search the app's data?**

This feature is not supported by the search framework. However, there are specific ways for the different types of data APIs. For example: if we have an SQLite DB, the android.database.sqlite APIs should be used. 

## **Other**

**What are the different Android Components?**

Activities, Intents, Services, Broadcast Receivers, and Content Providers.

**What is a Toast in Android?**

Android Toast can be used to display information for the short period of time. A toast contains message to be displayed quickly and disappears after sometime.

**What is an Executor?**

An Executor is an object that executes submitted Runnable tasks. This interface provides a way of decoupling task submission from the mechanics of how each task will be run, including details of thread use, scheduling, etc. 

**When is an Executor normalll used?**

Ab executor is normally used instead of explicitly creating threads.

