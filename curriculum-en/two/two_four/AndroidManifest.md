## The Android Manifest

In this lesson, we will discuss one of the most important configuration files in any Android project. You can find this file in:
[Project Name]/[Module Name]/src/main/AndroidManifest.xml

Within the AndroidManifest (hereby AM), you should find the following information:

    <?xml version="1.0" encoding="utf-8"?>
    <manifest xmlns:android="http://schemas.android.com/apk/res/android"
              package="com.opensource.helloworld">
    
        <application
                android:allowBackup="true"
                android:icon="@mipmap/ic_launcher"
                android:label="@string/app_name"
                android:roundIcon="@mipmap/ic_launcher_round"
                android:supportsRtl="true"
                android:theme="@style/AppTheme">
            <activity android:name=".MainActivity">
            </activity>
        </application>
    
    </manifest>
    
There is a great deal of different configurations available in the AM, most of which are global configurations for your application. We will take a brief look at these different configurations and tags.

### "manifest" Tag

The root tag for this file, "manifest", contains the package attribute. The value of this attribute dictates the unique package name for your application. When you reach the point of uploading an application to the Play Store (among other distribution platforms), you must keep this same package name for all subsequent updates to that application. 

If your application requires access to device features such as network or local storage, you will need to add <uses-permission android:name=""/> tags for each as a child tag within <manifest> (not within the application tag!)

### "application" Tag

This is where you will find global configurations for your application. Important attributes include:
- android:icon which specifies what image resource is to be used as the launcher icon in your app
- android:label which specifies the "name" of your application (generally visible under the launcher icon)
- android:theme which specifies the primary theme of your application. These are pre-made (or custom) styling configurations which save you from having to style your application from scratch each time

### "activity" Tag

Each time you create a new Activity via the wizard, an <activity> tag is added to the AM. As expected, MainActivity was added, but there is no entry present for PreferencesActivity which we manually added to the main package. 

**Exercise:** Go ahead an add the following tag within the application tag:

            <activity android:name=".PreferencesActivity"/>

Ensure that it is spelled correctly, but do not worry if it is showing up as an error; we will fix that shortly.

**Exercise:** When your application has more than one Activity, you may wish to specify which Activity should be the first one to be launched when your application is executed on an Android device. Again, without worrying too much about the specifics, add the following tags to your MainActivity's entry in the AM:

    <activity android:name=".MainActivity">
                <intent-filter>
                    <action android:name="android.intent.action.MAIN" />
                    <category android:name="android.intent.category.LAUNCHER" />
                </intent-filter>
    </activity>
    <activity android:name=".PreferencesActivity"/>

**[Previous Lesson](curriculum-en/two/two_three/Layouts.md)**<br>
**[Next Lesson](curriculum-en/two/two_five/Gradle.md)**<br>