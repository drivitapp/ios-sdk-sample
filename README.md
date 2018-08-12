<p align="center">
  <img height="250" src="logo.jpg" />
</p>

# Drivit

[![CocoaPods Compatible](https://img.shields.io/badge/pod-1.1.0-blue.svg)](https://img.shields.io/badge/pod-1.1.0-blue.svg) [![Platform](https://img.shields.io/badge/platform-ios-lightgrey.svg)](https://img.shields.io/badge/platform-ios-lightgrey.svg)

Meet Drivit, an SDK that helps you in your day-to-day activities while making you a better driver.

- [Features](#features)
- [Requirements](#requirements)
- [Installation](#installation)
- [Documentation](https://drivitapp.github.io/ios-sdk-sample/)
- [Usage](https://github.com/drivitapp/ios-sdk-sample/blob/master/USAGE.md)

## Features

- [x] Login

## Requirements

- iOS 10.0+
- Xcode 9.0+

Below is a table that shows which version of Drivit you should use for your Swift version.

Swift | Drivit   
:---- | -------- 
4.X   | >= 1.0.0

## Installation

### CocoaPods

[CocoaPods](https://cocoapods.org) is a dependency manager for Cocoa projects. You can install it with the following command:

```bash
$ gem install cocoapods
```

To integrate Drivit into your Xcode project using CocoaPods, specify it in your `Podfile`:

```ruby
source 'https://github.com/CocoaPods/Specs.git'
platform :ios, '10.0'
use_frameworks!

target '<Your Target Name>' do
    pod 'Drivit', '~> 1.1.0'
end
```

Then, run the following command:

```bash
$ pod install
```

### Manually

#### 1. Add the Drivit SDK framework to your app bundle

To get the Drivit SDK framework contact us at support@drivit.com.

#### 2. Add the dependencys needed for the Drivit SDK

If you are using carthage/cocoapods add "MagicalRecord" to your dependency tree. The framework should be in the embeded frameworks of the app.

#### 3. Make sure your project is running swift 4.0 or higher.

With these three steps, your app should be already compiling the Drivit SDK. Now let's put it to work

## License

Copyright (c) 2018 Bahub Business Analysis Systems, Lda. [See LICENSE](https://github.com/drivitapp/iOS-core/blob/master/LICENSE) for details.
