## Java And Kotlin Source Files

In this lesson, we will discuss the main/java directory (folder) and some information about its contents.

As mentioned in the previous section, most of the work you will be doing, will be within the following folder:
[Project Name]/[Module Name]/src/main/java

**Exercise:** Assuming that you followed the instructions in the previous lesson to create a new project, locate the "java" directory for this new project. Supposing that you chose the name "HelloWorld" for the new project, you will find it here:
*HelloWorld/app/src/main/java*

**Note:** If for some reason you are not able to locate this directory in Android Studio, you will likely need to switch to the "Project" View from the dropdown menu in the Project Panel.

Within this file, you will found your application's main package, which looks something like:
*com.opensource.javaexamples* or *com.opensource.kotlinexamples*

A "package" is a series of directories (folders) with two purposes:
- It indicates where you likely will find, and where to add, the Java/Kotlin source files for the project.
- It provides a unique identifier for your application in the form of the names of the directories which look rather like a website. In fact, if you have your own personal website, you may use a package name which includes this website in the next project you create, such as: *com.mytechblog.helloworld*

### Creating Activity Classes

**Exercise:** Before proceeding, please create a new Activity using the AS New Activity wizard:
1. Navigate to the bottom level directory of your main package, which should be called "helloworld"
2. Right-click on this directory
3. Select New -> Activity -> Empty Activity
4. Ensure that the "Generate Layout File" checkbox is selected, but otherwise use defaults
5. Select Finish

Android Studio's new Activity wizard performs the following operations (assuming defaults have been left alone):
- An Activity file called MainActivity (which may have an extension of either .java or .kt) is added to the projects main package
- A Layout file for this Activity was added to the [Project Name]/[Module Name]/src/main/res/layout (we will discuss Layouts in another lesson)
- An entry within the AndroidManifest file at [Project Name]/[Module Name]/src/main/AndroidManifest.xml for an Activity was added (also discussed in another lesson)

As is often the case with convenient tools like the new Activity wizard, the convenience can tend to hide what is actually occurring in order to get the expected result. 

**Exercise:** We will now manually add a new Activity in steps. Again, right click on the *helloworld* directory, but this time select New -> Java Class, or New -> Kotlin File/Class. For the name, type PreferencesActivity then select OK.  

In the next few lessons, we will look at the other directories present within the main directory. Some common beginners mistakes in manually adding these files comes from:
- Not adding a Layout file for the new Activity
- Using the wrong Layout file for the new Activity due to a copy/paste error
- Not adding an entry for the Activity within the AndroidManifest.xml file.

**[Previous Lesson](curriculum-en/two/two_one/DirectoryOverview.md)**<br>
**[Next Lesson](curriculum-en/two/two_three/Layouts.md)**<br>





