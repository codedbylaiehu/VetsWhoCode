# Vets Who Code 
> codedbylaiehu

## Modules

### HTML and CSS
#### Setting Up HQ

 1 **Setting up** was a challenge because I have used vs code and git before, however I am no git pro yet and cloning / pushing changes to my pre-existing main was an exercise in memory and research. 
 2 **Creating an HTML document**

```
$ touch firstWebPage.html
```

```
<!DOCTYPE html>
<html>
  <head>
    <title>codedbylaiehu's First Web Page</title>
  </head>
  <body>
    <h1>Welcome to my website!</h1>
    <p>This is my first web page.</p>
  </body>
</html>
```

 3 **Adding content to my HTML document**

```
<h1>This is my first heading</h1>

<p>This is my first paragraph.</p>

<!-- This is my image -->
<img src="image.jpg" alt="An image of codedbylaiehu" />

<!-- This is a link -->
<a href="https://www.example.com">Visit Example</a>

<!-- This is an unordered list of my goals -->
<ul>
  <li>Learn more JS</li>
  <li>Learn vim bindings</li>
  <li>Learn Devops</li>
  <li>Become Tech Pro</li>
</ul>
```
#### Styling The Web
 4 **Crafting CSS**

```
$ touch firstWebPageStyles.css
```

```
/* This rule sets the color of all h1 elements to red. */

h1 {
  color: red;
}
```

 5 **Linking CCS to firstWebPage.html**

> Inside of firstWebPage.html

```
<!DOCTYPE html>
<html>
  <head>
    <title>codedbylaiehu's First Web Page</title>
    <link rel="stylesheet" type="text/css" href="styles.css" />
  </head>
  <body>
    <h1>Welcome to my website!</h1>
    <p>This is my first web page.</p>
  </body>
</html>
```

 6 **Style the HTML document**

```
body {
  font-family: Arial, sans-serif;
  background-color: #f2f2f2;
}

h1 {
  color: #333;
  font-size: 36px;
}

p {
  color: #666;
  font-size: 18px;
}
```
### Javascript
#### Preparing My Toolkit
> For this exercise I'm choosing to use nvim instead of vscode because I enjoy the CLI environment more. There is a general lack of creature comforts but there are also less distraction. 
#### My First Javascript Code 
```
<script>
      function showMessage() {
        document.getElementById("message").innerHTML = "HELLO, WORLD!";
      }
    </script>
```

