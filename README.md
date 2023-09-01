
# Building a Simple Responsive Website

In this guide, you'll learn how to build a responsive website from scratch using HTML and CSS.

## Table of Contents

1. [Set Up the Environment](#step-1-set-up-the-environment)
2. [Create a Basic HTML Structure](#step-2-create-a-basic-html-structure)
3. [Implement Global Styles](#step-3-implement-global-styles)
4. [Style the Navigation Bar](#step-4-style-the-navigation-bar)
5. [Design the Hero Section](#step-5-design-the-hero-section)
6. [Design the Card Section](#step-6-design-the-card-section)
7. [Creating the "About" Section](#step-7-creating-the-about-section)
8. [Setting Up the "Testimonials" Section](#step-8-setting-up-the-testimonials-section)
9. [Add the Footer Section](#step-9-add-the-footer-section)
10. [Finalize the Layout](#step-10-finalize-the-layout)

## Step 1: Set Up the Environment

1. Create a new folder for your project.
2. Inside the project folder, create a sub-folder named `css`.
3. In the project folder, create a new file named `index.html`.
4. In the `css` folder, create a new file named `style.css`.

## Step 2: Create a Basic HTML Structure

Add the basic structure to `index.html`:

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta http-equiv="X-UA-Compatible" content="IE=edge">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <link rel="stylesheet" href="css/style.css">
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

Define a set of global styles in `css/style.css`:

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

Style the navigation bar in `css/style.css`:

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

Add and style the hero section in `index.html` and `css/style.css`:

**HTML:**

```html
<!-- Hero Section -->
<div id="hero">
  <h1>Welcome to My Website</h1>
  <p>This is a simple hero section with a call to action!</p>
  <button>Call to Action</button>
</div>
```

**CSS:**

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

Add the card section in `index.html` and style it in `css/style.css`:

**HTML:**

```html
<!-- Card Section -->
<div id="cards">
  <div class="card">
    <img src="https://images.pexels.com/photos/1181246/pexels-photo-1181246.jpeg" alt="Sample Image 1">
    <h2>Card Title 1</h2>
    <p>Card description here.</p>
  </div>
  <!-- Add more card blocks as needed -->
</div>
```

**CSS:**

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

## Step 7: Creating the "About" Section

Set up the "About" section:

**HTML:**

```html
<!-- About Section -->
<div id="about">
  <div class="about-img">
    <img src="https://images.pexels.com/photos/3184360/pexels-photo-3184360.jpeg" alt="About Image">
  </div>
  <div class="about-content">
    <h2>About Us</h2>
    <p>This is some information about our company. We do wonderful things and are awesome!</p>
  </div>
</div>
```

**CSS:**

```css
#about {
  padding: 50px 0;
  max-width: 1200px;
  margin: 0 auto;
  text-align: center;
}

.about-img,
.about-content {
  display: inline-block;
  width: 48%;
  vertical-align: top;
  box-sizing: border-box;
}

.about-img img {
  width: 100%;
  border-radius: 5px;
}

.about-content {
  padding: 0 2%;
}
```

## Step 8: Setting Up the "Testimonials" Section

Include client testimonials:

**HTML:**

```html
<!-- Testimonials Section -->
<div id="testimonials">
  <h2>Our Clients</h2>
  <div class="testimonial-img">
    <img src="https://via.placeholder

.com/150" alt="Client Image">
  </div>
  <div class="testimonial-content">
    <p>"This company did amazing things for me!" - Happy Client</p>
  </div>
  <!-- Add more testimonials as needed -->
</div>
```

**CSS:**

```css
#testimonials {
  padding: 50px 0;
  background-color: #f4f4f4;
  text-align: center;
}

.testimonial-img img {
  width: 150px;
  height: 150px;
  border-radius: 50%;
}

.testimonial-content {
  padding: 20px 0;
  font-style: italic;
}
```

## Step 9: Add the Footer Section

End with the footer:

**HTML:**

```html
<!-- Footer Section -->
<div id="footer">
  <p>© 2023 by My Website. Proudly created by [Your Name]</p>
</div>
```

**CSS:**

```css
#footer {
  padding: 20px 0;
  background-color: #333;
  color: white;
  text-align: center;
}
```

## Step 10: Finalize the Layout

Now that all sections are in place, make final adjustments:

1. Ensure each section is properly spaced.
2. Check that the website is responsive by adjusting the browser size.
3. Test the site on various devices for compatibility.

