# CSS Layouts and Responsive Design

## Objectives

Implement Flexbox and Grid for layout design.
Make the webpage responsive using media queries.
Ensure proper alignment and spacing.

## Instructions

- use Flexbox or CSS Grid.
- Add a navigation bar and structure the content.
- Use media queries to adjust layout for mobile, tablet, and desktop.

>[!NOTE]
>  - Include at least:
>  - navigation bar
>  - media queries

# Tasks

- Apply Flexbox or Grid for layout.
- Make the page responsive.
- Test across different screen sizes.

Happy Coding! 💻✨




<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Responsive Layout with Flexbox and Grid</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <header>
        <nav>
            <ul>
                <li><a href="#">Home</a></li>
                <li><a href="#">About</a></li>
                <li><a href="#">Services</a></li>
                <li><a href="#">Contact</a></li>
            </ul>
        </nav>
    </header>

    <main>
        <section class="hero">
            <h1>Welcome to Our Website!</h1>
            <p>We provide amazing services to help you succeed.</p>
        </section>

        <section class="content">
            <article class="card">
                <h2>Card 1</h2>
                <p>This is a card section with some content.</p>
            </article>
            <article class="card">
                <h2>Card 2</h2>
                <p>This is another card with content.</p>
            </article>
            <article class="card">
                <h2>Card 3</h2>
                <p>This card holds some interesting information.</p>
            </article>
        </section>
    </main>

    <footer>
        <p>&copy; 2025 Your Company. All Rights Reserved.</p>
    </footer>

    <script src="script.js"></script>
</body>
</html>


/* General Styles */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: Arial, sans-serif;
    line-height: 1.6;
    background-color: #f4f4f4;
}

header {
    background-color: #333;
    padding: 10px;
}

nav ul {
    list-style-type: none;
    display: flex;
    justify-content: center;
}

nav ul li {
    margin: 0 15px;
}

nav ul li a {
    color: white;
    text-decoration: none;
    font-size: 18px;
}

nav ul li a:hover {
    text-decoration: underline;
}

/* Hero Section */
.hero {
    text-align: center;
    background: #007bff;
    color: white;
    padding: 50px 20px;
}

/* Flexbox Layout for Content */
.content {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
    padding: 20px;
}

.card {
    background-color: white;
    border-radius: 8px;
    padding: 20px;
    margin: 10px;
    width: 30%;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
}

.card h2 {
    margin-bottom: 15px;
}

/* Footer */
footer {
    text-align: center;
    padding: 20px;
    background-color: #333;
    color: white;
}

/* Media Queries for Responsive Design */
@media (max-width: 768px) {
    /* Tablet */
    .content {
        flex-direction: column;
    }

    .card {
        width: 80%;
        margin: 10px auto;
    }

    nav ul {
        flex-direction: column;
    }

    nav ul li {
        margin-bottom: 10px;
    }
}

@media (max-width: 480px) {
    /* Mobile */
    .hero h1 {
        font-size: 24px;
    }

    .hero p {
        font-size: 16px;
    }

    .content {
        padding: 10px;
    }

    .card {
        width: 100%;
        margin: 5px 0;
    }
}



Explanation:
HTML:

The header contains a navigation bar with links to various sections.

The main section has a hero section with a title and description, followed by a content section with three cards.

The footer has copyright information.

CSS:

The page uses Flexbox for laying out the cards within the .content section. The cards are displayed in a row by default, and as the screen size reduces, they stack into columns.

Media Queries adjust the layout:

For screens smaller than 768px (tablets), the navigation bar switches to a vertical layout, and the cards become more compact and stack vertically.

For screens smaller than 480px (mobile), the card layout is set to full width, and the font size for the hero section is reduced for better readability on small devices.

Responsiveness:

The design is responsive across multiple devices (desktop, tablet, mobile) due to the use of media queries.

The content adjusts its layout based on the screen size using Flexbox and media queries for better user experience.




