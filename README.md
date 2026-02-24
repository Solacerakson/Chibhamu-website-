<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CHIBAMU ENTERPRISE | Multi-Industry Solutions</title>
    <style>
        /* --- RESET & VARIABLES --- */
        :root {
            --primary-color: #2c3e50; /* Dark Blue */
            --accent-color: #27ae60;  /* Green for Farming/Freshness */
            --secondary-color: #e67e22; /* Orange for Butchery/Action */
            --light-bg: #f4f7f6;
            --white: #ffffff;
            --text-dark: #333;
            --text-light: #666;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }

        body {
            line-height: 1.6;
            color: var(--text-dark);
            background-color: var(--light-bg);
        }

        a { text-decoration: none; color: inherit; }
        ul { list-style: none; }

        /* --- HEADER --- */
        header {
            background: var(--primary-color);
            color: var(--white);
            padding: 1rem 5%;
            display: flex;
            justify-content: space-between;
            align-items: center;
            position: sticky;
            top: 0;
            z-index: 1000;
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
        }

        .logo {
            font-size: 1.5rem;            font-weight: bold;
            text-transform: uppercase;
            letter-spacing: 2px;
        }
        
        .logo span { color: var(--accent-color); }

        nav ul {
            display: flex;
            gap: 20px;
        }

        nav a:hover {
            color: var(--accent-color);
            transition: 0.3s;
        }

        /* --- HERO SECTION --- */
        .hero {
            background: linear-gradient(rgba(0,0,0,0.6), rgba(0,0,0,0.6)), url('https://images.unsplash.com/photo-1486406146926-c627a92ad1ab?ixlib=rb-1.2.1&auto=format&fit=crop&w=1350&q=80');
            background-size: cover;
            background-position: center;
            height: 80vh;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            text-align: center;
            color: var(--white);
            padding: 0 20px;
        }

        .hero h1 {
            font-size: 3rem;
            margin-bottom: 1rem;
        }

        .hero p {
            font-size: 1.2rem;
            max-width: 600px;
            margin-bottom: 2rem;
        }

        .btn {
            padding: 12px 30px;
            background: var(--accent-color);
            color: var(--white);
            border-radius: 5px;
            font-weight: bold;
            transition: 0.3s;        }

        .btn:hover { background: #219150; }

        /* --- SECTIONS GENERAL --- */
        .section-title {
            text-align: center;
            margin: 4rem 0 2rem;
            font-size: 2.5rem;
            color: var(--primary-color);
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }

        /* --- DIVISIONS GRID --- */
        .divisions-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
            margin-bottom: 4rem;
        }

        .card {
            background: var(--white);
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
            transition: transform 0.3s ease;
        }

        .card:hover {
            transform: translateY(-5px);
        }

        .card-img {
            height: 200px;
            width: 100%;
            object-fit: cover;
        }

        .card-content {
            padding: 20px;
        }

        .card-title {
            font-size: 1.4rem;            margin-bottom: 10px;
            color: var(--primary-color);
            border-bottom: 2px solid var(--accent-color);
            display: inline-block;
            padding-bottom: 5px;
        }

        .card-list {
            margin-top: 15px;
            color: var(--text-light);
        }

        .card-list li {
            margin-bottom: 5px;
            padding-left: 15px;
            position: relative;
        }

        .card-list li::before {
            content: "•";
            color: var(--accent-color);
            position: absolute;
            left: 0;
            font-weight: bold;
        }

        /* --- SPECIFIC CARD STYLES --- */
        .card.transport .card-title { border-color: #3498db; }
        .card.retail .card-title { border-color: #e74c3c; }
        .card.farming .card-title { border-color: #27ae60; }
        .card.realestate .card-title { border-color: #8e44ad; }

        /* --- FOOTER --- */
        footer {
            background: var(--primary-color);
            color: var(--white);
            padding: 3rem 5%;
            margin-top: 4rem;
        }

        .footer-content {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 40px;
        }

        .footer-col h3 {
            margin-bottom: 15px;
            color: var(--accent-color);
        }
        .copyright {
            text-align: center;
            margin-top: 2rem;
            padding-top: 2rem;
            border-top: 1px solid rgba(255,255,255,0.1);
            font-size: 0.9rem;
        }

        /* --- RESPONSIVE --- */
        @media (max-width: 768px) {
            header { flex-direction: column; gap: 15px; }
            .hero h1 { font-size: 2rem; }
        }
    </style>
</head>
<body>

    <!-- Header -->
    <header>
        <div class="logo">Chibamu <span>Enterprises</span></div>
        <nav>
            <ul>
                <li><a href="#home">Home</a></li>
                <li><a href="#divisions">Our Divisions</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
    </header>

    <!-- Hero Section -->
    <section id="home" class="hero">
        <h1>Building a Better Future</h1>
        <p>From the farm to the table, and from the road to your home. We are a diversified group committed to quality and service excellence.</p>
        <a href="#divisions" class="btn">Explore Our Businesses</a>
    </section>

    <!-- Main Divisions Section -->
    <section id="divisions" class="container">
        <h2 class="section-title">Our Business Divisions</h2>
        
        <div class="divisions-grid">

            <!-- 1. Retail & Shops -->
            <div class="card retail">
                <img src="https://images.unsplash.com/photo-1578916171728-46686eac8d58?ixlib=rb-1.2.1&auto=format&fit=crop&w=800&q=80" alt="Supermarket" class="card-img">
                <div class="card-content">
                    <h3 class="card-title">Retail & Shops</h3>
                    <p>Your one-stop destination for daily essentials. We operate modern retail outlets stocked with high-quality goods.</p>
                    <ul class="card-list">                        <li>Groceries & Household Items</li>
                        <li>Electronics & Appliances</li>
                        <li>Fresh Produce Section</li>
                    </ul>
                </div>
            </div>

            <!-- 2. Butchery -->
            <div class="card butchery">
                <img src="https://images.unsplash.com/photo-1607623814075-e51df1bdc82f?ixlib=rb-1.2.1&auto=format&fit=crop&w=800&q=80" alt="Butchery" class="card-img">
                <div class="card-content">
                    <h3 class="card-title">Zveipapo Butchery</h3>
                    <p>Providing the freshest cuts of meat. We adhere to strict hygiene standards to serve our community.</p>
                    <ul class="card-list">
                        <li>Fresh Beef, Pork & Chicken</li>
                        <li>Processed Meats & Sausages</li>
                        <li>Custom Cuts & Marinated Meats</li>
                    </ul>
                </div>
            </div>

            <!-- 3. Farming -->
            <div class="card farming">
                <img src="https://images.unsplash.com/photo-1625246333195-f81961856161?ixlib=rb-1.2.1&auto=format&fit=crop&w=800&q=80" alt="Farming" class="card-img">
                <div class="card-content">
                    <h3 class="card-title">Agriculture & Farming</h3>
                    <p>Sustainable farming practices to feed the nation. We specialize in both crop production and livestock rearing.</p>
                    <ul class="card-list">
                        <li>Commercial Crop Production</li>
                        <li>Dairy & Poultry Farming</li>
                        <li>Organic Fertilizers</li>
                    </ul>
                </div>
            </div>

            <!-- 4. Transport -->
            <div class="card transport">
                <img src="https://images.unsplash.com/photo-1544620347-c4fd4a3d5957?ixlib=rb-1.2.1&auto=format&fit=crop&w=800&q=80" alt="Transport" class="card-img">
                <div class="card-content">
                    <h3 class="card-title">Transport & Logistics</h3>
                    <p>Moving people and goods safely and efficiently across the region. We offer a full spectrum of transport solutions.</p>
                    <ul class="card-list">
                        <li><strong>Passenger:</strong> Luxury Buses & Commuter Omnibus</li>
                        <li><strong>Freight:</strong> Heavy Duty Trucks & Logistics</li>
                        <li>Door-to-Door Delivery Services</li>
                    </ul>
                </div>
            </div>

            <!-- 5. Real Estate -->            <div class="card realestate">
                <img src="https://images.unsplash.com/photo-1564013799919-ab600027ffc6?ixlib=rb-1.2.1&auto=format&fit=crop&w=800&q=80" alt="Houses" class="card-img">
                <div class="card-content">
                    <h3 class="card-title">Houses & Lodges</h3>
                    <p>Quality accommodation and property development. Whether you need a home or a holiday getaway.</p>
                    <ul class="card-list">
                        <li>Residential House Rentals & Sales</li>
                        <li>Comfortable Lodges & Guest Houses</li>
                        <li>Property Management Services</li>
                    </ul>
                </div>
            </div>

        </div>
    </section>

    <!-- Footer -->
    <footer id="contact">
        <div class="footer-content">
            <div class="footer-col">
                <h3>Shumba Zveipapo</h3>
                <p>Empowering the community through diverse business solutions. Quality, Integrity, and Service.</p>
            </div>
            <div class="footer-col">
                <h3>Contact Us</h3>
                <p>📍 14 Ruargo farm Arcturus ,Arcturus Road</p>
                <p>📞 +123 456 7890</p>
                <p>✉️ info@chibhamuenterpisies.com</p>
            </div>
            <div class="footer-col">
                <h3>Quick Links</h3>
                <ul>
                    <li><a href="#">Book a Bus Ticket</a></li>
                    <li><a href="#7>View House Listings</a></li>
                    <li><a href="#">Order Meat Online</a></li>
                </ul>
            </div>
        </div>
        <div class="copyright">
            <p>&copy; 2026 Chibhamu Enterprises . solacetk@gmail.com All Rights Reserved.</p>
        </div>
    </footer>

</body>
</html>
