travel-agency-website/
├── index.html
├── styles/
│   └── style.css
├── scripts/
│   └── main.js
├── images/
│   └── (image files)
└── README.md
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Travel Agency</title>
    <link rel="stylesheet" href="styles/style.css">
</head>
<body>
    <header>
        <div class="logo">
            <h1>ExploreNow</h1>
        </div>
        <nav>
            <ul>
                <li><a href="#home">Home</a></li>
                <li><a href="#about">About</a></li>
                <li><a href="#services">Services</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
    </header>

    <section id="home">
        <div class="hero">
            <h2>Your Adventure Awaits</h2>
            <p>Discover the world's most beautiful destinations with us.</p>
            <button>Explore Now</button>
        </div>
    </section>

    <section id="about">
        <h2>About Us</h2>
        <p>ExploreNow is a travel agency committed to helping you discover the world's most stunning locations. With personalized services and unbeatable deals, we make your travel dreams a reality.</p>
    </section>

    <section id="services">
        <h2>Our Services</h2>
        <div class="service-list">
            <div class="service-item">
                <h3>Flight Booking</h3>
                <p>Get the best deals on domestic and international flights.</p>
            </div>
            <div class="service-item">
                <h3>Hotel Reservations</h3>
                <p>Choose from a wide range of accommodations to suit your budget.</p>
            </div>
            <div class="service-item">
                <h3>Customized Tours</h3>
                <p>Plan your trip exactly the way you want it.</p>
            </div>
        </div>
    </section>

    <section id="contact">
        <h2>Contact Us</h2>
        <form>
            <input type="text" placeholder="Your Name" required>
            <input type="email" placeholder="Your Email" required>
            <textarea placeholder="Your Message" required></textarea>
            <button type="submit">Submit</button>
        </form>
    </section>

    <footer>
        <p>&copy; 2024 ExploreNow. All Rights Reserved.</p>
    </footer>

    <script src="scripts/main.js"></script>
</body>
</html>
body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
}

header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    background-color: #333;
    color: #fff;
    padding: 1em 2em;
}

header .logo h1 {
    margin: 0;
}

nav ul {
    list-style: none;
    margin: 0;
    padding: 0;
    display: flex;
}

nav ul li {
    margin: 0 1em;
}

nav ul li a {
    color: #fff;
    text-decoration: none;
}

.hero {
    background: url('../images/hero.jpg') no-repeat center center/cover;
    color: #fff;
    text-align: center;
    padding: 5em 1em;
}

section {
    padding: 2em;
    text-align: center;
}

.service-list {
    display: flex;
    justify-content: space-around;
    margin-top: 1em;
}

.service-item {
    width: 30%;
    background-color: #f4f4f4;
    padding: 1em;
    border-radius: 5px;
}

footer {
    background-color: #333;
    color: #fff;
    text-align: center;
    padding: 1em 0;
}
// Example JavaScript to enhance functionality
document.querySelectorAll('nav ul li a').forEach(link => {
    link.addEventListener('click', event => {
        event.preventDefault();
        const target = document.querySelector(event.target.getAttribute('href'));
        window.scrollTo({
            top: target.offsetTop,
            behavior: 'smooth'
        });
    });
});
# Travel Agency Website

**ExploreNow** is a fictional travel agency website built to showcase the design and structure of a typical travel service platform.

## Features
- **Responsive Design** for desktop and mobile devices.
- **Navigation:** Easy-to-use menu with smooth scrolling.
- **Hero Section:** Attractive banner with a call-to-action.
- **Services Section:** List of travel-related services.
- **Contact Form:** Simple form for user inquiries.

## Technologies
- HTML
- CSS
- JavaScript

## How to Use
1. Clone the repository: `git clone https://github.com/yourusername/travel-agency-website.git`
2. Open `index.html` in a web browser.

## Screenshots
*(Include screenshots of the website if available)*

## License
This project is open-source and available under the MIT License.
