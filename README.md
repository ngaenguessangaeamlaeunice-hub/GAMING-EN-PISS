<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Gaming en Piste - Location PS5 à partir de 2000 FCFA. Livraison gratuite!">
    <meta name="keywords" content="PS5, PlayStation, location, gaming, Abidjan, Côte d'Ivoire">
    <title>Gaming en Piste - Location PS5</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background: linear-gradient(135deg, #0b0b16 0%, #1a1a2e 100%);
            color: #fff;
            line-height: 1.6;
            overflow-x: hidden;
        }

        /* 🎬 INTRO ANIMATION */
        .intro {
            position: fixed;
            width: 100%;
            height: 100%;
            background: #000;
            display: flex;
            justify-content: center;
            align-items: center;
            z-index: 999;
            animation: fadeOut 2.5s forwards;
        }

        .intro h1 {
            color: #00ffcc;
            font-size: clamp(24px, 8vw, 50px);
            animation: pulse 1s infinite;
            text-shadow: 0 0 20px #00ffcc;
        }

        @keyframes pulse {
            0%, 100% { transform: scale(1); }
            50% { transform: scale(1.15); }
        }

        @keyframes fadeOut {
            0% { opacity: 1; }
            80% { opacity: 1; }
            100% { opacity: 0; visibility: hidden; }
        }

        @keyframes slideInUp {
            from {
                opacity: 0;
                transform: translateY(30px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        /* HEADER */
        header {
            text-align: center;
            padding: 40px 20px;
            background: rgba(0, 255, 204, 0.05);
            border-bottom: 2px solid #00ffcc;
            animation: slideInUp 0.8s ease;
        }

        .logo {
            font-size: clamp(28px, 6vw, 40px);
            font-weight: bold;
            color: #00ffcc;
            letter-spacing: 3px;
            text-shadow: 0 0 15px #00ffcc;
            margin-bottom: 10px;
        }

        .tagline {
            color: #aaa;
            font-size: 14px;
            margin: 5px 0;
        }

        .highlight {
            color: #00ffcc;
            font-weight: bold;
            font-size: 18px;
        }

        .emoji {
            margin: 0 5px;
        }

        /* NAVIGATION MOBILE */
        nav {
            display: none;
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            background: #0b0b16;
            padding: 20px;
            z-index: 100;
        }

        nav.active {
            display: block;
        }

        nav ul {
            list-style: none;
        }

        nav li {
            margin: 15px 0;
        }

        nav a {
            color: #00ffcc;
            text-decoration: none;
            font-weight: bold;
            font-size: 18px;
        }

        .burger-menu {
            display: none;
            position: fixed;
            top: 20px;
            right: 20px;
            z-index: 101;
            cursor: pointer;
            flex-direction: column;
            gap: 6px;
        }

        .burger-menu span {
            width: 25px;
            height: 3px;
            background: #00ffcc;
            border-radius: 2px;
        }

        /* CONTAINER */
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 20px;
        }

        /* CARDS */
        .card {
            background: rgba(255, 255, 255, 0.08);
            border: 1px solid rgba(0, 255, 204, 0.3);
            padding: 25px;
            margin: 20px 0;
            border-radius: 15px;
            transition: all 0.3s ease;
            animation: slideInUp 0.8s ease forwards;
            backdrop-filter: blur(10px);
        }

        .card:nth-child(1) { animation-delay: 0.1s; }
        .card:nth-child(2) { animation-delay: 0.2s; }
        .card:nth-child(3) { animation-delay: 0.3s; }
        .card:nth-child(4) { animation-delay: 0.4s; }
        .card:nth-child(5) { animation-delay: 0.5s; }

        .card h2 {
            color: #00ffcc;
            font-size: 24px;
            margin-bottom: 15px;
            text-shadow: 0 0 10px rgba(0, 255, 204, 0.5);
        }

        .card:hover {
            transform: translateY(-10px);
            background: rgba(0, 255, 204, 0.15);
            border-color: #00ffcc;
            box-shadow: 0 10px 30px rgba(0, 255, 204, 0.2);
        }

        .card p {
            color: #ddd;
            margin: 10px 0;
            font-size: 15px;
        }

        .price {
            font-size: 18px;
            color: #00ffcc;
            font-weight: bold;
        }

        /* BUTTONS */
        .btn {
            display: inline-block;
            padding: 15px 30px;
            background: linear-gradient(135deg, #00ffcc 0%, #00d9a3 100%);
            color: #000;
            border-radius: 50px;
            text-decoration: none;
            font-weight: bold;
            transition: all 0.3s ease;
            border: none;
            cursor: pointer;
            font-size: 16px;
            box-shadow: 0 5px 15px rgba(0, 255, 204, 0.3);
            margin-top: 15px;
        }

        .btn:hover {
            background: linear-gradient(135deg, #00fff5 0%, #00ffcc 100%);
            transform: scale(1.08);
            box-shadow: 0 8px 25px rgba(0, 255, 204, 0.5);
        }

        .btn:active {
            transform: scale(0.95);
        }

        /* WHATSAPP BUTTON */
        .whatsapp {
            position: fixed;
            bottom: 30px;
            right: 30px;
            background: #25D366;
            color: white;
            padding: 18px 22px;
            border-radius: 50px;
            text-decoration: none;
            font-weight: bold;
            box-shadow: 0 5px 20px rgba(37, 211, 102, 0.4);
            transition: all 0.3s ease;
            z-index: 50;
            font-size: 18px;
        }

        .whatsapp:hover {
            background: #1ead47;
            transform: scale(1.1);
            box-shadow: 0 8px 30px rgba(37, 211, 102, 0.6);
        }

        /* RATING */
        .rating {
            color: #ffc107;
            font-size: 16px;
            margin: 10px 0;
        }

        /* TESTIMONIALS */
        .testimonials {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 20px;
            margin-top: 20px;
        }

        .testimonial {
            background: rgba(0, 255, 204, 0.1);
            padding: 20px;
            border-radius: 10px;
            border-left: 4px solid #00ffcc;
        }

        .testimonial p {
            font-style: italic;
            color: #ccc;
        }

        .testimonial-author {
            color: #00ffcc;
            font-weight: bold;
            margin-top: 10px;
        }

        /* FOOTER */
        footer {
            text-align: center;
            padding: 30px;
            background: #0a0a14;
            border-top: 2px solid #00ffcc;
            margin-top: 40px;
            color: #999;
            font-size: 14px;
        }

        /* RESPONSIVE */
        @media (max-width: 768px) {
            .burger-menu {
                display: flex;
            }

            .logo {
                font-size: 28px;
            }

            .card {
                padding: 20px;
            }

            .whatsapp {
                bottom: 20px;
                right: 20px;
                padding: 15px 18px;
                font-size: 16px;
            }

            .testimonials {
                grid-template-columns: 1fr;
            }
        }

        @media (max-width: 480px) {
            header {
                padding: 20px 15px;
            }

            .logo {
                font-size: 22px;
            }

            .container {
                padding: 15px;
            }

            .card {
                padding: 15px;
                margin: 15px 0;
            }

            .btn {
                width: 100%;
                text-align: center;
            }
        }

        /* GLOW EFFECT */
        .glow {
            text-shadow: 0 0 10px #00ffcc, 0 0 20px #00ffcc;
        }
    </style>
</head>

<body>

    <!-- 🎬 INTRO ANIMATION -->
    <div class="intro">
        <h1>🎮 GAMING EN PISTE</h1>
    </div>

    <!-- BURGER MENU (Mobile) -->
    <div class="burger-menu" id="burgerMenu">
        <span></span>
        <span></span>
        <span></span>
    </div>

    <!-- NAVIGATION -->
    <nav id="navMenu">
        <ul>
            <li><a href="#services">Services</a></li>
            <li><a href="#pricing">Tarifs</a></li>
            <li><a href="#about">À propos</a></li>
            <li><a href="#contact">Contact</a></li>
        </ul>
    </nav>

    <!-- HEADER -->
    <header>
        <div class="logo glow">🎮 GAMING EN PISTE</div>
        <p class="tagline">✨ La meilleure location PS5 en Côte d'Ivoire</p>
        <p class="tagline"><span class="highlight">À partir de 2000 FCFA</span></p>
        <p class="tagline">🚚 Livraison gratuite | 💰 Paiement à la livraison</p>
    </header>

    <!-- MAIN CONTENT -->
    <div class="container">

        <!-- SÉANCES JOUR -->
        <div class="card">
            <h2>☀️ Séances Jour</h2>
            <p><span class="price">5 000 FCFA / 2h</span> → 1 console + 2 manettes</p>
            <p><span class="price">8 000 FCFA / 2h</span> → 1 console + 4 manettes</p>
            <p class="rating">⭐⭐⭐⭐⭐ (127 avis)</p>
            <a class="btn" href="https://wa.me/2250713806258" target="_blank">📲 Réserver une séance jour</a>
        </div>

        <!-- SÉANCES NUIT -->
        <div class="card">
            <h2>🌙 Séances Nuit</h2>
            <p><span class="price">40 000 FCFA / 9h</span> → 4 joueurs maximum</p>
            <p>21h15 - 07h15 (Sans interruption)</p>
            <p class="rating">⭐⭐⭐⭐⭐ (89 avis)</p>
            <a class="btn" href="https://wa.me/2250713806258" target="_blank">🌙 Réserver une soirée gaming</a>
        </div>

        <!-- HORAIRES -->
        <div class="card">
            <h2>⏰ Horaires d'Ouverture</h2>
            <p>📍 <strong>Jour :</strong> 08h00 - 21h15</p>
            <p>📍 <strong>Nuit :</strong> 21h15 - 07h15</p>
            <p>📞 Support 24h/24 sur WhatsApp</p>
        </div>

        <!-- AVANTAGES -->
        <div class="card">
            <h2>🎁 Nos Avantages</h2>
            <p>✅ Consoles dernière génération (PS5 Standard)</p>
            <p>✅ Jeux AAA disponibles (FIFA, 2K, COD, etc.)</p>
            <p>✅ Livraison rapide (max 30 min)</p>
            <p>✅ Équipement impeccable & hygiénique</p>
            <p>✅ Support client réactif</p>
        </div>

        <!-- RÉSERVATION -->
        <div class="card">
            <h2>🚀 Réservation Rapide</h2>
            <p>Cliquez ci-dessous pour réserver directement sur WhatsApp</p>
            <p style="color: #aaa; font-size: 13px;">⏱️ Réponse garantie en moins de 5 minutes</p>
            <a class="btn" href="https://wa.me/2250713806258" target="_blank">
                📲 RÉSERVER MAINTENANT
            </a>
        </div>

        <!-- TÉMOIGNAGES -->
        <div class="card">
            <h2>💬 Ce que disent nos clients</h2>
            <div class="testimonials">
                <div class="testimonial">
                    <p>"Service impeccable! Les consoles sont en excellent état. Je recommande vivement!"</p>
                    <div class="testimonial-author">— Kofi M. ⭐⭐⭐⭐⭐</div>
                </div>
                <div class="testimonial">
                    <p>"Livraison ultra rapide et équipe très professionnelle. À louer sans hésiter!"</p>
                    <div class="testimonial-author">— Ama K. ⭐⭐⭐⭐⭐</div>
                </div>
                <div class="testimonial">
                    <p>"Meilleur prix du marché avec une qualité irréprochable. C'est du sérieux!"</p>
                    <div class="testimonial-author">— Yves P. ⭐⭐⭐⭐⭐</div>
                </div>
            </div>
        </div>

    </div>

    <!-- WHATSAPP BUTTON -->
    <a class="whatsapp" href="https://wa.me/2250713806258" target="_blank" title="Contactez-nous sur WhatsApp">
        📞 WhatsApp
    </a>

    <!-- FOOTER -->
    <footer>
        <p>&copy; 2026 Gaming en Piste - Location PS5 | Tous droits réservés</p>
        <p>📍 Abidjan, Côte d'Ivoire | 📞 +225 07 13 80 62 58</p>
    </footer>

    <script>
        // Mobile Menu Toggle
        const burgerMenu = document.getElementById('burgerMenu');
        const navMenu = document.getElementById('navMenu');

        burgerMenu.addEventListener('click', () => {
            navMenu.classList.toggle('active');
        });

        // Close menu when link is clicked
        document.querySelectorAll('nav a').forEach(link => {
            link.addEventListener('click', () => {
                navMenu.classList.remove('active');
            });
        });

        // Smooth scroll
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                const target = document.querySelector(this.getAttribute('href'));
                if (target) {
                    target.scrollIntoView({ behavior: 'smooth' });
                }
            });
        });
    </script>

</body>
</html>
