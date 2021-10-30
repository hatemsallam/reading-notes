# Application Fundamentals

* Android apps can be written using Kotlin, Java, and C++ languages.
* The Android SDK tools compile the code along with any data and resource files into an APK or an Android App Bundle
* Android package :  is an archive file with an .apk suffix, contains the contents of an Android app that are required at runtime and it is the file that Android-powered devices use to install the app.
* Android App Bundle : is an archive file with an .aab suffix, contains the contents of an Android app project including some additional metadata that is not required at runtime.
* Each Android app lives in its own security sandbox

## Android security features

* The Android operating system is a multi-user Linux system in which each app is a different user.
* By default, the system assigns each app a unique Linux user ID .
* Each process has its own virtual machine (VM), so an app's code runs in isolation from other apps.
* By default, every app runs in its own Linux process.

## The principle of least privilege

* That is, each app, by default, has access only to the components that it requires to do its work and no more.
* This creates a very secure environment in which an app cannot access parts of the system for which it is not given permission.

## The ways for an app to share data with other apps

* It's possible to arrange for two apps to share the same Linux user ID in which case they are able to access each other's files.
* To conserve system resources, apps with the same user ID can also arrange to run in the same Linux process and share the same VM.
* An app can request permission to access device data such as the device's location, camera, and Bluetooth connection.

## App components

* App components are the essential building blocks of an Android app.
* Some components depend on others.
* There are four different types of app components:

1. Activities
2. Services
3. Broadcast receivers
4. Content providers

## Activities

* An activity is the entry point for interacting with the user.
* It represents a single screen with a user interface. 

### interactions between system and app:

* Keeping track of what the user currently cares about (what is on screen) to ensure that the system keeps running the process that is hosting the activity.
* Knowing that previously used processes contain things the user may return to (stopped activities), and thus more highly prioritize keeping those processes around.
* Helping the app handle having its process killed so the user can return to activities with their previous state restored.
* Providing a way for apps to implement user flows between each other, and for the system to coordinate these flows.

## Services

* A service is a general-purpose entry point for keeping an app running in the background for all kinds of reasons. 
* It is a component that runs in the background to perform long-running operations or to perform work for remote processes.
* A service does not provide a user interface.
* Bound services run because some other app (or the system) has said that it wants to make use of the service.
* This is basically the service providing an API to another process.

## Broadcast receivers

* A broadcast receiver is a component that enables the system to deliver events to the app outside of a regular user flow, allowing the app to respond to system-wide broadcast announcements .
* Because broadcast receivers are another well-defined entry into the app, the system can deliver broadcasts even to apps that aren't currently running. 

## Content providers

* A content provider manages a shared set of app data that you can store in the file system, in a SQLite database, on the web, or on any other persistent storage location that your app can access. 
* Content providers are also useful for reading and writing data that is private to your app and not shared.
* A unique aspect of the Android system design is that any app can start another app’s component.


### things that allows the system to do in managing an app:

* Assigning a URI doesn't require that the app remain running, so URIs can persist after their owning apps have exited. 
* These URIs also provide an important fine-grained security model.

## Activating components

* Three of the four component types—activities, services, and broadcast receivers—are activated by an asynchronous message called an intent.
* Intents bind individual components to each other at runtime.
* An intent is created with an Intent object
* For activities and services, an intent defines the action to perform .
* For broadcast receivers, the intent simply defines the announcement being broadcast.
* a broadcast to indicate the device battery is low includes only a known action string that indicates battery is low.

## There are separate methods for activating each type of component:

* You can start an activity or give it something new to do by passing an Intent to startActivity() or startActivityForResult()
* you can use the JobScheduler class to schedule actions. 
* earlier Android versions, you can start a service (or give new instructions to an ongoing service) by passing an Intent to startService(). You can bind to the service by passing an Intent to bindService().
* You can initiate a broadcast by passing an Intent to methods such as sendBroadcast(), sendOrderedBroadcast(), or sendStickyBroadcast().
* You can perform a query to a content provider by calling query() on a ContentResolver.

## The manifest file

* Before the Android system can start an app component, the system must know that the component exists by reading the app's manifest file, AndroidManifest.xml.
* The manifest does a number of things in addition to declaring the app's components, such as the following:

1. Identifies any user permissions the app requires, such as Internet access or read-access to the user's contacts.
2. Declares the minimum API Level required by the app, based on which APIs the app uses.
3. Declares hardware and software features used or required by the app, such as a camera, bluetooth services, or a multitouch screen.
4. Declares API libraries the app needs to be linked against (other than the Android framework APIs), such as the Google Maps library.

## App resources

* For every resource that you include in your Android project, the SDK build tools define a unique integer ID, which you can use to reference the resource from your app code or from other resources defined in XML
* One of the most important aspects of providing resources separate from your source code is the ability to provide alternative resources for different device configurations. 
* Android supports many different qualifiers for your alternative resources. 
* The qualifier is a short string that you include in the name of your resource directories in order to define the device configuration for which those resources should be used. 