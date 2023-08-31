# Building a Simple Responsive Website

In this guide, you'll learn how to build a responsive website from scratch using HTML and CSS.

## Table of Contents

1. Set Up the Environment
2. Create a Basic HTML Structure
3. Implement Global Styles
4. Style the Navigation Bar
5. Design the Hero Section
6. Design the Card Section
7. Add the Contact Section
8. Finalize the Layout

## Step 1: Set Up the Environment

- Create a new folder for your project.
- Inside the project folder, create a sub-folder named `css`.
- In the project folder, create a new file named `index.html`.
- In the `css` folder, create a new file named `style.css`.

## Step 2: Create a Basic HTML Structure

Add the basic structure to `index.html`:

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <link rel="stylesheet" href="css/style.css" />
    <title>Your Website</title>
  </head>
  <body>
    <!-- Navigation -->
    <div id="navbar">
      <div class="nav-content">
        <a href="#hero">Home</a>
        <a href="#cards">Features</a>
        <a href="#contact">Contact</a>
      </div>
    </div>
  </body>
</html>
```

## Step 3: Implement Global Styles

Before we add specific content styles, it's essential to define a set of global styles that apply universally across the website. In `css/style.css`:

```css
/* Global Styles */
body {
  font-family: Arial, sans-serif;
  margin: 0;
  padding: 0;
  background-color: #f4f4f4;
}

img {
  max-width: 100%;
  height: auto;
}

button {
  padding: 10px 20px;
  font-size: 1em;
  border: none;
  cursor: pointer;
}
```

## Step 4: Style the Navigation Bar

Next, add styles for the navigation bar:

```css
/* Navigation Styles */
#navbar {
  background-color: #333;
  overflow: auto;
  text-align: left;
}

.nav-content {
  display: block;
  max-width: 1200px;
  margin: 0 auto;
}

#navbar a {
  color: white;
  padding: 14px 16px;
  text-decoration: none;
  float: left;
}

#navbar a:hover {
  background-color: #555;
  color: white;
}
```

## Step 5: Design the Hero Section

Now, let's design a hero section. Add the following HTML code after the navigation:

```html
<!-- Hero Section -->
<div id="hero">
  <h1>Welcome to My Website</h1>
  <p>This is a simple hero section with a call to action!</p>
  <button>Call to Action</button>
</div>
```

Then, style the hero section:

```css
/* Hero Section Styles */
#hero {
  text-align: center;
  padding: 100px 0;
  background-color: #e9e9e9;
}

#hero h1 {
  font-size: 2em;
  color: #333;
  margin-bottom: 10px;
}

#hero p {
  color: #555;
  margin-bottom: 20px;
}

#hero button {
  background-color: #333;
  color: #fff;
  font-size: 1.2em;
}

#hero button:hover {
  background-color: #555;
  color: #fff;
}
```

## Step 6: Design the Card Section

Add the following HTML code for the card section:

```html
<!-- Card Section -->
<div id="cards">
  <div class="card">
    <img src="https://images.pexels.com/photos/1181246/pexels-photo-1181246.jpeg" alt="Sample Image 1" />
    <h2>Card Title 1</h2>
    <p>Card description here.</p>
  </div>
</div>
```

And then, style the card section:

```css
/* Cards Styles */
#cards {
  padding: 50px 0;
  text-align: center;
  max-width: 1200px;
  margin: 0 auto;
}

.card {
  display: inline-block;
  width: 30%;
  margin: 0 1.5%;
  background-color: white;
  box-shadow: 2px 2px 12px rgba(0, 0, 0, 0.1);
  border-radius: 5px;
  overflow: hidden;
}

.card img {
  width: 100%;
  max-height: 200px;
  display: block;
  object-fit: cover;
}

.card h2,
.card p {
  padding: 10px;
  text-align: left;
}
```

## Step 7: Add the Footer Section

At the bottom of your `index.html`, incorporate the footer section:

```html
<!-- Footer Section -->
<footer id="footer">
    <p>© WEBDEVNCIII 2023</p>
    <div class="social-icons">
        <a href="https://facebook.com" target="_blank" class="fa-icon">
          <i class="fab fa-facebook-f"></i>
        </a>
        <a href="https://twitter.com" target="_blank" class="fa-icon">
          <i class="fab fa-twitter"></i>
        </a>
        <a href="https://instagram.com" target="_blank" class="fa-icon">
          <i class="fab fa-instagram"></i>
        </a>
      </div>
</footer>
```

Now, style the footer by adding these styles to your `css/style.css`:

```css
/* Footer Styles */
#footer {
  background-color: #333;
  padding: 20px 0;
  color: #fff;
  text-align: center;
}

#footer p {
  margin: 0;
  display: inline-block;
  margin-right: 20px;
}

.social-icons {
  display: inline-block;
}

.fa-icon {
  font-size: 24px;  /* Adjust based on desired size */
  margin: 0 10px;
  transition: opacity 0.3s;
  color: #fff;
  text-decoration: none;
}

.fa-icon img {
  width: 24px;  /* Adjust based on desired size */
  height: 24px;  /* Adjust based on desired size */
}

.fa-icon:hover {
  opacity: 0.7;
}
```

With the footer in place, you now have a complete website layout with styled navigation, hero section, card section, and footer with social media icons.

---

## Step 8: Finalize the Layout

Review your HTML and CSS to make sure everything is correctly linked and styled. Test your website in different browsers and screen sizes to ensure it's responsive.
