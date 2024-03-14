# SampleCode_AcousticMobilePush_iOS_Swift

SampleCode_AcousticMobilePush_iOS_Swift is one of the sample iOS application that shows how to integrate [Acoustic-Mobile-Push SDK](https://github.com/go-acoustic/Acoustic-Mobile-Push-iOS) with any iOS Application.


## Getting Started for Cocoapods

### Prerequisites

You need to have recent cocoapods version install on your Mac OS. Current version is 1.4.0. Please refer to cocoapods website for the details.

For SDK prerequisites and documentation, please refer to the SDK documentation [here](https://developer.goacoustic.com/acoustic-campaign/docs/add-the-ios-sdk-to-your-app)

## Updating podfile

Open Podfile in a text editor of your choice and note the following lines in the Podfile.
```
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
 pod 'AcousticMobilePush'
 pod 'AcousticMobilePush'
 pod 'AcousticMobilePushNotification'
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
git clone https://github.com/go-acoustic/SampleCode_AcousticMobilePush_iOS_Swift.git
```

Open terminal window and go to the sample app location
```
cd SampleCode_AcousticMobilePush_iOS_Swift
```

Run the following command
```
pod install
```

Then follow the instructions on [build-mobile-app-messages-with-the-sample-app](https://developer.goacoustic.com/acoustic-campaign/docs/build-mobile-app-messages-with-the-sample-app)

# License

License files can be read [here](https://github.com/go-acoustic/Acoustic-Mobile-Push-iOS/blob/master/license/license.txt)

