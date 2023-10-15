# HTML
* Hypertext Markup Language


- What is HyperText?
- hypertext is the text that contains links to other text.
- Markup lang is a way to give instructions to a computer about how content should be organized and displayed.
```
<p> </p>
paragraph tag
<p>This is a <strong>bold</strong> text.</p>
```
- What is Hypertext?
- hypertext is text that contains links to other text.


- HTML 5 (2014)
- HTML 5 has Semantics, and better support for web applications, It introduced new elements like
```
<video> , <audio> , <picture>
```
and much more
- html5 made web development more versatile and capable.


- HTML Syntax
```
<h1> Opening Tag
content :)
</h1> Closing Tag
all of this is called an HTML ELEMENT




Headings = <h1></h1>
<h2></h2>
<h3></h3>
<h4></h4>
```
- Index.html
- file extension must be **.html or .htm**
- MS-DOS and Windows 3.1 had limitations in the number of characters in file name
- the file name must be **index.html** because it's the default path of our homepage or the root of our website.




## HTML Documents and Structure


```
<!DOCTYPE html>


<html>
<head>
<title> Home page </title>
</head>


<body>
<h1> best html course </h1>
</body>
</html>


```
- !DOCTYPE html --> Let the browser know it's an HTML5 Appear once, at the top of the page.
- HTML --> Root of an HTML document


- head --> Contains the information about the HTML Document
- title --> title of the HTML page


- body --> Contains everything you want to display on the Web page


- h1 --> defines a large heading


## How the browser determines the language of an HTML document.
- after DOCTYPE we have to write another line that is
- html lang = "en"
- lang is an Attribute
- Lang is a type of attribute that specifies the language of the element's contents.
- en --> Specify the language code for the element's content
- if i want to write in Hindi --> lang = "hi"
for Korean lang = "ko"
for France lang = "fr"


## HTML Attribute


- The lang Attribute
- en Specifies the language code for teh element's content 
- What are Attribute in HTML
- Attributes are used along with the HTML tags to define the element's characteristics.
- Attributes provide additional information about the elements

## HTML Headings and Text
- Question know the difference between Tags and Elements
- Headings 
   - From h1-h6
   ```
   <h1> Heading 1</h1> largest one 
   MAX pixel size = Typically largest and Bold, around 24px to 36px or even larger. 
   <h2> Heading 1</h2>

   MAX pixel  size = Slightly smaller, around 18px to 30px.
   <h3> Heading 1</h3>

   MAX pixel  size = Smaller than h2, around 16px to 24 px 
   <h4> Heading 1</h4>

   MAX pixel  size = generally, around 14px to 20 px
   <h5> Heading 1</h5>

   MAX pixel  size = smaller often around 12 to 18 px
   <h6> Heading 1</h6>
   MAX pixel  size = the Smallest, around 10px to 16px.
   ```
  - Notes on Html
      - The tag element name is case insensitive.
      - A single H1 is typically used per page
      - Follow the hierarchy from H1 to H6 consistently.
   - Why we don't skip the size of h1 to h3 directly --> Skipping heading levels can be confuse both the users and search engines. It's best to maintain a proper hierarchical structure for better accessibility and SEO. 

- Paragraphs
   ```
   <p> This is a Paragraph </p> 
   The <p> Tag defines a paragraph 

   Browsers automatically add a single blank line before and after each <p> element 
   ```
   -  can we nest other HTML tags in the P tag --> NO we can't 
   Because p is already a block element we can't nest other block elements in in a block element itself. 
   But we can Include Inline elements in the p tag like 
   ```
   <Strong>, <em>
   ```
- Line Break 
   - br
   - to break a Paragraph.
- Horizontal rule
   - hr
   - It gives a horizontal line in between Paragraphs.
   - <hr> 

- No matter how much whitespace you use inside HTML element content (which can include one or more spaces characters, but also line breaks), the HTML parser reduces each sequence of whitespace to a single space when rendering the code.

