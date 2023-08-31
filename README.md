Certainly! I'll restructure the guide for the hero and card sections, integrating the CSS code snippets you've provided into the step-by-step instructions for the `README.md` file:

---

# Building a Simple Responsive Website

In this guide, you'll learn how to build a responsive website from scratch using HTML and CSS.

## Table of Contents

1. Set Up the Environment
2. Create a Basic HTML Structure
3. Style the Navigation Bar
4. Design the Hero Section
5. Design the Card Section
6. Add the Contact Section
7. Finalize the Layout

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
    <!-- Content will go here -->
  </body>
</html>
```

## Step 3: Style the Navigation Bar

In `index.html`, under the `<body>` tag, add:

```html
<!-- Navigation -->
<div id="navbar">
  <div class="nav-content">
    <a href="#hero">Home</a>
    <a href="#cards">Features</a>
    <a href="#contact">Contact</a>
  </div>
</div>
```

Add styles in `css/style.css`:

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

**Result**: A top navigation bar with links to different sections.

## Step 4: Design the Hero Section

In `index.html`, add:

```html
<!-- Hero Section -->
<div id="hero">
  <h1>Welcome to My Website</h1>
  <p>This is a simple hero section with a call to action!</p>
  <button>Call to Action</button>
</div>
```

Style the hero section in `css/style.css`:

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

**Result**: A centered hero section.

## Step 5: Design the Card Section

In `index.html`, add:

```html
<!-- Card Section -->
<div id="cards">
  <!-- ... card content ... -->
 <div class="card">
        <img
          src="https://images.pexels.com/photos/1181246/pexels-photo-1181246.jpeg"
        />
        alt="Sample Image 1" />
        <h2>Card Title 1</h2>
        <p>Card description here.</p>
      </div>
      <!-- ... Replicate this twice to create a three cards on this  section
  and use the following link images  
https://images.pexels.com/photos/1181244/pexels-photo-1181244.jpeg
https://images.pexels.com/photos/1181245/pexels-photo-1181245.jpeg-->
</div>
```

Style the card section in `css/style.css`:

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
  margin-bottom: 20px;
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

**Result**: Three stylized cards below the hero section.

## Step 6: Add the Contact Section

In `index.html`, add:

```html
<!-- Contact Section -->
<div id="contact">
  <h2>Contact Us</h2>
</div>
```

Style the contact section in `css/style.css`:

```css
/* Contact Section Styles */
#contact {
  text-align: center;
  padding: 50px 0;
  background-color: #e9e9e9;
}
```

**Result**: A contact section below the cards.

## Step 7: Finalize the Layout

Review your `index.html` and `css/style.css` files, adjust as needed.

---

## Conclusion

You've now built a simple, responsive website from scratch! Continue to experiment, expand, and optimize for various devices. 
