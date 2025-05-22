<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Support for Families</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <header>
        <h1>Helping Struggling Families</h1>
        <p>Resources, support, and connection for families in need.</p>
    </header>

    <main>
        <section>
            <h2>Resources</h2>
            <ul>
                <li><a href="https://www.feedingamerica.org/">Food Assistance</a></li>
                <li><a href="https://www.benefits.gov/">Financial Support</a></li>
                <li><a href="https://www.mentalhealth.gov/">Mental Health Services</a></li>
            </ul>
        </section>

        <section>
            <h2>Get Help</h2>
            <form action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
                <label for="name">Your Name:</label>
                <input type="text" id="name" name="name" required>

                <label for="email">Your Email:</label>
                <input type="email" id="email" name="_replyto" required>

                <label for="message">How can we help?</label>
                <textarea id="message" name="message" required></textarea>

                <button type="submit">Submit</button>
            </form>
        </section>
    </main>

    <footer>
        <p>© 2025 Support for Families. All rights reserved.</p>
    </footer>
</body>
</html>

body {
    font-family: Arial, sans-serif;
    line-height: 1.6;
    margin: 0;
    padding: 0;
    background: #f4f4f4;
    color: #333;
}

header {
    background: #006699;
    color: white;
    padding: 20px;
    text-align: center;
}

main {
    padding: 20px;
}

section {
    margin-bottom: 20px;
    background: white;
    padding: 15px;
    border-radius: 5px;
}

form {
    display: flex;
    flex-direction: column;
}

input, textarea {
    margin-bottom: 10px;
    padding: 8px;
    font-size: 1em;
}

button {
    background: #006699;
    color: white;
    border: none;
    padding: 10px;
    cursor: pointer;
}

button:hover {
    background: #004466;
}

footer {
    text-align: center;
    padding: 10px;
    background: #eee;
}


