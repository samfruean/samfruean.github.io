<html lang="en">
<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
    <title>Support for Kiwi Families</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            line-height: 1.6;
            margin: 0;
            padding: 0;
            background: #f4f4f4;
            color: #333;
        }

        header {
            background: #005c3c;
            color: white;
            padding: 20px;
            text-align: center;
        }

        nav {
            display: flex;
            flex-direction: column;
            align-items: center;
        }

        nav h1 {
            margin: 0;
            font-size: 2em;
        }

        .nav-links {
            list-style: none;
            padding: 0;
            display: flex;
            gap: 20px;
            margin: 10px 0 0;
        }

        .nav-links a {
            color: white;
            text-decoration: none;
        }

        .nav-links a:hover {
            text-decoration: underline;
        }

        .intro {
            margin-top: 10px;
            font-size: 1.1em;
        }

        main {
            padding: 20px;
            display: flex;
            flex-direction: column;
            gap: 20px;
        }

        section {
            background: white;
            padding: 15px;
            border-radius: 5px;
            box-shadow: 0 0 8px rgba(0, 0, 0, 0.05);
        }

        form {
            display: flex;
            flex-direction: column;
        }

        input, textarea {
            margin-bottom: 10px;
            padding: 8px;
            font-size: 1em;
            border: 1px solid #ccc;
            border-radius: 3px;
        }

        button {
            background: #005c3c;
            color: white;
            border: none;
            padding: 10px;
            cursor: pointer;
            border-radius: 3px;
            font-size: 1em;
        }

        button:hover {
            background: #003f2c;
        }

        footer {
            text-align: center;
            padding: 10px;
            background: #eee;
            margin-top: 20px;
        }

        figure {
            max-width: 300px;
            text-align: center;
        }

        figure img {
            width: 100%;
            border-radius: 5px;
        }

        @media (max-width: 600px) {
            .nav-links {
                flex-direction: column;
                gap: 10px;
            }

            .change-grid {
                flex-direction: column;
                align-items: center;
            }
        }
    </style>
</head>
<body>
    <header>
        <nav aria-label="Main navigation">
            <h1>Helping New Zealand Families</h1>
            <ul class="nav-links">
                <li><a href="#resources">Resources</a></li>
                <li><a href="#get-help">Get Help</a></li>
                <li><a href="#extra-support">More Support</a></li>
                <li><a href="#change-situation">Changing Your Situation</a></li>
            </ul>
        </nav>
        <p class="intro">Local support, resources, and guidance for whānau in need across Aotearoa.</p>
    </header>

    <main role="main">
        <section id="resources">
            <h2>Essential Resources</h2>
            <ul>
                <li><a href="https://www.workandincome.govt.nz/" target="_blank" rel="noopener">Work and Income (WINZ)</a></li>
                <li><a href="https://www.foodbank.co.nz/" target="_blank" rel="noopener">Food Banks NZ</a></li>
                <li><a href="https://mentalhealth.org.nz/" target="_blank" rel="noopener">Mental Health Foundation NZ</a></li>
            </ul>
        </section>

        <section id="get-help">
            <h2>Reach Out for Help</h2>
            <form action="https://formspree.io/f/YOUR_FORM_ID" method="POST" aria-label="Contact Form">
                <label for="name">Your Name:</label>
                <input type="text" id="name" name="name" required aria-required="true">

                <label for="email">Your Email:</label>
                <input type="email" id="email" name="_replyto" required aria-required="true">

                <label for="message">How can we help?</label>
                <textarea id="message" name="message" required aria-required="true"></textarea>

                <button type="submit">Submit</button>
            </form>
            <div id="confirmation" style="display:none;">Thank you for reaching out. We'll get back to you soon!</div>
        </section>

        <section id="extra-support">
            <h2>Additional NZ Services</h2>
            <ul>
                <li><a href="https://www.08004kids.org.nz/" target="_blank" rel="noopener">Oranga Tamariki – Child and Youth Wellbeing</a></li>
                <li><a href="https://www.lifeline.org.nz/" target="_blank" rel="noopener">Lifeline Aotearoa</a></li>
                <li><a href="https://www.hud.govt.nz/" target="_blank" rel="noopener">Ministry of Housing and Urban Development</a></li>
            </ul>
        </section>

        <section id="change-situation">
            <h2>How to Change Your Situation</h2>
            <div class="change-grid" style="display: flex; flex-wrap: wrap; gap: 20px; justify-content: center;">
                <figure>
                    <img src="images/assess.jpg" alt="Assessing situation">
                    <figcaption><strong>Step 1:</strong> Understand your current financial state.</figcaption>
                </figure>

                <figure>
                    <img src="images/help.jpg" alt="Getting help">
                    <figcaption><strong>Step 2:</strong> Reach out for immediate local assistance.</figcaption>
                </figure>

                <figure>
                    <img src="images/skills.jpg" alt="Building job skills">
                    <figcaption><strong>Step 3:</strong> Explore job training and upskilling options.</figcaption>
                </figure>

                <figure>
                    <img src="images/mental_health.jpg" alt="Mental health support">
                    <figcaption><strong>Step 4:</strong> Take care of your mental wellbeing.</figcaption>
                </figure>
            </div>
        </section>
    </main>

    <footer>
        <p>© 2025 Support for Kiwi Families. All rights reserved. | Aotearoa New Zealand</p>
    </footer>

    <script>
        // Simulate a confirmation message (demo purposes only)
        document.querySelector('form').addEventListener('submit', function (e) {
            e.preventDefault(); // Prevent actual submission for demo
            this.style.display = 'none';
            document.getElementById('confirmation').style.display = 'block';
        });
    </script>
</body>
</html>
