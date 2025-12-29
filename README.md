<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Nurture & Create - Art Therapy for Your Pregnancy Journey</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Georgia', serif;
            line-height: 1.6;
            color: #333;
        }

        /* Header & Navigation */
        header {
            background: linear-gradient(135deg, #f8e8e8 0%, #e8d8d8 100%);
            padding: 1rem 0;
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 1000;
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
        }

        nav {
            max-width: 1200px;
            margin: 0 auto;
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 0 2rem;
        }

        .logo {
            font-size: 1.8rem;
            font-weight: bold;
            color: #d4698b;
        }

        nav ul {
            list-style: none;
            display: flex;
            gap: 2rem;
        }

        nav a {
            text-decoration: none;
            color: #555;
            transition: color 0.3s;
        }

        nav a:hover {
            color: #d4698b;
        }

        /* Hero Section */
        .hero {
            margin-top: 80px;
            background: linear-gradient(rgba(212, 105, 139, 0.1), rgba(232, 216, 216, 0.2)),
                        url('data:image/svg+xml,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1200 600"><rect fill="%23f8e8e8" width="1200" height="600"/></svg>');
            padding: 8rem 2rem;
            text-align: center;
        }

        .hero h1 {
            font-size: 3.5rem;
            color: #d4698b;
            margin-bottom: 1rem;
            line-height: 1.2;
        }

        .hero p {
            font-size: 1.3rem;
            color: #666;
            max-width: 700px;
            margin: 0 auto 2rem;
        }

        .cta-button {
            background: #d4698b;
            color: white;
            padding: 1.2rem 3rem;
            font-size: 1.2rem;
            border: none;
            border-radius: 50px;
            cursor: pointer;
            text-decoration: none;
            display: inline-block;
            transition: transform 0.3s, box-shadow 0.3s;
        }

        .cta-button:hover {
            transform: translateY(-3px);
            box-shadow: 0 10px 25px rgba(212, 105, 139, 0.3);
        }

        .price-tag {
            display: inline-block;
            background: #fff;
            padding: 0.5rem 1.5rem;
            border-radius: 30px;
            margin-top: 1rem;
            font-size: 1.5rem;
            color: #d4698b;
            font-weight: bold;
        }

        /* Features Section */
        .features {
            max-width: 1200px;
            margin: 4rem auto;
            padding: 0 2rem;
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 3rem;
        }

        .feature-card {
            background: white;
            padding: 2rem;
            border-radius: 15px;
            box-shadow: 0 5px 20px rgba(0,0,0,0.1);
            transition: transform 0.3s;
        }

        .feature-card:hover {
            transform: translateY(-10px);
        }

        .feature-card h3 {
            color: #d4698b;
            font-size: 1.8rem;
            margin-bottom: 1rem;
        }

        .feature-icon {
            font-size: 3rem;
            margin-bottom: 1rem;
        }

        /* Emotional Support Section */
        .emotional-support {
            background: linear-gradient(135deg, #f8e8e8 0%, #e8d8d8 100%);
            padding: 4rem 2rem;
            margin: 4rem 0;
        }

        .emotional-support h2 {
            text-align: center;
            color: #d4698b;
            font-size: 2.5rem;
            margin-bottom: 3rem;
        }

        .emotions-grid {
            max-width: 1000px;
            margin: 0 auto;
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 2rem;
        }

        .emotion-card {
            background: white;
            padding: 1.5rem;
            border-radius: 10px;
            text-align: center;
            box-shadow: 0 3px 15px rgba(0,0,0,0.1);
        }

        /* Trimester Section */
        .trimesters {
            max-width: 1200px;
            margin: 4rem auto;
            padding: 0 2rem;
        }

        .trimesters h2 {
            text-align: center;
            color: #d4698b;
            font-size: 2.5rem;
            margin-bottom: 3rem;
        }

        .trimester-container {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
            gap: 2rem;
        }

        .trimester-card {
            background: linear-gradient(135deg, #fff 0%, #f8e8e8 100%);
            padding: 2rem;
            border-radius: 15px;
            border-left: 5px solid #d4698b;
        }

        .trimester-card h3 {
            color: #d4698b;
            font-size: 2rem;
            margin-bottom: 1rem;
        }

        .trimester-card ul {
            list-style: none;
            padding-left: 0;
        }

        .trimester-card li {
            padding: 0.5rem 0;
            padding-left: 1.5rem;
            position: relative;
        }

        .trimester-card li:before {
            content: "🎨";
            position: absolute;
            left: 0;
        }

        /* Box Contents */
        .box-contents {
            background: white;
            max-width: 1200px;
            margin: 4rem auto;
            padding: 4rem 2rem;
        }

        .box-contents h2 {
            text-align: center;
            color: #d4698b;
            font-size: 2.5rem;
            margin-bottom: 3rem;
        }

        .contents-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 2rem;
        }

        .content-item {
            text-align: center;
            padding: 1.5rem;
        }

        .content-item h4 {
            color: #d4698b;
            margin-top: 1rem;
        }

        /* Footer */
        footer {
            background: #333;
            color: white;
            text-align: center;
            padding: 2rem;
            margin-top: 4rem;
        }

        @media (max-width: 768px) {
            .hero h1 {
                font-size: 2.5rem;
            }

            nav ul {
                flex-direction: column;
                gap: 1rem;
            }
        }
    </style>
</head>
<body>
    <header>
        <nav>
            <div class="logo">Nurture & Create</div>
            <ul>
                <li><a href="#home">Home</a></li>
                <li><a href="#about">About</a></li>
                <li><a href="#trimesters">Trimesters</a></li>
                <li><a href="#contents">What's Inside</a></li>
                <li><a href="#order">Order Now</a></li>
            </ul>
        </nav>
    </header>

    <section class="hero" id="home">
        <h1>Your Pregnancy Journey,<br>Through Art & Healing</h1>
        <p>A complete art therapy program designed to support you through every trimester. 
           Express, heal, and celebrate the beautiful transformation of motherhood.</p>
        <a href="#order" class="cta-button">Begin Your Journey</a>
        <div class="price-tag">Complete Kit: £150</div>
    </section>

    <section class="features">
        <div class="feature-card">
            <div class="feature-icon">📦</div>
            <h3>Complete Art Kit</h3>
            <p>Everything you need delivered to your door. Premium art supplies, guided journal, 
               and trimester-specific activities all included.</p>
        </div>
        <div class="feature-card">
            <div class="feature-icon">🤰</div>
            <h3>9-Month Journey</h3>
            <p>Structured activities for each trimester, designed by certified art therapists 
               and prenatal wellness experts.</p>
        </div>
        <div class="feature-card">
            <div class="feature-icon">💝</div>
            <h3>Emotional Support</h3>
            <p>Process anxiety, depression, body changes, and hormonal shifts through 
               therapeutic creative expression.</p>
        </div>
    </section>

    <section class="emotional-support">
        <h2>We Understand Your Journey</h2>
        <div class="emotions-grid">
            <div class="emotion-card">
                <h4>💙 Anxiety</h4>
                <p>Calm your mind through creative expression</p>
            </div>
            <div class="emotion-card">
                <h4>🌸 Depression</h4>
                <p>Find light in artistic healing</p>
            </div>
            <div class="emotion-card">
                <h4>💪 Body Image</h4>
                <p>Celebrate your changing form</p>
            </div>
            <div class="emotion-card">
                <h4>🌊 Hormonal Shifts</h4>
                <p>Ride the waves with grace</p>
            </div>
            <div class="emotion-card">
                <h4>✨ Transformation</h4>
                <p>Document your metamorphosis</p>
            </div>
            <div class="emotion-card">
                <h4>❤️ Self-Love</h4>
                <p>Nurture yourself as you nurture life</p>
            </div>
        </div>
    </section>

    <section class="trimesters" id="trimesters">
        <h2>Your Trimester-by-Trimester Guide</h2>
        <div class="trimester-container">
            <div class="trimester-card">
                <h3>First Trimester</h3>
                <p><strong>Weeks 1-13: New Beginnings</strong></p>
                <ul>
                    <li>Hope & Dreams Collage</li>
                    <li>Anxiety Release Watercolors</li>
                    <li>Morning Sickness Expression Journal</li>
                    <li>Body Gratitude Sketches</li>
                    <li>Fear & Excitement Mandala</li>
                    <li>Letter to Your Future Baby</li>
                </ul>
            </div>
            <div class="trimester-card">
                <h3>Second Trimester</h3>
                <p><strong>Weeks 14-27: Blossoming</strong></p>
                <ul>
                    <li>Energy Return Celebrations</li>
                    <li>Growing Belly Art</li>
                    <li>Connection & Bonding Paintings</li>
                    <li>Body Changes Acceptance Art</li>
                    <li>Nesting Instinct Vision Board</li>
                    <li>Self-Portrait Evolution</li>
                </ul>
            </div>
            <div class="trimester-card">
                <h3>Third Trimester</h3>
                <p><strong>Weeks 28-40: Preparing</strong></p>
                <ul>
                    <li>Birth Wishes Visualization</li>
                    <li>Strength & Power Symbols</li>
                    <li>Letting Go of Control Art</li>
                    <li>Motherhood Identity Exploration</li>
                    <li>Final Reflections Book</li>
                    <li>Welcome Baby Keepsake</li>
                </ul>
            </div>
        </div>
    </section>

    <section class="box-contents" id="contents">
        <h2>What's Inside Your Kit</h2>
        <div class="contents-grid">
            <div class="content-item">
                <div class="feature-icon">📖</div>
                <h4>Guided Art Therapy Journal</h4>
                <p>140-page hardcover book with prompts & activities</p>
            </div>
            <div class="content-item">
                <div class="feature-icon">🎨</div>
                <h4>Premium Art Supplies</h4>
                <p>Watercolors, acrylics, colored pencils, brushes</p>
            </div>
            <div class="content-item">
                <div class="feature-icon">📜</div>
                <h4>Canvas & Papers</h4>
                <p>Variety pack of textures and sizes</p>
            </div>
            <div class="content-item">
                <div class="feature-icon">✂️</div>
                <h4>Collage Materials</h4>
                <p>Magazines, stickers, decorative papers</p>
            </div>
            <div class="content-item">
                <div class="feature-icon">🖍️</div>
                <h4>Drawing Tools</h4>
                <p>Pastels, charcoal, markers, gel pens</p>
            </div>
            <div class="content-item">
                <div class="feature-icon">💌</div>
                <h4>Keepsake Items</h4>
                <p>Memory box, milestone cards, belly stickers</p>
            </div>
        </div>
    </section>

    <section class="hero" id="order" style="background: linear-gradient(135deg, #d4698b 0%, #c5577a 100%); color: white;">
        <h2 style="color: white;">Ready to Begin Your Healing Journey?</h2>
        <p style="color: white;">One complete kit. Nine months of support. A lifetime of memories.</p>
        <a href="#" class="cta-button" style="background: white; color: #d4698b;">Order Now - £150</a>
        <p style="margin-top: 2rem; font-size: 0.9rem;">Free UK Shipping • 30-Day Money-Back Guarantee</p>
    </section>

    <footer>
        <p>&copy; 2025 Nurture & Create. Supporting mothers through art therapy.</p>
        <p>Created with love for expecting mothers everywhere 💕</p>
    </footer>
</body>
</html>
