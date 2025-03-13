# Gym-Management
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Gym Management</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <header>
        <nav>
            <div class="logo">Gym<span>.</span></div>
            <ul>
                <li><a href="#">Home</a></li>
                <li><a href="#">Sign Up</a></li>
                <li><a href="#">Sign In</a></li>
                <li><a href="#">Contact Us</a></li>
                <li><a href="#">About Us</a></li>
            </ul>
        </nav>
    </header>

    <section class="hero">
        <h1>Train Like a Beast</h1>
    </section>

    <section class="features">
        <h2>FEATURE</h2>
        <div class="feature-container">
            <div class="feature-card">
                <img src="https://cdn-icons-png.flaticon.com/512/1041/1041976.png" alt="Weight Loss">
                <h3>Weight Loss</h3>
            </div>
            <div class="feature-card">
                <img src="https://cdn-icons-png.flaticon.com/512/1247/1247946.png" alt="Spinning Studio">
                <h3>Spinning Studio</h3>
            </div>
            <div class="feature-card">
                <img src="https://cdn-icons-png.flaticon.com/512/2424/2424690.png" alt="Personal Training">
                <h3>Personal Training</h3>
            </div>
        </div>
    </section>

    <section class="contact">
        <h2>Contact Us</h2>
        <p>Have questions? Reach out to us.</p>
        <form>
            <input type="text" placeholder="Enter Your Name" required>
            <input type="email" placeholder="Enter Your Email" required>
            <textarea placeholder="Enter Your Message" required></textarea>
            <button type="submit">SEND</button>
        </form>
    </section>

    <footer>
        <p>© 2025 Gym Management | All Rights Reserved</p>
    </footer>

    <script src="script.js"></script>
</body>
</html>





* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: 'Arial', sans-serif;
}

body {
    background: #111;
    color: white;
}

header {
    background: black;
    padding: 15px 20px;
}

nav {
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.logo {
    font-size: 24px;
    font-weight: bold;
    color: white;
}

.logo span {
    color: red;
}

nav ul {
    list-style: none;
    display: flex;
}

nav ul li {
    margin: 0 15px;
}

nav ul li a {
    color: white;
    text-decoration: none;
    font-size: 16px;
}

.hero {
    background: url('https://source.unsplash.com/1600x900/?gym,fitness') no-repeat center center/cover;
    height: 60vh;
    display: flex;
    align-items: center;
    justify-content: center;
    text-align: center;
}

.hero h1 {
    font-size: 50px;
    text-shadow: 2px 2px 10px rgba(0,0,0,0.7);
}

.features {
    text-align: center;
    padding: 50px 20px;
}

.feature-container {
    display: flex;
    justify-content: center;
    gap: 20px;
    margin-top: 20px;
}

.feature-card {
    background: #222;
    padding: 20px;
    border-radius: 10px;
    width: 200px;
    text-align: center;
}

.feature-card img {
    width: 50px;
    margin-bottom: 10px;
}

.contact {
    text-align: center;
    padding: 40px;
    background: #222;
}

.contact form {
    display: flex;
    flex-direction: column;
    align-items: center;
}

.contact input, .contact textarea {
    width: 80%;
    max-width: 400px;
    padding: 10px;
    margin: 10px 0;
    background: black;
    color: white;
    border: 1px solid white;
    border-radius: 5px;
}

.contact button {
    padding: 10px 20px;
    background: red;
    color: white;
    border: none;
    cursor: pointer;
    font-size: 16px;
}

footer {
    text-align: center;
    padding: 15px;
    background: black;
}





document.querySelector("form").addEventListener("submit", function(event) {
    event.preventDefault();
    alert("Your message has been sent successfully!");
});
