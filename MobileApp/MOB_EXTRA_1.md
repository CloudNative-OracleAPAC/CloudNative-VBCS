## 11. If You Have Extra Time

> In this lab you have run your app using the built-in mobile application simulator. You will have noticed that the **‘Build My App’** option was disabled

![alt text](../resources/images/mob/E1.png "Logo Title Text 1") 


Before you can build the app for installation on an iOS or Android device, you have to create a Build Configuration

## Android

### Keystpore for Signing app
Your mobile application must be signed before it can be deployed to an Android device. Android does not require a certificate authority; an application can instead be self-signed.

We have generated a sample keystore for you to use. Download the KeyStore file below.

Sample Keystore file:  <a href="resources/KSFile/vbcsdoc.keystore">vbcsdoc.keystore</a>

+ Keystore Password: **vbcsdoc_ks_pass**
+ Key alias: **vbcsdoc_ksalias**
+ Key password: **vbcsdoc_ks_pass**

### Configure Application Setting.
Once you've downloaded the KeyStore file, you're ready to configure the application settings.

![alt text](../resources/images/android/android1.png "Logo Title Text 1")
![alt text](../resources/images/android/android2.png "Logo Title Text 1")
![alt text](../resources/images/android/android3.png "Logo Title Text 1")
![alt text](../resources/images/android/android4.png "Logo Title Text 1")

### Define a Build Configuration

![alt text](../resources/images/android/android5.png "Logo Title Text 1")
![alt text](../resources/images/android/android6.png "Logo Title Text 1")
![alt text](../resources/images/android/android7.png "Logo Title Text 1")
![alt text](../resources/images/android/android8.png "Logo Title Text 1")
![alt text](../resources/images/android/android9.png "Logo Title Text 1")
![alt text](../resources/images/android/android10.png "Logo Title Text 1")
![alt text](../resources/images/android/android11.png "Logo Title Text 1")

### Build the Mobile Application

![alt text](../resources/images/android/android12.png "Logo Title Text 1")
![alt text](../resources/images/adroid/android13.png "Logo Title Text 1")
![alt text](../resources/images/android/android14.png "Logo Title Text 1")
![alt text](../resources/images/android/android15.png "Logo Title Text 1")


## iOS
Below is an example of how to setup and build an iOS version of your mobile app.  The lab does not provide the elements for you to complete this setup

Click on the **`Settings`** icon for your mobile app and click on the Build Configurations tab

![alt text](../resources/images/mob/E2.png "Logo Title Text 1")
 
Click **`New Configuration`**.

To follow this example, click on iOS, but if you are more familiar with Android, go there too

![alt text](../resources/images/mob/E3.png "Logo Title Text 1") 

The configuration settings on the left side are defaulted by VBCS, but can all be edited to suit your needs

On the right side you must add your Apple Developer program credentials – whether an Enterprise or Standard program, developer of distribution profile etc.

> Note: it is outside the scope of this lab to provide instruction on how to get an Apple Developer Program account, go to developer.apple.com for more details

Add your provisioning profile, certificate and certificate password details to the configuration. Ensure that the Signing Identity is exactly as shown in your Keychain entry for the certificate. To ensure this, use Get Info in keychain and copy the complete entry from the Common Name property

If you want to use this profile as the default build when you ask VBCS to build your mobile app, click on the appropriate checkboxes (bottom right)

![alt text](../resources/images/mob/E4.png "Logo Title Text 1") 

Now the Build My App button on your simulator running app will be enabled.

Clicking on it takes you to Stage Application. Here you can select how the business data should be deployed:

If this is a first Stage deployment you may want to take the development data into the app, or start with a clean database. For subsequent deployments you may want to keep any data that was in the previously staged version, start from clean or start from the development data again.

![alt text](../resources/images/mob/E5.png "Logo Title Text 1")

Once you hit the Stage button (above) the Mobile application is staged and, as it says on the screen, you can scan to install on your device (via the QR scan or by downloading the .ipa file) and start the next stage of your development process

![alt text](../resources/images/mob/E6.png "Logo Title Text 1")

## Congratulations you have completed your myTravel Mobile App using VBCS!

---
> [`HOME`](../README.md) | [`PART 1`](MOB_PART_1.md) | [`PART 2`](MOB_PART_2.md) | [`EXTRA`](MOB_EXTRA_1.md)
