## 1. HTML and CSS
HTML stands for hypertext markup language. It isn't a programming language, but it is commonly confused as one. It is a markup language. It uses carrots like so ```<``` ```>``` to denote an HTML tag. The tag informs the web browser how to render the content in a tag. 

```html
<!-- this is an HTML comment, below is an unordered list -->
<ul>
   <li>One Fish</li>
   <li>Two Fish</li>
   <li>Red Fish</li>
</ul>
```

### Standard HTML index file
An index file is the main HTML page that is loaded for a web application. A standard HTML index file could look like this:

```html
<html>
  <head>
    <!-- this is the header tag, this is where you would import javascript files and CSS files that interact with your HTML -->
    <title>Sample "Hello, World" Application</title>
  </head>
  <body>
    
    <!-- table tag -->
    <table border="0" cellpadding="10">
      <tr>
        <td>
          <!-- image tag, an image loaded from a URL -->
          <img src="images/springsource.png">
        </td>
        <td>
          <h1>Sample "Hello, World" Application</h1>
        </td>
      </tr>
    </table>
   
    
    <!-- paragraph tags -->
    <p>This is the home page for the HelloWorld Web application. </p>
    <p>To prove that they work, you can execute either of the following links:
   
    <!-- unordered list tags and hyper-link tags "a" -->
    <ul>
      <li>To a <a href="hello.jsp">JSP page</a>.
      <li>To a <a href="hello">servlet</a>.
    </ul>

  </body>
</html>
```

### HTML/CSS Classes and IDs
To style an HTML tag, you can add a **class** or **id** to that HTML tag and add CSS styles. As an example, here is a snippet of html that would change the color and font size of a header tag:
```html
<html>
   <head>
      <!-- embedded CSS is denoted with style tags -->
      <style>
          #mainHeader{  /* the ID is denoted with a hashtag in front of the name */
               color:red;
               font-size: 28px; /* these semi-colons are required! */
          }
           
          .embolden{   /* this will bold any HTML contents where the tag surrounding those contents has the "embolden" class */
               font-weight:bold;
           }
      </style>
   </head>
   <body>
      <h1 id="mainHeader">My First Header!</h1>
      <p class="embolden">
          For styles that you want to use over and over on multiple tags, you would use a class. The style for this is called embolden and you can throw it on any tag 
      </p>
   </body>
</html>
```


### Javascript
Javascript is the programming language of the web browser. Every browser is able to read javascript. Javascript is a front-end language, front-end because it is used to interact the with very elements that a user will visibly see and touch (via user input). Javascript uses curly brackets ```{}``` and semicolons ```;```. Javascript can be embedded into HTML very easy, here is a sample webpage that produces a popup alert:

```html
<html>
   <head>
      <!-- embedded JS is denoted with script tags -->
      <script>
           // this is a function in javascript. when the main button is clicked, it will call this function.
           function hello_world(){
                alert("Hello USER!");     // this will produce a pop-up alert printing the words "Hello USER!"
           }
      </script>
   </head>
   <body>
       <!-- we use the HTML tag attribute "onclick" to call javascript functions -->
       <button onclick="hello_world()">Push Me</button> 
   </body>
</html>
```
