
# DrivitSDK-Sample

This is a sample project to demonstrate the Drivit iOS SDK integration. This document also outlines the key steps to integrate Drivit SDK into your application and put it to work.

## Get an API_KEY
To use the Drivit SDK you need an API Key. Contact us at support@drivit.com to get one. 

## Setup your XCode Project
### 1. Add the Drivit SDK framework to your app bundle

LINK TO THE FRAMEWORK

### 2. Add the dependencys needed for the Drivit SDK

If your using carthage/cocoapods add "MagicalRecord" to your dependency tree. The framework should be in the embeded frameworks of the app.

### 3. Make sure your project is running swift 4.0 or higher.

With these three steps, your app should be already compiling the Drivit SDK. Now let's put it to work

## Using the SDK
### 1. Add the the following methods to your app delegate.
Add the following code to your application(_ application: UIApplication, didFinishLaunchingWithOptions launchOptions: [UIApplicationLaunchOptionsKey: Any]?) -> Bool
```
Drivit.shared.applicationDidWakeWithOptions(launchOptions)
```
Next add the following code to application(_ application: UIApplication, handleEventsForBackgroundURLSession identifier: String, completionHandler: @escaping () -> Void)
```
Drivit.shared.applicationDiStartWithBackgroundSessionEvents(SessionIdentifier: identifier, completion: completionHandler)
```

### 2. Login/signup your user into the SDK
You have to login the user into the SDK before it starts recording trips. To do so, create an instance of the ```DIAuth``` object and provide it with the info of your user

```
let simple = DIAuth.regular(email: "email", password: "password")
OR
let advanced = DIAuth.advance(secret: "secret")
            
Drivit.shared.login(auth: simple) { result in                
        switch(result) {
        case .success(_): break
        case .error(_): break
}
```

### 3. To start recording a trip
After you login you can start a trip by running the following code:

```
Drivit.shared.forceTripStart()
```


And that is it! Safe trips!

**The Drivit Team**

<br/><br/>P.S. You can see the complete reference documentation [here](LINK)
