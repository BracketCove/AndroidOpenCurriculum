## Building And Deploying To A Device

For the final lesson in this part, we will look at deploying the HelloWorld application to a [device](DevicesAndEmulators.md). 

### Building A Project

Before proceeding with that, ensure that HelloWorld can actually be built in to a deployable APK file. An APK is a packaged version of your application which is ready for debugging. 

**Exercise** Within AS, select Build -> Make Project. If you modified the build.gradle files, you will also be prompted to "Sync Project with Gradle Files", after which AS will also build the project. 

To see the result of the build process, click on the "Build" panel in AS, which is generally located near the bottom of the window. You may also find it via View -> Tool Windows -> Build. Assuming you see "Build: completed successfully", you now have an application which can be deployed to a device.

In the event that the build was unsuccessful, you will generally receive some information on why it failed (although the sad truth is that this information can be vague or useless depending on the cause). You will need to correct this error (or errors) before proceeding, which may necessitate creating a brand new project and starting from scratch.

### Deploying To A Device

**Exercise:** Assuming your device is configured for USB Debugging as mentioned in an earlier lesson, select the green "Run" button, or Run -> Run 'app'. This will open up the deployment target dialogue. If you have correctly configured your device, then you should be able to select it in this dialogue when the device is connected via USB. 

Select your device, and click OK. With luck, a very useless, but very deployable application should now be open on your device. Congratulations!

### Deploying to an Emulator

**Exercise:** If you do not have a physical device (or prefer not to use it), and you do have a system which is capable of running AS Emulators, click on the AVD Manager button, or select Tools -> AVD Manager.

Assuming you have configured an Emulator, select the green Run button in the Actions column within the AVD Manager, and expect to wait several minutes. Once your Emulator loads, you may now select Run -> Run 'app' (in the main AS window). Your Emulator should be visible in the Deploy Target Dialogue now. Select it and click "OK" to deploy your application. Congratulations!

**[Previous Lesson](Gradle.md)**<br>
