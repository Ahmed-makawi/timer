# Stopwatch - Android App with Jetpack Compose

A simple stopwatch application with jetpack compose using foreground and bound services 




<img src= "https://github.com/Ahmed-makawi/timer/assets/119809534/c7dc0db8-f463-404b-9f5d-3f675bfb7374" alt="photo_2023-11-20_00-38-11.gif" width="300" hight="400">
<img src="https://github.com/Ahmed-makawi/timer/assets/119809534/6ff25f98-a1d9-42ad-ba1a-58eeba998ecc" alt="WhatsApp Image 2023-11-24 at 12 30 52_8f4f198c" width="300">



This application basically consists of 3 different textunits representing Hours, Minutes and Seconds.
Also we got two buttons on the UI. The first button will be changed on the basis of service state and the second button will allow us to cancel the foreground service which will result in resetting of our stopwatch.

You can control the stopwatch either by the UI buttons or with the notification panel. As we are using services, so if we even close the application then also we can track the stopwatch state by notification panel. 

## This project uses: 

* Dagger-Hilt
* Bound Service
* Foreground Service 

### Dagger-Hilt 

Hilt is a dependency injection library for Android that reduces the boilerplate of doing manual dependency injection in your project. Doing manual dependency injection requires you to construct every class and its dependencies by hand, and to use containers to reuse and manage dependencies.

Hilt provides a standard way to use DI in your application by providing containers for every Android class in your project and managing their lifecycles automatically. Hilt is built on top of the popular DI library Dagger to benefit from the compile-time correctness, runtime performance, scalability, and Android Studio support that Dagger provides. 

### Bound Service 

A bound service is an implementation of the Service class that allows other applications to bind to it and interact with it. To provide binding for a service, you must implement the onBind() callback method. This method returns an IBinder object that defines the programming interface that clients can use to interact with the service.

### Foreground Service 

Foreground services perform operations that are noticeable to the user.

Foreground services show a status bar notification, so that users are actively aware that your app is performing a task in the foreground and is consuming system resources.

Devices that run Android 12 (API level 31) or higher provide a streamlined experience for short-running foreground services. On these devices, the system waits 10 seconds before showing the notification associated with a foreground service. There are a few exceptions; several types of services always display a notification immediately.
