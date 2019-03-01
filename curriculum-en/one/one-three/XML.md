## Extensible Markup Language

XML, which stands for (Extensible Markup Language), is like HTML with fewer rules. While it was frequently used as a language for modelling and sharing data in a human and machine readable format in the past (JSON is generally used for this purpose nowadays), it is still used frequently on the Android Platform for creating Layouts, Views, and configuration files. Such topics will be discussed in the next part; for now, please familiarize yourself with the structure of XML:


XML as a language, is comprised of the following things:
#### Tags/Elements:
A basic XML Tag is made of angle brackets and some text:

    <!-- Comments use exclamation marks and dashes --!>
    <Human> 
           <Name>John Doe</Name>
    </Human>
    
    <!-- tags may be closed on a single line as below --!>
    <Cat/>
As you can see, you may place tags within tags if necessary, as long as you correctly write the slash to indicate when a tag is open or closed.     

#### Attributes:
Tags may contain attributes. The only rule for attributes is that the name of the attribute is given,
followed by the equals sign, and the value of the attribute:
<Cat scientificName="Felis Catus"/>

#### Namespaces:
Since XML does not restrict you to using any particular names (however, the Android SDK will expect you to use specific tags and attributes), there is a risk of repeating the names of attributes within a given XML file. In order to avoid this situation, we can prefix an attribute with a "namespace" (the thing before the colon). This provides more information to the programs which read these XML files; thus avoiding accidental duplication and allowing attributes to be reused when appropriate:

    <TextView
        android:text="Hello Universe!"
        tools:text="Hello World!"/>

For example, as we will see with Layouts (which form the basis of building a User Interface on Android), the tools namespace can be used to add "design-time" data to your layouts, to preview what they look like without having to compile and deploy the application:

**[Previous Lesson](Primary_Languages.md)**<br>
**[Next Lesson](IDE.md)**<br>