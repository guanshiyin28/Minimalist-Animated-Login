# Simple Minimalist Animated Login

This repository presents a simple, animated login page with a minimalist design, prioritizing a clean user experience and subtle animations.

<hr><br>

## Purpose of This Repository

This repository aims to provide a basic, visually appealing login page implementation that can be easily customized and integrated into various web projects. It serves as a starting point for developers seeking to create clean, user-friendly login interfaces.

<hr><br>

## Demonstration

Here is a demonstration of the function from the `index.html`, `style.css`, and `script.js` files:

### index.html

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <!-- ...existing code... -->
  </head>
  <body>
    <div class="container">
      <div class="signup-section">
        <header>Signup</header>
        <!-- ...existing code... -->
      </div>
      <div class="login-section">
        <header>Login</header>
        <!-- ...existing code... -->
      </div>
    </div>
    <script src="script.js"></script>
  </body>
</html>
```

### style.css

```css
@import url("https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700;800&display=swap");

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: "Poppins", sans-serif;
}

/* ...existing code... */

.container {
  position: relative;
  width: 460px;
  height: 640px;
  border-radius: 12px;
  padding: 20px 30px 120px;
  background: #19a7ce;
  box-shadow: 0 5px 10px rgba(0, 0, 0, 0.1);
  overflow: hidden;
}

/* ...existing code... */

.container.active .login-section {
  bottom: -12%;
  border-radius: 220px;
  box-shadow: 0 -5px 10px rgba(0, 0, 0, 0.1);
}

.container.active .login-section header {
  opacity: 1;
}

.container.active .signup-section header {
  opacity: 0.6;
}
```

### script.js

```javascript
const container = document.querySelector(".container");
const signupButton = document.querySelector(".signup-section header");
const loginButton = document.querySelector(".login-section header");

loginButton.addEventListener("click", () => {
  container.classList.add("active");
});

signupButton.addEventListener("click", () => {
  container.classList.remove("active");
});
```

<hr><br>

## Features

- Minimalist design
- Smooth animations
- Easy to customize
- Responsive layout

<hr><br>

## Technologies Used

- HTML
- CSS
- JavaScript

<hr><br>

## Project Setup

1. **Clone this Repository**

   ```bash
   git clone https://github.com/guanshiyin28/Minimalist-Animated-Login.git
   ```

2. **Navigate to the Project Directory**

   ```bash
   cd Minimalist-Animated-Login
   ```

3. **Open the Project in Your Code Editor**

   ```bash
   code .
   ```

<hr><br>

## Steps to Run

1. **Open the `index.html` File in Your Browser**

   Simply open the `index.html` file in your preferred web browser to see the login page in action.

<hr><br>

## License

This project is licensed under the Apache-2.0 License. See the [LICENSE](LICENSE) file for details.

<hr><br>

<div align="center">
  <a href="https://www.instagram.com/guanshiyin_/">
     <img src="https://capsule-render.vercel.app/api?type=waving&height=200&color=100:393E46,20:F7F7F7&section=footer&reversal=false&textBg=false&fontAlignY=50&descAlign=48&descAlignY=59"/>
  </a>
</div>
