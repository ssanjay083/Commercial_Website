# Ex02 Commercial Website
## Date: 23.02.2026

## AIM
To create a commercial website using CSS Flexbox.

## ALGORITHM
### STEP 1
Create an HTML file (index.html)

### STEP 2
Create a CSS file (style.css)

### STEP 3
Include a navigation bar with links to different sections.

### STEP 4
Add structured sections for Homepage, Products / Services, About Us, Contact Details and User Account.

### STEP 5
Include social media links at the footer with copyright information.

### STEP 6
Define global styles for fonts, colors, and layout.

### STEP 7
Style the header, navigation bar, and sections.

### STEP 8
Use Flexbox for layout design.

### STEP 9
Add hover effects and transitions for interactivity.

### STEP 10
Add Images and Media.

### STEP 11
Use optimized images for a professional look.

### STEP 12
Open the HTML file in a browser to check layout and functionality.

### STEP 13
Fix styling issues and refine content placement.

### STEP 14
Deploy the website.

### STEP 15
Upload to GitHub Pages for free hosting.

## PROGRAM
### HTML :
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>ProTech Solutions</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

    <!-- Header -->
    <header>
        <h1>ProTech Solutions</h1>
    </header>

    <!-- Navigation -->
    <nav>
        <ul class="nav-links">
            <li><a href="#home">Home</a></li>
            <li><a href="#about">About Us</a></li>
            <li><a href="#products">Products</a></li>
            <li><a href="#services">What We Provide</a></li>
            <li><a href="#contact">Contact</a></li>
            <li><a href="#account">User Account</a></li>
        </ul>
    </nav>

    <!-- Home Section -->
    <section id="home" class="section hero">
        <h2>Welcome to ProTech</h2>
        <p>Your one-stop solution for modern web and mobile services.</p>
        <img src="https://images.unsplash.com/photo-1498050108023-c5249f4df085"
             alt="Technology Workspace">
    </section>

    <!-- About Section (NOW FIRST AFTER HOME) -->
    <section id="about" class="section about-flex">
        <div class="about-text">
            <h2>About Us</h2>
<p>
    ProTech Solutions is a fast-growing technology company specializing 
    in web and mobile development. We provide innovative digital solutions 
    tailored to meet client requirements.
</p>

<p>
    Our mission is to deliver reliable, scalable and secure solutions 
    that empower businesses to grow in the digital world.
</p>
        </div>

        <div class="about-image">
            <img src="https://images.unsplash.com/photo-1522071820081-009f0129c71c"
                 alt="Our Team">
        </div>
    </section>

    <!-- Products Section -->
    <section id="products" class="section">
        <h2>Our Products</h2>
        <div class="flex-container">
 <div class="card">
    <img src="https://images.unsplash.com/photo-1498050108023-c5249f4df085" alt="Web Development">
    <h3>Web Development</h3>
    <p>
        We build responsive, high-performance and SEO-optimized websites 
        using modern technologies like HTML, CSS, JavaScript and frameworks.
        Our solutions ensure speed, security and scalability.
    </p>
</div>

<div class="card">
    <img src="https://images.unsplash.com/photo-1518770660439-4636190af475" alt="App Development">
    <h3>App Development</h3>
    <p>
        We develop user-friendly Android and iOS applications with 
        modern UI/UX design. Our apps are secure, scalable and optimized 
        for performance across multiple devices.
    </p>
</div>

<div class="card">
    <img src="https://images.unsplash.com/photo-1460925895917-afdab827c52f" alt="Digital Marketing">
    <h3>Digital Marketing</h3>
    <p>
        Our digital marketing services include SEO, social media marketing,
        content creation and online advertising to boost brand visibility 
        and increase customer engagement.
    </p>
</div>
        </div>
    </section>

    <!-- What We Provide -->
    <section id="services" class="section">
        <h2>What We Provide</h2>
        <div class="flex-container">
<div class="card">
    <h3>Website Design</h3>
    <p>
        Custom-designed websites with creative layouts, smooth navigation
        and responsive design to provide excellent user experience.
    </p>
</div>

<div class="card">
    <h3>Mobile Apps</h3>
    <p>
        Cross-platform mobile applications with secure backend systems
        and modern features tailored to business requirements.
    </p>
</div>

<div class="card">
    <h3>Cloud Solutions</h3>
    <p>
        Reliable cloud hosting, data storage, and scalable infrastructure
        services to ensure business continuity and security.
    </p>
</div>

<div class="card">
    <h3>IT Consulting</h3>
    <p>
        Strategic IT consulting services to help businesses adopt
        the latest technologies and improve operational efficiency.
    </p>
