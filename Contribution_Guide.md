## Style Guide:

### Be Impersonal
Avoid usage of personal pronouns which reference the author, such as "I", "me", "mine" and so forth. However, you may still be creative and employ your personal writing style.

Bad:
Most of the experienced developers I talk to, feel as though Activities should be used as Container Classes (many even opt to have a Single Activity for the entire application) for...

Good:
The consensus among experienced developers, is that Activities should generally be used as Container Classes (many even opt to have a Single Activity for the entire application), rather than...



### Don't Assume Knowledge
While there are some topics which are truly complex in nature, the majority of difficulty for individuals learning programming languages and concepts, stems from excessive usage of jargon and
nested definitions in order to explain what are often simple concepts. Unless a term or concept has been discussed previously in the curriculum, **assume the student is not aware of it.**

Bad:
Fragments are generally used as Views.

To create a Fragment...

Good:
Fragments are generally used as Views. In this context, the word View is a term from Software Architecture, which refers to a class which is possesses code which is concerned with drawing the User Interface (what the user sees and can interact with) of a particular part of the application. This term is common among many different styles of Software Architecture, such as Model-View-Controller (MVC), Model-View-Presenter (MVP), and Model-View-ViewModel (MVVM).

To create a Fragment...

### Make Purposeful Explanations
If at all possible, try to explain where and when the student may employ the subject material at hand. This may be done by giving a plainly worded explanation, or even by creating a make-belief scenario which the student must work through.

Bad:
Kotlin Extension Functions and Properties, allow the developer to extend the functionality of classes of a particular type, without modifying the source of those classes.

To create an Extension Function...

Good:
Kotlin Extension Functions and Properties, allow the developer to extend the functionality of classes of a particular type, without modifying the source of those classes.

Suppose for example, that you would like all of your Fragments to be capable of quickly and easily showing Toast messages to the User, without adding repetitious code to each individual Fragment. It is possible to use an Abstract Class to solve this problem, but a great alternative in Kotlin
for problems of this kind, is to use an Extension Function...

### Use Code Examples And Diagrams:
It can be very difficult to explain new concepts to individuals who have little to no experience in writing code. For
these individuals, it is especially important to provide concise and relevant code samples, in order to encourage them to "know it in the code" as opposed to being at the mercy of technical or abstract verbal definitions. If the subject
material has not yet been introduced in code, providing graphics is an excellent way to give students a way of conceptualizing the material in a more effective way.

### Use language the simplest words and phrases possible to accurately communicate the concept

### Avoid usage of contractions (for consistency language)

Bad: I'd prefer if you didn't use contractions

Good: I would prefer it if you did not use contractions