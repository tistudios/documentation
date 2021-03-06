**<span class="label label-release label-version">Creo 1.2.2</span>December 12th 2018 (Build 15618)**
* Added cubeSQL support
* Added isCreoKit, isCreoPlayer and isRealDevice to Device class
* Improved readString method in FileManager class
* Fix a crash that occurred with a NULL font 
* Fixed random issue with registered creo versions not correctly recognized
* Fixed ipa builder
* Several fixes related to TableView
* Several fixes related to TabBar
* Updated Gravity to the latest version
* A lot of other internal fixes and improvements
* **[CreoPlayer 1.2.7](https://creolabs.com/creoplayer)** is required and it should be available via TestFlight within the next 48 hours

**<span class="label label-release label-version">Creo 1.2.0</span>November 23th 2018 (Build 15544)**
* Exposed a lot of new properties and methods to Camera control
* Extended Camera control with barcode scanning capabilities
* Extended CameraRoll (it can now save metadata)
* Extended Crypto class with base64 encoding methods
* Added IP address methods to NetworkReachability class
* Improved autocompletion for some classes
* Exposed new events to all UI controls: WillShow, DidShow, WillHide, DidHide
* Added a second ndigits precision parameter to the Math.round method
* Fixed an old issue with the TextField in secure mode
* Fixed a Mojave specific issue that affects the Font class
* Several issues fixed related to Undo/Redo
* Several issue fixed in the HTTPServer class
* A lot of other internal fixes and improvements
* An updated **[CreoPlayer](https://creolabs.com/creoplayer)** app should be available via TestFlight within the next 48 hours

**<span class="label label-release label-version">Creo 1.1.8</span>October 29th 2018 (Build 15378)**
* Improved error reporting on App building panel
* Improved Math.random
* Improved NavigationBar emulation
* Improved Toolbar and BarButtons
* Extended RecordSet with intValue, int64Value, floatValue, doubleValue and boolValue
* Exposed lensAperture to Camera
* Exposed a new valueForIndex method to DataSet
* Exposed TimeZone class
* Added DidSelectAnnotation/DidDeselectAnnotation events to MapView
* Exposed ShouldChangeText event to TextField (see )
* Query editor is now able to succesfully execute non select statements
* TableView dataSet can now be set to null
* Fixed a FileManager issue
* Fixed a Map annotation issue
* Fixed a HTTPRequest issue
* Several issues fixed in Gesture objects
* New general Creo documentation available on **[https://docs.creolabs.com/creo](https://docs.creolabs.com/creo)**
* A lot of other internal fixes and improvements
* An updated **[CreoPlayer](https://creolabs.com/creoplayer)** app should be available via TestFlight within the next 48 hours

**<span class="label label-release label-version">Creo 1.1.7</span>October 9th 2018 (Build 15242)**
* Several UI fixes for 10.14 Mojave
* Improved TableView
* Improved Label, TextField and TextView
* Improved SQLite support
* Navigation has been renamed to NavigationBar
* A lot of other internal fixes and improvements
* An updated **[CreoPlayer](https://creolabs.com/creoplayer)** app should be available via TestFlight within the next 48 hours

**<span class="label label-release label-version">Creo 1.1.6</span>September 26th 2018 (Build 15134)**
* Improved error reporting
* Improved DataSet selection from Inspectors
* Improved HTTPClient JSON handling
* Improved PageContainer
* Improved InputView support
* Added support for new iPhone XR/XS/XS Max devices
* Added support for custom url in Application
* Fixed a potential crash bug introduced in 1.1.5 version
* Fixed some potential issue due to race conditions
* A lot of other internal fixes and improvements
* An updated **[CreoPlayer](https://creolabs.com/creoplayer)** app should be available via TestFlight within the next 48 hours

**<span class="label label-release label-version">Creo 1.1.5</span>September 19th 2018 (Build 15032)**
* Added Search panel
* Greatly improved compiler and runtime error reporting
* SQLite databases can now be automatically copied on a read-write directory on real iOS devices
* Added a new Advanced preference to control message sent to NULL behaviours
* Application events are now correctly raised within the Simulator
* Console.write on a real device now log directly to system log
* Added the ability to schedule local notifications
* Added the NetworkReachability class to check the network status
* Added Device.vibrate() method
* Fixed an issue with Large Title in NavigationBar
* Fixed an issue with WebView
* Fixed minor issues with TableView header and footer
* A lot of other internal fixes and improvements
* An updated **[CreoPlayer](https://creolabs.com/creoplayer)** app should be available via TestFlight within the next 48 hours

**<span class="label label-release label-version">Creo 1.1.1</span>September 10th 2018 (Build 14655)**
* Fixed several ScrollView issues (introduced in the 1.1.0 version). These issues affect several controls like PickerView, DatePicker and TableView.
* Increased compatibility with the upcoming MacOS 10.14 Mojave release.

**<span class="label label-release label-version">Creo 1.1.0</span>September 7th 2018 (Build 14633)**
* Added support for Safe Area (with preview)
* Added new DatabaseRecord class
* Added Toolbar item subnodes to NavigationBar
* New inspectors for all objects
* New subnodes added to several controls
* Improved Simulator performance
* Several fixes and enhancements to ScrollView
* Several fixes to PickerView
* Several fixes to SQLite database built-in inspector
* Several fixes to TableView
* Fix for SystemButton in iPhone X
* Fix for BezierPath image method
* Fix for RefreshControl position in NavigationBar
* Tons of others internal fixes and improvements
* **[CreoPlayer](https://creolabs.com/creoplayer)** has been updated and it is now available through the TestFlight program

**<span class="label label-release label-version">Creo 1.0.8</span>July 31st 2018 (Build 14201)**
* Improved NavigationBar class with new blur layer and others internal improvements
* Improved Window class with exposed firstResponder and new methods to convert from/to the Window's view coordinate system
* Improved TableView
* Improved Open/OpenIn/OpenModal methods
* Improved ChartView
* Improved Map with new Annotations related methods and properties
* Improved performance for large projects
* Added an optional closure parameter to the Open method (that will be executed by the newly opened Window/Navigation)
* Exposed autoresizingMask property to all UIView subclasses
* Fixed an issue with ExposedEvents
* Fixed an issue with Image class
* Others internal improvements and fixes
* New documentation engine at **[https://docs.creolabs.com/](https://docs.creolabs.com/)**. Users can submit examples, articles or any other improvement via our new public **[GitHub](https://github.com/creoapp/documentation/)** repo.

**<span class="label label-release label-version">Creo 1.0.7</span>July 19th 2018 (Build 14057)**
* Improved WebView
* Improved String.split method and added new String.replace and String.contains methods
* Exposed idleTimerDisabled Boolean flag to App instance
* Improved TextField and SearchBar
* Added Map annotation basic implementation
* Improved syntax error line recognition
* Fixed colorBorder property
* Various fixes and improvements to PageScroll and PageCurl
* Various fixes and improvements to TabBar and NavigationBar
* Added a workaround for iPad multitasking not yet supported
* Improved iOS app build process
* Various fixes and improvements to TableView
* Exposed new Application type setting
* Various fixes and improvements to the Property List editor
* Fix for Exposed Events
* Others internal improvements

**<span class="label label-release label-version">Creo 1.0.6</span>July 12th 2018 (Build 13963)**
* Fixed a crash with some combination characters in the code editor
* Added the ability to execute JavaScript from the WebView (and callback Gravity code)
* Added setFocus/clearFocus method  to controls
* Fixed Actions Inspector for non UI objects
* Added address property to MapView
* New useful properties added to Device and App objects
* Fixed an issue with mySQL TEXT field recognized as BLOB
* Fixed the status bar properties of the App object
* Various fixes and improvements to the HTTPClient Request class
* Fix for deleted gesture recognizer
* Others internal improvements

**<span class="label label-release label-version">Creo 1.0.5</span>July 6th 2018 (Build 13895)**
* Fixed an issue in generated apps with a registered Creo version
* Added format method to Date class (with an example in documentation)
* Improved autocompletion
* [Build your app](https://docs.creolabs.com/creo/build-your-app.html) tutorial has been updated with a new "Submit your app to the App Store" section and an "Apple Configurator 2" tutorial
* Others internal improvements

**<span class="label label-release label-version">Creo 1.0.4</span>July 5th 2018 (Build 13884)**
* Fixed an issue in Preferences.write method
* Fixed an issue with local html files and WebView
* Fixed an issue with Database.execute
* Fixed an issue with labelsColumn parameter of ChartView
* [Spotify](https://docs.creolabs.com/tutorials/spotify.html) tutorial has been updated
* Others internal improvements

**<span class="label label-release label-version">Creo 1.0.3</span>July 3rd 2018 (Build 13867)**
* **[CreoPlayer](https://creolabs.com/creoplayer)** is now available through the TestFlight program
* Added a new Properties and Privacy panel
* Added support for class properties and methods in custom classes
* Improved StatusBar support
* Exposed anchorPoint property in Inspector Geometry
* Fixed an issue with application builder and the Development Distribution target
* Fixed the default redirect callback url scheme for oAuth1 and oAuth2 in HTTPClient class. The new uri is **com.creolabs.creo://oauth2Callback**
* Several crashes has been fixed thanks to the feedback from our users
* Several others internal fixes and improvements

**<span class="label label-release label-version">Creo 1.0.2</span>June 21st 2018 (Build 13657)**
* Added TestFlight support
* Small improvements in the Animation panel
* Improved performance of ImageView control
* Fixed some issues related to iOS lower than 11.0
* Fixed a crash issue in the Action panel

**<span class="label label-release label-version">Creo 1.0.1</span>June 18th 2018 (Build 13630)**
* Fixed a crash that occurred when a gradient was saved in favourites
* Fixed a crash that can occurs when zoom factor in multi-screen environments was returned as zero
* Improved multi display support
* Fixed an issue in TabBar controller
* Added a new Advanced panel in Preferences to check if beta versions should be checked in in-app updates
* Custom subclasses now correctly expose events from super class (more work needs to be done)
* Added a workaround for a 10.14 issue (as a result the Font class cannot be directly used in 10.14)

**<span class="label label-release label-version">Creo 1.0.0</span>June 13th 2018 (Build 13600)**
* First official release
* **[CreoPlayer](https://creolabs.com/creoplayer)** version 1.1 or higher is now required
