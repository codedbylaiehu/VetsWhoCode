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

> For this exercise I swapped between nvim and vscode and I'm finding myself less distracted by vscode than I was previously, specifically when writing markdown. A huge plus for vscode is the live-preview and plugin easy-of-use. nvim is great but to get the enironment fleshed out can take a bit of know-how.

#### My First Javascript Code 

> This little snippet of code helped me to understand so much more of js.
```
<!DOCTYPE html>
<html>
  <head>
    <title>My First JavaScript Code</title>
  </head>
  <body>
    <button onclick="showMessage()">Click me</button>
    <p id="message"></p>
    <script>
      function showMessage() {
        document.getElementById("message").innerHTML = "Hello, World!";
      }
    </script>
  </body>
</html>
```

> I challenged myself to make the next few sections interactive, aiming to use UI elements like buttons and text input boxes. First was concatenating some strings with other object types.

```
    <button onclick="showMessage2()">Get Joe's Info</button>
    <p id="joe"></p>
    <script>
      var name = "Joe";
      let age = 31;
      const height = 71;
      function showMessage2() {
        document.getElementById("joe").innerHTML = "Name: " + name + ", " + "Age: " + age.toString() + ", " + "Height: " + height.toString() + "in.";
      }
    </script>
```

> Next was running a conditional function within a button press AND without affecting the previous buttons or button presses.

```
    <p>Looks like we've got an 85 on our test.</p>
    <button onclick="showMessage3()">Letter Grade</button>
    <p id="grade"></p>
    <script>
      let score = 85;
      function showMessage3() {
        if (score >= 90) {
          document.getElementById("grade").innerHTML = "A Grade";
        } else if (score >= 80) {
          document.getElementById("grade").innerHTML = "B Grade";
        } else {
          document.getElementById("grade").innerHTML = "C or Lower";
        };
      }
    </script>
```

> After that I had to get creative and use a "for loop" inside of another button.

```
    <button onclick="showMessage4()">"For" Loop</button>
    <p id="forLoop"></p>
    <script>
      function showMessage4() {
        for (let i = 0; i < 5; i++) {
        document.getElementById("forLoop").innerHTML = "Count: " + i.toString();
        }
      }
    </script>
```

> The "while loop" was and will be an interesting challenge in rendering on the html page. I suspect I would have to use time instead of counts but I haven't figured a way to display the numbers counting up without modifying DOM

```
    <button onclick="showMessage5()">"While" Loop</button>
    <p id="whileLoop"></p>
    <script>
      function showMessage5() {
        let count = 0;
        while (count < 100) {
          document.getElementById("whileLoop").innerHTML = "looping... " + count.toString();
          count++;
        }
      }
    </script>
```