# SampleCode_AcousticMobilePush_iOS_Swift

SampleCode_AcousticMobilePush_iOS_Swift is one of the sample iOS application that shows how to integrate [Acoustic-Mobile-Push SDK](https://github.com/Acoustic-Mobile-Push/iOS) with any iOS Application.

## Getting Started for Carthage

### Prerequisites

You need to have recent carthage version install on your Mac OS. Current version is 0.36.0.[Please refer to carthage website for the details](https://github.com/Carthage/Carthage).

For SDK prerequisites and documentation, please refer to the SDK documentation [here](https://developer.goacoustic.com/acoustic-campaign/docs/add-the-ios-sdk-to-your-app)

## Updating Cartfile

Open Cartfile in a text editor of your choice and note the following lines:

In the respective targets for your project in the Podfile add the following line if you want to use AcousticMobilePush SDK's release version
```
binary "https://raw.githubusercontent.com/Acoustic-Mobile-Push/iOS/master/AcousticMobilePush.json" >= 3.8.18
binary "https://raw.githubusercontent.com/Acoustic-Mobile-Push/iOS/master/AcousticMobilePushNotification.json" >= 3.8.18
binary "https://raw.githubusercontent.com/Acoustic-Mobile-Push/iOS/master/AcousticMobilePushWatch.json" >= 3.8.18
```

In the respective targets for your project in the Podfile add the following line if you want to use AcousticMobilePush SDK's debug version
```
binary "https://raw.githubusercontent.com/Acoustic-Mobile-Push/iOS/master/AcousticMobilePushDebug.json" >= 3.8.18
binary "https://raw.githubusercontent.com/Acoustic-Mobile-Push/iOS/master/AcousticMobilePushNotificationDebug.json" >= 3.8.18
binary "https://raw.githubusercontent.com/Acoustic-Mobile-Push/iOS/master/AcousticMobilePushWatchDebug.json" >= 3.8.18
```

You will notice that by default the sample application uses `Debug` version of libraries.

Note that you can use only one of  `Release` or `Debug`. Do not use both at the same time.

Now you need to install the carthage by running the following command.
```
carthage update --use-xcframeworks
```

Above carthage command should complete with no errors.

## Run Sample Application

Clone the sample app code from github location

```
git clone https://github.com/Acoustic-Mobile-Push/SampleCode_AcousticMobilePush_iOS_Swift.git
```

Open terminal window and go to the sample app location
```
cd SampleCode_AcousticMobilePush_iOS_Swift
```

Run the following command
```
carthage update --use-xcframeworks
```

Then follow the instructions on [build-mobile-app-messages-with-the-sample-app](https://developer.goacoustic.com/acoustic-campaign/docs/build-mobile-app-messages-with-the-sample-app)

# License

License files can be read [here](https://github.com/acoustic-analytics/Tealeaf/tree/master/Licenses)

