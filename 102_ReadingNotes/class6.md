# Class 6 - Reading Notes

## JavaScript


JavaScript (JS) is a lightweight, interpreted, or just-in-time compiled programming language with first-class functions.
JavaScript is a prototype-based, multi-paradigm, single-threaded, dynamic language, supporting object-oriented, imperative, and declarative (e.g. functional programming) styles.

JavaScript's dynamic capabilities include runtime object construction, variable parameter lists, function variables, dynamic script creation (via eval), object introspection (via for...in and Object utilities), and source-code recovery (JavaScript functions store their source text and can be retrieved through toString()).

### Introduction to JavaScript

That JavaScript code would run in the browser (what we call "client side", as opposed to running on the web server which is called "server side"). 
In recent years people have started to put JavaScript code on the server as well.
Probably the most well know environment to run JavaScript on the server is Node.js, but there are others. For example io.js which started as a Node.js fork.

#### 3 major parts of what we usually refer to as "JavaScript".

1. The language itself. This is fairly standard among the various environments, both in the various browsers and in the various server-side environments.
2. The DOM API - how the language can interact with the various parts of a web page while in the browser. While in this respect the various browsers are getting closer to each other they still differ. Several libraries, most prominently JQuery, is trying to provide a unified API.
3. The server API (or just API) provided by Node.js or one of the other server-side systems.

### alert

```
examples/js/alert.html

<script language="javascript">
 
alert("Hello World");
 
</script>
 ```

### document.write
 ```
 examples/js/document_write.html

First line
<script>
 
document.write("<h1>Hello World</h1>");
 
</script>
Last line
```

### console.log
```
examples/js/console.html

<script>
 
console.log("Hello World");
 
</script>
```
 
## JavaScript input with prompt and confirm

### prompt

t will show a pop-up window with the text provided as the first parameter and with a textbox the user can fill in. When the user presses OK, the value in the text box will be returned by the prompt() function. Then, in this example we use the document.write method to update the html with the text.

```
examples/js/prompt.html

<script>
 
var name = prompt("Your name:", "");
document.write("Hello ", name);
 
</script>
```
```
examples/js/edit.html

<script>
 
var name = prompt("Please correct your e-mail address:", "foo@bar.co");
document.write("Your e-mail address is ", name);
 
</script>
```
### confirm

The other pop-up is not really an input method. It allows the developer to ask a Yes/No question. Calling the confirm() function will show a pop-up window with the provided texts and with two buttons. If the user presses OK the confirm() function will return true, if the user presses cancel or hits the ESC key, the function will return false.

```
examples/js/confirm.html

<script>
 
if (confirm("Shall I print Hello World?")) {
    document.write("Hello World");
} else {
    document.write("OK, I won't print it.");
}
 
</script>
```


#### References

https://developer.mozilla.org/en-US/docs/Web/JavaScript

https://code-maven.com/introduction-to-javascript

https://code-maven.com/javascript-input-with-prompt-and-confirm

https://darranholmes74.github.io/reading-notes/102_ReadingNotes/class6.html