</div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="section">
        <h2>Contact Details</h2>
        <p>Email: info@protech.com</p>
        <p>Phone: +91 9876543210</p>
        <p>Location: Chennai, India</p>
    </section>

    <!-- User Account Section -->
    <section id="account" class="section">
        <h2>User Login</h2>
        <form>
            <input type="text" placeholder="Username" required>
            <input type="password" placeholder="Password" required>
            <button type="submit">Login</button>
        </form>
    </section>

    <!-- Footer -->
    <footer>
        <div class="social">
            <a href="#">Facebook</a>
            <a href="#">Instagram</a>
            <a href="#">Twitter</a>
            <a href="#">LinkedIn</a>
        </div>
        <p>© 2026 ProTech Solutions. All Rights Reserved.</p>
    </footer>

</body>
</html>
```
### CSS :
```
/* STEP 6: Global Styles */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: Arial, sans-serif;
}

body {
    background-color: #f4f4f4;
    color: #333;
    line-height: 1.6;
}

/* Header */
header {
    background: #1e1e2f;
    color: white;
    padding: 25px;
    text-align: center;
    letter-spacing: 1px;
}

/* Navigation */
nav {
    background: #333;
}

.nav-links {
    display: flex;   /* Flexbox */
    justify-content: center;
    list-style: none;
    flex-wrap: wrap;
}

.nav-links li {
    margin: 15px;
}

.nav-links a {
    color: white;
    text-decoration: none;
    padding: 8px 15px;
    transition: 0.3s;
}

.nav-links a:hover {
    background: #00adb5;
    border-radius: 5px;
}

/* Sections */
.section {
    padding: 60px 20px;
    text-align: center;
}

/* HERO SECTION */
.hero img {
    width: 100%;
    height: 350px;
    object-fit: cover;   /* Optimized image look */
    border-radius: 8px;
    margin-top: 20px;
}

/* Flexbox for products & services */
.flex-container {
    display: flex;
    justify-content: space-around;
    flex-wrap: wrap;
}

/* Cards */
.card {
    background: white;
    padding: 20px;
    margin: 15px;
    width: 250px;
    border-radius: 10px;
    box-shadow: 0 4px 10px rgba(0,0,0,0.1);
    transition: transform 0.3s, box-shadow 0.3s;
}

.card img {
    width: 100%;
    height: 180px;
    object-fit: cover;   /* Keeps image professional */
    border-radius: 10px;
}

.card:hover {
    transform: scale(1.05);
    box-shadow: 0 8px 18px rgba(0,0,0,0.2);
}

/* ABOUT SECTION FLEXBOX */
.about-flex {
    display: flex;
    justify-content: space-around;
    align-items: center;
    flex-wrap: wrap;
}

.about-text {
    width: 45%;
    text-align: left;
}

.about-image img {
    width: 350px;
    border-radius: 10px;
}

/* Form */
form {
    display: flex;
    flex-direction: column;
    align-items: center;
}

form input, form button {
    padding: 10px;
    margin: 10px;
    width: 250px;
}

form button {
    background: #00adb5;
    color: white;
    border: none;
    cursor: pointer;
    transition: 0.3s;
}

form button:hover {
    background: #007b7f;
}

/* Footer */
footer {
    background: #1e1e2f;
    color: white;
    text-align: center;
    padding: 20px;
}

.social a {
    color: #00adb5;
    margin: 10px;
    text-decoration: none;
    transition: 0.3s;
}

.social a:hover {
    text-decoration: underline;
}

/* RESPONSIVE DESIGN */
@media (max-width: 768px) {

    .about-text {
        width: 100%;
        text-align: center;
        margin-bottom: 20px;
    }

    .about-image img {
        width: 90%;
    }

    .flex-container {
        flex-direction: column;
        align-items: center;
    }

    .card {
        width: 80%;
    }
}
```


## OUTPUT
<img width="1920" height="1200" alt="Screenshot 2026-02-23 130817" src="https://github.com/user-attachments/assets/30875415-fb8b-497e-b2b0-305f62d480bb" />
<img width="1920" height="1200" alt="Screenshot 2026-02-23 130927" src="https://github.com/user-attachments/assets/cf98558e-2a9b-47bf-941d-a738fcbebb4f" />
<img width="1909" height="723" alt="Screenshot 2026-02-23 131016" src="https://github.com/user-attachments/assets/0faf9a95-3dfc-4a4c-bcea-625fa4dd8fa7" />





## RESULT
The program for creating commercial website using CSS Flexbox is executed successfully.
