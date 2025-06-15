<!DOCTYPE html>
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
                    <img src="images/assess.jpg" alt="Assessing situation" />
                    <figcaption><strong>Step 1:</strong> Understand your current financial state.</figcaption>
                </figure>

                <figure>
                    <img src="images/help.jpg" alt="Getting help" />
                    <figcaption><strong>Step 2:</strong> Reach out for immediate local assistance.</figcaption>
                </figure>

                <figure>
                    <img src="images/skills.jpg" alt="Building job skills" />
                    <figcaption><strong>Step 3:</strong> Explore job training and upskilling options.</figcaption>
                </figure>

                <figure>
                    <img src="images/mental_health.jpg" alt="Mental health support" />
                    <figcaption><strong>Step 4:</strong> Take care of your mental wellbeing.</figcaption>
                </figure>
            </div>
        </section>

        <!-- Added Food Assistance Section -->
        <section id="food-assistance">
            <h2>Food Assistance in Auckland</h2>
            <p>Find support from local food banks and community organizations in the Auckland region:</p>
            <ul>
                <li><strong>Auckland City Mission</strong> – 15 Auburn Street, Grafton. Call <a href="tel:093039266">09 303 9266</a> to arrange a food parcel. Visit: <a href="https://www.taikura.org.nz/food-deliveries-packed-meals-foodbanks-and-food-parcels/" target="_blank" rel="noopener">taikura.org.nz</a></li>

                <li><strong>St Vincent de Paul Society of Auckland</strong> – Foodbank in Newton and South Auckland. Call <a href="tel:098156122">09 815 6122</a> or use the <a href="https://svdpak.org.nz/svdpak/need-food-support/" target="_blank" rel="noopener">online request form</a>.</li>

                <li><strong>KiwiHarvest</strong> – Supports food redistribution to other charities. More info: <a href="https://www.kiwiharvest.org.nz/receive-food" target="_blank" rel="noopener">kiwiharvest.org.nz</a></li>

                <li><strong>The Fono</strong> – Provides support for Pasifika families. Call <a href="tel:0800366648">0800 FONO4U (0800 366 648)</a>.</li>

                <li><strong>Manukau Urban Māori Authority (MUMA)</strong> – Food parcels for South Auckland. Call <a href="tel:0800686232">0800 686 232</a> (Weekdays 9:30am–1:30pm).</li>

                <li><strong>Salvation Army</strong> – Mt Wellington branch: <a href="tel:093797615">09 379 7615</a> or national helpline: <a href="tel:0800530000">0800 53 0000</a>. Arrange a food parcel ahead of time.</li>

                <li><strong>Papakura Marae</strong> – Delivers to Papakura & Manurewa. Call <a href="tel:092972036">09 297 2036</a>.</li>

                <li><strong>Sunday Blessings</strong> – Free meals on Sunday evenings at Ellen Melville Centre (2 Freyberg Place, Auckland Central). Visit: <a href="https://www.sundayblessings.co.nz/" target="_blank" rel="noopener">sundayblessings.co.nz</a></li>

                <li><strong>FoodTogether</strong> – Affordable fresh produce across Auckland. Visit: <a href="https://www.foodtogether.co.nz/" target="_blank" rel="noopener">foodtogether.co.nz</a></li>
            </ul>
            <p><em>Note:</em> Most services require photo ID and proof of address. Contact providers directly for eligibility and hours.</p>
        </section>

        <!-- Added Financial Assistance Section -->
        <section id="financial-assistance">
            <h2>Pathways Out of Poverty: Achieving Financial Success</h2>
            <p>Poverty is more than lack of money — it's about opportunity, access, and support. Here's a 10-step roadmap to help your whānau gain financial stability in Aotearoa:</p>
            <ol>
                <li>
                    <strong>Understand Your Financial Situation</strong><br>
                    Track all income, expenses, and debts. Use tools like <a href="https://sorted.org.nz/tools/budgeting-tool" target="_blank" rel="noopener">Sorted Budget Tool</a> to find out where you stand and what needs changing.
                </li>
                <li>
                    <strong>Create a Survival Budget, Then a Growth Budget</strong><br>


    
        
