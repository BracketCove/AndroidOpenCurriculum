## Resources and Layouts

In this lesson, we will discuss the [Project Name]/[Module Name]/src/main/res directory and contents. Although you will come to know these directories through using them (do not worry about memorizing these details), here is a quick overview of them:
- drawable: Graphic resources which may be of various formats such as .png, .jpg, .svg, and so forth
- layout: XML files which are used to create the User Interface of an Android Applicaiton (although it is also possible to do so programmatically in Java or Kotlin)
- mipmap: Specifically used for launcher icons
- values: colors.xml (color resources typically in Hex Code format such as #000000 for Black, #FFFFFF for white), strings.xml (text resources), and styles.xml (similar to CSS, provides styles and themes for your application's aesthetic design) 

### Layouts

**Exercise:** Carrying on from the previous lesson, we will add a new layout for PreferencesActivity:
- Navigate to src/main/res/layout, and right click on the layout directory
- Select New -> Layout resource file
- Enter activity_preferences as the name, then click OK

While you do not need to specifically use that name (or naming convention) for layouts, it is advisable to be some consistent approach to avoid confusing yourself and others.

We will look at building layouts another time, but it is important to note that if you want an Activity to use a specific layout file, that Activity must contain a reference to it within its onCreate() function. Do not worry about the finer details of what onCreate() does (or what a function is); just understand that a common error for beginners is to use the wrong layout file.

**Note:** By convention, the Java programming language uses the word "Method" to refer to what most other languages refer to as a "Function"; including Kotlin. If you are working in Java, please assume each time the word Function is used, it is a synonym (different word for the same thing) for Method.

**Exercise:** Open up MainActivity from your main package. Depending on how AS is configured, you should at minimum see the following code block in the generated file:
    
    class MainActivity : AppCompatActivity() {
    
        override fun onCreate(savedInstanceState: Bundle?) {
            super.onCreate(savedInstanceState)
            setContentView(R.layout.activity_main)
        }
    }

Without worrying about what everything else means, understand that the text within the brackets of the setContentView(...) function, must refer to the correct layout file. Note that in R.layout.activity_main, layout refers to the "layout" folder within src/main/res, and activity_main is the actual name of the layout file within this folder. 

R itself is a file which is generated when you "build" your Android project. It contains a dynamically generated list of the "Resources" which your application can refer to within Java/Kotlin source files. 

**[Previous Lesson](curriculum-en/two/two_two/Activity.md)**<br>
**[Next Lesson](curriculum-en/two/two_four/AndroidManifest.md)**<br>
