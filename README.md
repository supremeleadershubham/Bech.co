<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Bech. Co - Marketing Agency</title>
    <style>
        body {
            margin: 0;
            font-family: "Segoe UI", Roboto, sans-serif;
            color: #d0f0c0;
            text-align: center;
            min-height: 100vh;
            position: relative;
            background-color: #0d0d0d;
        }

        /* Background watermarks */
        body::before {
            content: "";
            background: url('db738d1a519b8af43dea7ea2a9e1b15e.jpg') no-repeat center center;
            background-size: cover;
            opacity: 0.12;
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 50%;
            z-index: -1;
        }

        body::after {
            content: "";
            background: url('MoonSwatch-With-Camera.webp') no-repeat center center;
            background-size: cover;
            opacity: 0.12;
            position: fixed;
            bottom: 0;
            left: 0;
            width: 100%;
            height: 50%;
            z-index: -1;
        }

        header {
            padding: 60px 20px 20px 20px;
        }

        header h1 {
            margin: 0;
            font-size: 44px;
            font-weight: 600;
            letter-spacing: 2px;
            color: #245c2a; /* darker green */
            text-shadow: 0 2px 4px rgba(0,0,0,0.7);
        }

        nav {
            margin: 20px 0;
        }

        button {
            margin: 10px;
            padding: 12px 28px;
            background: linear-gradient(145deg, #1b3f1f, #245c2a);
            color: #f0f0f0;
            font-weight: 500;
            font-size: 16px;
            border: none;
            border-radius: 30px;
            cursor: pointer;
            transition: all 0.3s ease;
            box-shadow: 0 4px 10px rgba(0,0,0,0.4);
        }

        button:hover {
            background: linear-gradient(145deg, #245c2a, #2f7a36);
            transform: translateY(-2px);
        }

        section {
            max-width: 750px;
            margin: 30px auto;
            color: #e6e6e6;
            line-height: 1.6;
            background: rgba(20, 20, 20, 0.6);
            padding: 25px;
            border-radius: 15px;
            box-shadow: 0 6px 20px rgba(0,0,0,0.5);
            backdrop-filter: blur(8px);
            display: none; /* hidden until clicked */
            animation: fadeIn 0.6s ease forwards;
            text-align: left;
        }

        section h2 {
            color: #2f7a36;
            text-align: center;
        }

        ul.client-list {
            list-style: none;
            padding: 0;
            text-align: center;
        }

        ul.client-list li {
            margin: 8px 0;
            font-size: 18px;
            font-weight: 500;
            color: #d9ead3;
        }

        .work-gallery {
            text-align: center;
            margin-top: 20px;
        }

        .work-gallery img {
            max-width: 100%;
            height: auto;
            border-radius: 12px;
            margin: 10px 0;
            box-shadow: 0 6px 15px rgba(0,0,0,0.6);
            transition: transform 0.3s ease;
        }

        .work-gallery img:hover {
            transform: scale(1.05);
        }

        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(20px); }
            to { opacity: 1; transform: translateY(0); }
        }

        /* Home section is always visible by default */
        #home {
            display: block;
        }
    </style>
</head>
<body>
    <header>
        <h1>Bech. Co</h1>
        <p>Your trusted marketing agency for promotional activities and brand growth.</p>
    </header>

    <nav>
        <button onclick="showSection('home')">Home</button>
        <button onclick="showSection('about')">About Us</button>
        <button onclick="showSection('clients')">Clients</button>
        <button onclick="showSection('work')">Our Work</button>
    </nav>

    <!-- Home Section -->
    <section id="home">
        <h2>Welcome to Bech. Co</h2>
        <p>We connect brands with creative freelancers to deliver impactful promotional campaigns through photography, videography, and influencer-driven marketing.</p>
    </section>

    <!-- About Section -->
    <section id="about">
        <h2>About Us</h2>
        <p>
            Bech.co is a dynamic platform dedicated to revolutionizing how businesses scale their reach and how skilled individuals monetize their influence. 
            We seamlessly connect companies with a vetted network of freelance product promoters and brand advocates ready to drive targeted awareness and sales. 
            Our mission is to dismantle traditional marketing barriers by providing a transparent, efficient, and performance-driven marketplace where companies 
            can easily find the perfect voice for their product, and promoters can connect with impactful, relevant opportunities. 
            At Bech.co, we're not just a connector; we're building the future of decentralized, results-focused marketing.
        </p>
    </section>

    <!-- Clients Section -->
    <section id="clients">
        <h2>Our Clients</h2>
        <p>We’ve proudly collaborated with leading brands across industries, including:</p>
        <ul class="client-list">
            <li>✔ Titan</li>
            <li>✔ Tanishq</li>
            <li>✔ Rolex</li>
            <li>✔ Jacob & Co.</li>
            <li>✔ Omega</li>
            <li>✔ Hublot</li>
        </ul>
    </section>

    <!-- Our Work Section -->
    <section id="work">
        <h2>Our Work</h2>
        <p>From jewelry showcases to luxury watch promotions, our creative campaigns blend aesthetics with strategy to drive measurable results.</p>
        <div class="work-gallery">
            <img src="Rolex-watches-for-man-Australia_480x480.webp" alt="Rolex Watch Campaign">
        </div>
    </section>

    <script>
        function showSection(id) {
            document.querySelectorAll("section").forEach(sec => sec.style.display = "none");
            document.getElementById(id).style.display = "block";
        }
    </script>
</body>
</html>
