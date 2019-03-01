## Important Directories And Files

In this part of the curriculum, we will look at the basic anatomy of an Android project. This includes the folders which are most important to know, as well as some information about what you will find within such folders. 

As mentioned in the lesson on [IDEs](IDE.md), you must download and install an IDE to proceed with the practical instructions and exercises moving forward. 

Knowing the basic structure of a typical Android project is of mandatory importance for creating a deployable Android application.

For the purposes of this curriculum, the above terms can be defined as such:
- An Android **project** refers to all files within the root folder of a newly generated project in Android Studio.
- An Android **application** (app), is a compiled (translated into JVM Bytecode), installable, runnable collection of files. These files are typically in the form of an Android Package (APK), which Android Studio can generate for you. 

Until you begin to create multi-module and cross-platform applications, most of the work you will be doing in your AS projects will be within the **[Project/Root Folder Name]/[Module Name]/src/main** folder. 

By default, AS generates a Gradle (discussed soon) Module called "app" each time a new project is created. In the "Project" tab of AS, consider switching to the "Project" View in the dropdown menu at the top of the tab. While you are encouraged to use whatever View suits you best, the Project tab presents an unmodified view of your Android project's files. 

**Exercise:** Before proceeding, open AS and select File -> New -> New Project. Then select "Add No Activity" -> Next. In the name field, enter HelloWorld. Then select your preferred language and hit Finish. Expect to wait some time while AS configures and builds the new project.

### Table of Contents
**[Java And Kotlin Source Files](curriculum-en/two/two_two/Activity.md)**<br>
**[Resources And Layouts](curriculum-en/two/two_three/Layouts.md)**<br>
**[The AndroidManifest Configuration File](curriculum-en/two/two_four/AndroidManifest.md)**<br>
**[The Gradle Build Tool](curriculum-en/two/two_five/Gradle.md)**<br>
**[Deploying An Application](curriculum-en/two/two_six/Deployment.md)**<br>




  