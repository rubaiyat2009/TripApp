# TripApp
This is a trip app with Xamarin.
To start, it is important to understand the requirements and features of the TripApp. 
We will do this by quickly defining some of the high-level things this app will allow its users to do:

View existing log entries (online and offline)
Add new log entries with the following data:
Title
Location using GPS
Date
Notes
Rating
Sign into the app

# To Create the initial app
To start off the new TripApp mobile app project, we will need to create the initial solution architecture. 
We can also create the core shell of our app’s user interface by creating the initial screens based on the basic features we have just defined.

# Outcome 

There will be a single portable class library project and two platform-specific projects, as follows:

TripApp: This is a portable class library project that will serve as the core layer of the solution architecture. This is the layer that will include all our business logic, data objects, Xamarin.Forms pages, and other non-platform-specific code. The code in this project is common and not specific to a platform, and can therefore, be shared across the platform projects.

TripApp.iOS: This is the iOS platform-specific project containing all the code and assets required to build and deploy the iOS app from this solution. By default, it will have a reference to the TripLog core project.

TripApp.Android: This is the Android platform-specific project containing all the code and assets required to build and deploy the Android app from this solution. By default, it will have a reference to the TripApp core project.

If you are using Visual Studio for Mac, you will only get an iOS and an Android project when you create a new Xamarin.Forms solution. To include a Windows (UWP) app in your Xamarin.Forms solution, you will need to use Visual Studio for Windows. 
