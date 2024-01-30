# SampleCode_AcousticMobilePush_iOS_Swift

SampleCode_AcousticMobilePush_iOS_Swift is one of the sample iOS application that shows how to integrate [Acoustic-Mobile-Push SDK](https://github.com/Acoustic-Mobile-Push/iOS) with any iOS Application.

## Getting Started for Swift Package

### Prerequisites

You just need xcode.

For SDK prerequisites and documentation, please refer to the SDK documentation [here](https://developer.goacoustic.com/acoustic-campaign/docs/add-the-ios-sdk-to-your-app)

## Updating xcode project

Open Podfile in a text editor of your choice and note the following lines in the Podfile.
```
source 'https://github.com/Acoustic-Mobile-Push/iOS.git'
source 'https://github.com/CocoaPods/Specs.git'
```

Also note the platform in the Podfile iOS 12.1
```
platform :ios, '12.1'
```

Note that use_frameworks is uncommented for xcframeworks.
```
use_frameworks!
```

In the respective targets for your project in the Podfile add the following line if you want to use AcousticMobilePush SDK's release version
```
pod 'AcousticMobilePush'
pod 'AcousticMobilePushNotification'
```

If iWatch is used, add iwatch extension
```
pod 'AcousticMobilePushWatch'
```

In the respective targets for your project in the Podfile add the following line if you want to use AcousticMobilePush SDK's debug version
```
pod 'AcousticMobilePushDebug'
pod 'AcousticMobilePushNotificationDebug'
```

If iWatch is used, add iwatch extension
```
pod 'AcousticMobilePushWatchDebug'
```

You will notice that by default the sample application uses `pod 'AcousticMobilePushDebug'`,`pod 'AcousticMobilePushDebug'` and `pod 'AcousticMobilePushNotificationDebug'`

Note that you can use only one of 
```
 pod 'AcousticMobilePushDebug'
 pod 'AcousticMobilePushDebug'
 pod 'AcousticMobilePushNotificationDebug'
 ```
 
 or 
 ```
 pod 'AcousticMobilePushDebug'
 pod 'AcousticMobilePushDebug'
 pod 'AcousticMobilePushNotificationDebug'
 ```
 
Do not use both at the same time.

Now you need to install the pods by running one of the following commands.
```
pod install
```

or to update
```
pod update
```

Above pod command (install or update) should complete with no errors. If you do see errors run the same command with `--verbose` option and share the error log with us.

## Run Sample Application

Clone the sample app code from github location

```
git clone https://github.com/Acoustic-Mobile-Push/SampleCode_AcousticMobilePush_iOS_Swift.git
```

Then follow the instructions on [build-mobile-app-messages-with-the-sample-app](https://developer.goacoustic.com/acoustic-campaign/docs/build-mobile-app-messages-with-the-sample-app)

This project also uses Swift Package from https://github.com/Acoustic-Mobile-Push/AcousticMobilePushDebug-SP, https://github.com/Acoustic-Mobile-Push/AcousticMobilePushNotificationDebug-SP and https://github.com/Acoustic-Mobile-Push/AcousticMobilePushWatchDebug-SP which installs debug version of AcousticMobilePush swift packages.

# License

License files can be read [here](https://github.com/acoustic-analytics/Tealeaf/tree/master/Licenses)