## Comments in HTML 
``` 
<!-- Comment here-- >
```
- To comment out in HTML, Insert Information between <!-- and --> tags (Browser won't show these notes)

- commenting in HTML allows developers to leave notes about their code and its functionality or to indicate necessary changes for the future.

## Text Formatting
   - Bold and Italic   
      ```
         <strong>, <em>
      ```

   - Underline and Strikethrough: 
      ```
      <u>, <s>
      ```
   - Subscript and superscript
      ```
      <sub>, <sup>
      ```
   - Preformatted Text
      ```
      <pre> --> used to give formatting to the text that can't be done using <p> tag
      , <kbd> --> its full form is a Keyboard for commands  
      it's used to show keyboard commands to the user
      ,<abbr> --> it's short of Abbreviation 
      Used to tell abbreviation to the user 
      like WHO = World Health Organization.
      <abbr title = "World Health Organization"> WHO </abbr>
      ```
   - Text Highlighting
      ```
      <mark> --> Highlighting of text, 
      <small> --> makes text smaller,
      <del> -->  It was used to show the modification of the document the output may be the same as strikethrough but the use case is different.
      ```
   
      - the **s** Tag specifies text that is no longer correct, accurate or relevant, 
      - The **del** Tag is used to identify text that has been deleted from a document but retained to show  the history of modification made to the document.
   - Inline Styling
      ```
      <sub>, <sup>
      ```
      - CSS is imp in showing the website in a better way 
      ```
      <p style= "red"></p> 
      ```  
   -  TIP --> While using nested tags in one element never mismatch the tags
      ```
      ❌ <p>My cat is <strong>very grumpy.</p></strong>
      ✅ <p>My cat is <strong>very</strong> grumpy.</p>
      ```

## HTML Anchor Tag
 - The **a** tag defines a hyperlink, which is used to link from one page to another.
 - Attributes of Anchor tag 
      - herf = the URL or the destination the link points to
      - Target = specifies where the linked content will be displayed (eg = _blank --> for a new window/tab)
      - rel = Describes the relationship between the current page and the linked page. "NOT used in real practice"
      - title =  provides additional information about the link
      - id = assigns a unique identifier to the anchor tag for linking within the page.
      "helps us redirect some request to a section of the page also"
      - Class = Assigns a class for styling or JavaScript interactions
      - style: Applies inline CSS styling to the anchor.  
      - tabindex: Specifies the tab order when navigating using the keyboard.
      - accesskey: Defines a keyboard shortcut to activate the link.
      - aria-*: Attributes for accessibility purposes (e.g., aria-label). 
      - Download: Suggests that the target will be downloaded when clicked.

- Question 
   - How can you create a link within the same webpage that takes the user to a specific section or element on the page?
      --> use the id Attribute 

   - **Also we can make it with smooth scrolling**
      - Go to head 
      - in it use style tag 
      - and add a property 
      - CSS scroll property 
      - scroll-behavior 
      - make it smooth
      - It will look like this 
      ```
      <head>
         <meta charset="UTF-8">
         <meta http-equiv="X-UA-Compatible" content="IE=edge">
         <meta name="viewport" content="width=device-width, initial-scale=1.0">
         <title>Html anchor tag</title>
         <style>
            html{
               scroll-behavior: smooth;
            }
         </style>
      </head>
      ```
   - What's the difference between relative and absolute URLs in the href attribute?
      --> 
      <br>
      **Relative path**
      <br>Relative URLs are URLs that are relative to the current page's URL.
      <br>
      **Absolute path** 
      <br>Absolute URLs are complete URLs, including the protocol (http/https) and domain.
   
   - How does the download attribute work in the anchor tag?
   --> Download used in the anchor tab is easy 
   ```
    <a href="./html.zip" download>Download Zip file  </a>
   ```
   - How do you create an HTML link that opens the user's default email client with a specific email address?

   ```
   <a href="mailto:Sahajjain@gmail.com">send me a email</a>
   Also, we can hit the call 
   <a href="tel:+919876543210">Call us</a>
   <br>
   and we can open WhatsApp to add them to a group.
   <a href="LINK_GOES_HERE"> join the wp group</a>
   ```

- Bonus 
   - When to use Quotes
   <br>
   So the best practice is to Always include the attribute quotes. It avoids such problems, and results in more readable code.
   <br>
   - Single or Double Quotes?
   <br>
   **Double Quotes are Best Practice** 
   & remember that using one double and one single is **not RIGHT.** 

## HTML Entities 
   - HTML entities are codes used to represent special characters and symbols that have reserved meanings in HTML. These entities are especially important when you  want to display characters that might conflict with HTML syntax or when you want to display characters that aren't directly available on your keyboard. HTML entities are represented using an ampersand (&) followed by a code and a semicolon (;)
      - **&lt**; = Less than sign "<"
      - **&gt**; = greater than sign ">"
      - **&amp**; = Ampersand "&"
      - **&quot**; = Double Quote (")
      - **&apos**; = Apostrophe or Single Quote"'"
      - **&nbsp**; = non Breaking space " "
      - **&dollar**; = Dollar sign "$"
      - **&copy**; = Copyright symbol " &copy;"
      - **&reg**; = registered trademark symbol"&reg;"
      - **&trade**; = Trademark symbol "&trade;"
      - **&hearts**; = Heart symbol " &hearts;"
- Question 
   - When we need to use nbsp -->The **&nbsp** entity is used to insert a non-breaking space, which prevents the browser from collapsing consecutive spaces into one
   - How would you display a trademark symbol using an HTML entity? <br> --> You can display a trademark symbol using the &trade; entity: **&trade** ; 
   - Why is it important to use HTML entities for special characters?
   <br>         
   --> Using HTML entities ensures proper rendering of characters and symbols and helps avoid conflicts with HTML syntax
   - 4: Represent the dollar sign symbol using different HTML entity methods
   <br>
   --> Using Named Entity: &dollar ; & also Using Hexadecimal Numeric Reference: #x00024; OR Using Decimal Numeric Reference: &#36 ; 

## Image tag 
 - the <**img**> tag is used to embed(ADD) an image in an HTML page.
 ```
 <img src = "/image.png" alt= "alt text"/>

sre --> Specifies the path of teh image
alt --> specifies an alternate text for the image, if the image for some reason cannot be displayed.
width --> width of the image
height --> height of the image
title --> give extra info about the image
loading --> lazy Meaning that the image will load only when you get to the section not before that 

This helps reduce the load on server side.
 ```
 - Some Deprecated image tags Align, Border, hspace, vpace.
 - Best practice 
 ``` 
 ❌ <img alt="image" src="penguin.jpg" /> 
 Bad for Seo ranking

 ✅<img  alt="A Rockhopper Penguin standing on a beach."  src="penguin.jpg" /> 
 ``` 

 - Always write proper description in alt Attribute
 - how to make image responsive 
      - Width = 100% 
      - height = auto
      - we can also update the css in that we can say max-width = 500px;
- Question 
  - How would you make an image responsive using the width attribute?
  <br> You can set the width attribute to a percentage value (e.g., width="100%") to make the image adjust its width based on the available space.
  - How do you create an image link using the <**img**> tag? <br> You wrap the <**img**> tag with an anchor <**a**> tag and provide the href attribute in the <**a**> tag.
  - What's the difference between relative and absolute URLs in the href attribute? <br> Relative URLs are URLs that are relative to the current page's URL.<br> Absolute URLs are complete URLs, including the protocol (http/https) and domain.
  - Why is providing descriptive alt text for images important? It improves  <br> accessibility for users with visual impairments and helps search engines understand image content.
  - Another way to clicking the image is Map Elements

  ```
   <img src="./images/html.png" 
  alt="Clickable World Map"
  usemap = "#map"
  width = "250"
  height = "150"
  />

  <map name="map">
    <area 
    shape="rect" 
    coords="0,0,125,150" 
    href="https://youtube.com/watch?v=5ccq_nLHneE" 
    alt="My yt channel link"
    />
    <!--     <area 
    shape="polygon" 
    coords="300, 1001 350, 200, 250, 200" 
    href="https://youtube.com/watch?v=5ccq_nLHneE" 
    alt="south Area"
    /> -->
    <!--     <area 
    shape="circle" 
    coords="200,150,50" 
    href="https://youtube.com/watch?v=5ccq_nLHneE" 
    alt="Central Area"
    /> -->
  </map>

  area --> is the area where it's clickable 
  shape --> in which shape it's clickable 
  coords --> coordinates of the shape in image 
  href --> link 
  alt --> alternative
  ```
  - we can use map tag to define an image map. An image map is an image which clickable area.
  - the required name attribute of the map element is associated with the img's usemap attributes and creates a relationship between the image and map.
- Advanced part
   - srcset --> The srcset attribute specifies the URL of the image to use in different situations.
   - sizes --> The sizes attribute on an <**img**> element specifies different image widths <br>  These widths are tied to browser conditions which helps create responsive images.

## Void Elements In HTML
 - Void elements / Empty elements
      - Not all parts of web page use the usual pattern of having an opening tag, some content, and then a closing tag. Some parts only need a single tag to work. These are called "void element" or "Empty elements".
      - Examples = img tag, Area Tag, br tag , hr tag, etc.


## Picture Tag 
 - The <**picture**> HTML elements contains zero or more <**source**> elements and one <**img**> element to offer alternative versions of an image for different display/devices scenarios.

 ```
 <picture>
 <source srcset = "./sahaj.webp">
 <source srcset = "./sahaj.png">
 <img src = "./Sahaj.jpg" alt = "" />
 </picture> 

 it will try to load 1st one and then the second and so on.

 the images in all 3 formats should be same
 ```
 - use webp because it's file size is smaller than any other extension.

 ```
     <picture>
      <source srcset="./images/html.webp" type="image/webp" />
      <source srcset="./images/html.jpg" type="image/jpg" />
      <source srcset="./images/html.jpeg" type="image/jpeg" />
      <source srcset="./images/html.svg" type="image/svg" />
      <img
        src="./images/html.png"
        alt="best html course by sah"
        width="500"
      />
    </picture>
``` 

## Figure HTML
 - The <**figure**> tag specifies self-contained content, like illustrations, diagrams, photos, code listings, etc.

- While the content of the <**figure**> element is related to the main flow, its position is independent of the main flow, and if removed it should not affect the flow of the document.

- Tip: The <**figcaption**> element is used to add a caption for the <**figure**> element.

## List in HTML 

 - Unordered HTML List
An unordered list starts with the <**ul**> tag. Each list item starts with the <**li**> tag.
 - The list items will be marked with bullets (small black circles) by default:
 - Unordered List (<**ul**>) Styles:
```
   <ul>
      <li>Coffee</li>
      <li>Tea</li>
      <li>Milk</li>
   </ul>
```
- Ordered HTML List
An ordered list starts with the <**ol**> tag. Each list item starts with the <**li**> tag.
- The list items will be marked with numbers by default:

 ```
 <ol>
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ol>
 ```

