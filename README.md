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


