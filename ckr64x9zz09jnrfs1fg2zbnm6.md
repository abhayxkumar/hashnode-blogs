## Password Strength Checker using HTML, CSS & JavaScript

Hello friends, today in this blog I'm going to design a **Password Strength Checker** by using HTML, CSS & JavaScript.
We can use this to check entered password strength. When typing the password it will show us the strength of entered password in real-time and you can hide or unhide the password in the text field.


![Screenshot 2021-05-21 205350.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1626427061916/DOt0M9vot.png) 

![Screenshot 2021-05-21 205508.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1626427189766/ph1269nLy.png)

![Screenshot 2021-05-21 205543.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1626427199015/MhEpPzK4C.png)


If you are feeling confused about this program or you like watching the video tutorials. I have a full video tutorial of this program given below. I'm sure after watching this video, all your confusion will clear.

### Video of Password Strength Checker using HTML, CSS, & JavaScript
<iframe width="640" height="360" src="https://www.youtube.com/embed/LAvssgpiAZI" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

If you guys are familiar with HTML CSS and JavaScript then you can easily make this program and you can also add more functionality as you want. Those friends who are feeling difficulty creating this program, don't worry I have provided all source code files of this program below. You can copy all codes for free.

## Source Codes
To paste the given codes of this program, first of all, you need to create three files one is an HTML file and one is a CSS file and another one is a JavaScript file. After creating these files then you can copy-paste the given codes in your files.

### HTML Code:

```
<!DOCTYPE html>
<html lang="en">
  <head>
    <title>Password Strength Checker</title>
    <!-- FontAwesome Icons -->
    <link
      rel="stylesheet"
      href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.3/css/all.min.css"
    />
    <!-- Google Font -->
    <link rel="preconnect" href="https://fonts.gstatic.com" />
    <link
      href="https://fonts.googleapis.com/css2?family=Roboto+Mono&display=swap"
      rel="stylesheet"
    />
    <!--Stylesheet-->
    <link rel="stylesheet" href="style.css" />
  </head>
  <body>
    <div class="wrapper">
      <div class="container">
        <input type="password" id="password" oninput="strengthChecker()" />
        <span id="toggle" onclick="toggle()">
          <i class="fas fa-eye"></i>
        </span>
        <div id="strength-bar"></div>
      </div>
      <p id="msg"></p>
    </div>
    <!--Script-->
    <script src="script.js"></script>
  </body>
</html>
``` 

### CSS Code:

```
*,
*:before,
*:after {
    padding: 0;
    margin: 0;
    box-sizing: border-box;
}

body {
    height: 100vh;
    background: #1B262C;
}

.wrapper {
    background-color: #ffffff;
    width: 450px;
    padding: 50px 0;
    position: absolute;
    transform: translate(-50%, -50%);
    left: 50%;
    top: 50%;
    border-radius: 8px;
    box-shadow: 0 20px 25px rgba(0, 0, 0, 0.2);
}

.container {
    width: 300px;
    position: relative;
    margin: auto;
}

input,
p {
    font-family: "Roboto Mono", monospace;
}

input {
    width: 100%;
    height: 50px;
    padding: 0 40px 0 20px;
    position: relative;
    background-color: #f5f5f5;
    border: none;
    outline: none;
    border-radius: 5px 5px 0 0;
}

#toggle {
    position: absolute;
    top: 17px;
    right: 15px;
    color: #808080;
    cursor: pointer;
}

.strength {
    width: 25%;
    display: inline-block;
    position: relative;
    height: 100%;
    bottom: 5px;
}

#strength-bar {
    background-color: #dcdcdc;
    height: 10px;
    position: relative;
}

p {
    width: 100%;
    text-align: center;
    margin-top: 20px;
}
``` 

### JAVASCRIPT Code:

```
let parameters = {
  count: false,
  letters: false,
  numbers: false,
  special: false,
};
let strengthBar = document.getElementById("strength-bar");
let msg = document.getElementById("msg");

function strengthChecker() {
  let password = document.getElementById("password").value;

  parameters.letters = /[A-Za-z]+/.test(password) ? true : false;
  parameters.numbers = /[0-9]+/.test(password) ? true : false;
  parameters.special = /[!\"$%&/()=?@~`\\.\';:+=^*_-]+/.test(password)
    ? true
    : false;
  parameters.count = password.length > 7 ? true : false;

  let barLength = Object.values(parameters).filter((value) => value);

  console.log(Object.values(parameters), barLength);

  strengthBar.innerHTML = "";
  for (let i in barLength) {
    let span = document.createElement("span");
    span.classList.add("strength");
    strengthBar.appendChild(span);
  }

  let spanRef = document.getElementsByClassName("strength");
  for (let i = 0; i < spanRef.length; i++) {
    switch (spanRef.length - 1) {
      case 0:
        spanRef[i].style.background = "#ff3e36";
        msg.textContent = "Your password is very weak";
        break;
      case 1:
        spanRef[i].style.background = "#ff691f";
        msg.textContent = "Your password is weak";
        break;
      case 2:
        spanRef[i].style.background = "#ffda36";
        msg.textContent = "Your password is good";
        break;
      case 3:
        spanRef[i].style.background = "#0be881";
        msg.textContent = "Your password is strong";
        break;
    }
  }
}

function toggle() {
  let password = document.getElementById("password");
  let eye = document.getElementById("toggle");

  if (password.getAttribute("type") == "password") {
    password.setAttribute("type", "text");
    eye.style.color = "#0be881";
  } else {
    password.setAttribute("type", "password");
    eye.style.color = "#808080";
  }
}
``` 

