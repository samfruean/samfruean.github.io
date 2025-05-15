<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Simple GitHub Website</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <header>
        <h1>Welcome to My GitHub Page!</h1>
        <nav>
            <a href="#">Home</a>
            <a href="#">About</a>
            <a href="#">Contact</a>
        </nav>
    </header>

    <main>
        <section>
            <h2>About This Page</h2>
            <p>This is a simple website hosted on GitHub Pages. It's a great way to share your projects and ideas with the world!</p>
            <button onclick="sayHello()">Click Me</button>
        </section>
    </main>

    <footer>
        <p>&copy; 2025 My GitHub Site</p>
    </footer>

    <script src="script.js"></script>
</body>
</html>

body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
    background: #f4f4f4;
    color: #333;
}

header {
    background: #007acc;
    color: white;
    padding: 20px 0;
    text-align: center;
}

nav a {
    color: white;
    margin: 0 15px;
    text-decoration: none;
}

main {
    padding: 20px;
}

footer {
    background: #333;
    color: white;
    text-align: center;
    padding: 10px 0;
    position: fixed;
    width: 100%;
    bottom: 0;
}

function sayHello() {
    alert("Hello from your GitHub website!");
}
