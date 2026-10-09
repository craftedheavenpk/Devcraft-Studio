<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>DevCraft Studio - Website Development & Digital Solutions</title>
    <style>
        :root {
            --primary: #0F172A;
            --secondary: #D4AF37;
            --accent: #1E293B;
            --text-light: #F8FAFC;
            --text-dark: #334155;
            --bg-light: #F1F5F9;
        }
        * { margin: 0; padding: 0; box-sizing: border-box; font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif; }
        body { background-color: var(--bg-light); color: var(--text-dark); line-height: 1.6; }
        
        header { background: var(--primary); color: var(--text-light); padding: 1rem 5%; display: flex; justify-content: space-between; align-items: center; position: sticky; top: 0; z-index: 1000; box-shadow: 0 4px 6px rgba(0,0,0,0.1); }
        .logo-area h2 { color: var(--secondary); font-size: 1.5rem; letter-spacing: 1px; }
        nav { display: flex; gap: 15px; flex-wrap: wrap; }
        nav a { color: var(--text-light); text-decoration: none; font-weight: 500; font-size: 0.9rem; transition: 0.3s; }
        nav a:hover { color: var(--secondary); }

        .hero { background: linear-gradient(135deg, var(--primary), var(--accent)); color: var(--text-light); padding: 4rem 5%; display: flex; align-items: center; justify-content: space-between; flex-wrap: wrap; gap: 40px; }
        .hero-content { flex: 1; min-width: 280px; }
        .hero-content h1 { font-size: 2.5rem; margin-bottom: 20px; line-height: 1.2; }
        .hero-content h1 span { color: var(--secondary); }
        .hero-content p { font-size: 1rem; margin-bottom: 30px; color: #CBD5E1; }
        .btn { background: var(--secondary); color: var(--primary); padding: 12px 30px; border-radius: 5px; font-weight: bold; text-decoration: none; display: inline-block; }
        .hero-img { flex: 1; min-width: 280px; text-align: center; }
        .hero-img img { max-width: 100%; border-radius: 10px; box-shadow: 0 10px 25px rgba(0,0,0,0.3); }

        section { padding: 4rem 5%; }
        .section-title { text-align: center; margin-bottom: 2.5rem; }
        .section-title h2 { font-size: 2rem; color: var(--primary); margin-bottom: 10px; }
        .section-title p { color: #64748B; font-size: 1rem; }

        .about { background: #FFFFFF; display: flex; gap: 30px; align-items: center; flex-wrap: wrap; }
        .about-text { flex: 1; min-width: 280px; }
        .about-text h3 { font-size: 1.8rem; margin-bottom: 15px; color: var(--primary); }
        .about-img { flex: 1; min-width: 280px; background: var(--accent); padding: 30px; border-radius: 10px; color: var(--text-light); text-align: center; }

        .services-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(240px, 1fr)); gap: 20px; }
        .service-card { background: #FFFFFF; padding: 25px; border-radius: 8px; box-shadow: 0 4px 6px rgba(0,0,0,0.05); border-top: 4px solid var(--secondary); }
        .service-card h3 { margin-bottom: 10px; color: var(--primary); font-size: 1.2rem; }

        .packages-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(220px, 1fr)); gap: 20px; }
        .package-card { background: #FFFFFF; padding: 25px; border-radius: 8px; text-align: center; box-shadow: 0 4px 6px rgba(0,0,0,0.05); border: 1px solid #E2E8F0; }
        .package-card.popular { border-color: var(--secondary); background: #fffcf0; }
        .package-card h3 { font-size: 1.4rem; color: var(--primary); margin-bottom: 10px; }
        .price { font-size: 1.6rem; font-weight: bold; color: var(--secondary); margin-bottom: 15px; }
        .package-card ul { list-style: none; margin-bottom: 20px; text-align: left; }
        .package-card ul li { padding: 6px 0; border-bottom: 1px solid #F1F5F9; font-size: 0.9rem; }

        .portfolio-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(260px, 1fr)); gap: 20px; }
        .portfolio-item { background: var(--primary); color: white; padding: 30px; border-radius: 8px; text-align: center; font-weight: bold; font-size: 1.1rem; border-bottom: 4px solid var(--secondary); }

        .testimonials-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(260px, 1fr)); gap: 20px; }
        .testimonial-card { background: #FFFFFF; padding: 20px; border-radius: 8px; box-shadow: 0 4px 6px rgba(0,0,0,0.05); }
        .testimonial-card p { font-style: italic; margin-bottom: 12px; font-size: 0.95rem; }
        .client-name { font-weight: bold; color: var(--secondary); font-size: 0.9rem; }

        footer { background: var(--primary); color: var(--text-light); padding: 2.5rem 5%; text-align: center; }
        footer p { margin-top: 15px; color: #94A3B8; font-size: 0.85rem; }
    </style>
</head>
<body>

    <header>
        <div class="logo-area">
            <h2>DEVCRAFT STUDIO</h2>
        </div>
        <nav>
            <a href="#home">Home</a>
            <a href="#about">About</a>
            <a href="#services">Services</a>
            <a href="#packages">Packages</a>
            <a href="#portfolio">Demo</a>
            <a href="#testimonials">Reviews</a>
            <a href="#contact">Contact</a>
        </nav>
    </header>

    <section class="hero" id="home">
        <div class="hero-content">
            <h1>Crafting Digital Experiences, <span>Building Businesses Online.</span></h1>
            <p>A digital studio where we blend technology and elegant design to craft your complete business online. Fast, responsive, and high-performing websites.</p>
            <a href="#contact" class="btn">Get Started Now</a>
        </div>
        <div class="hero-img">
            <img src="https://images.unsplash.com/photo-1460925895917-afdab827c52f?auto=format&fit=crop&w=500&q=80" alt="Agency Preview">
        </div>
    </section>

    <section class="about" id="about">
        <div class="about-text">
            <h3>About DevCraft Studio</h3>
            <p>DevCraft Studio ek peshewar website development aur digital solutions agency hai. Humara maqsad business ko modern, fast aur secure websites ke zariye online grow karna hai. Hum sirf developers nahi, balkay aapke digital growth partner hain.</p>
        </div>
        <div class="about-img">
            <h3>Your Vision, Our Code</h3>
            <p style="margin-top: 10px; color: #CBD5E1; font-size: 0.9rem;">Modern Design | Fast Performance | SEO Ready | Long-Term Support</p>
        </div>
    </section>

    <section id="services">
        <div class="section-title">
            <h2>Our Services</h2>
            <p>Complete Web Solutions for Your Business</p>
        </div>
        <div class="services-grid">
            <div class="service-card">
                <h3>Business Websites</h3>
                <p>Showcase your brand professionally with modern layouts.</p>
            </div>
            <div class="service-card">
                <h3>E-Commerce Stores</h3>
                <p>Sell online with complete ease, security and payment integration.</p>
            </div>
            <div class="service-card">
                <h3>Portfolio Websites</h3>
                <p>Perfect for freelancers, creators and professionals.</p>
            </div>
            <div class="service-card">
                <h3>Landing Pages</h3>
                <p>High-converting pages designed to turn visitors into customers.</p>
            </div>
            <div class="service-card">
                <h3>Custom Web Applications</h3>
                <p>Tailored web solutions designed specifically for your unique needs.</p>
            </div>
            <div class="service-card">
                <h3>Website Redesign & SEO</h3>
                <p>Give your old site a fresh look and get better visibility.</p>
            </div>
        </div>
    </section>

    <section id="packages" style="background: #FFFFFF;">
        <div class="section-title">
            <h2>Website Packages & Fee Structure</h2>
            <p>Choose the plan that fits your goals</p>
        </div>
        <div class="packages-grid">
            <div class="package-card">
                <h3>Basic</h3>
                <div class="price">Rs. 2,500</div>
                <ul>
                    <li>Search bar included</li>
                    <li>Products - up to 30</li>
                    <li>Basic checkout system</li>
                    <li>Free GitHub domain</li>
                    <li>2 editing rounds free</li>
                </ul>
            </div>
            <div class="package-card">
                <h3>Standard</h3>
                <div class="price">Rs. 3,500</div>
                <ul>
                    <li>Search bar included</li>
                    <li>Products - up to 40</li>
                    <li>Product categories & images</li>
                    <li>Updated checkout system</li>
                    <li>3 editing rounds free</li>
                </ul>
            </div>
            <div class="package-card popular">
                <h3>Professional</h3>
                <div class="price">Rs. 5,000</div>
                <ul>
                    <li>Products up to 50</li>
                    <li>Updated checkout systems</li>
                    <li>Lifetime GitHub domain</li>
                    <li>WhatsApp button & Search bar</li>
                    <li>Free product editing rounds</li>
                </ul>
            </div>
            <div class="package-card">
                <h3>Ultimate</h3>
                <div class="price">Rs. 7,000</div>
                <ul>
                    <li>Seller dashboard included</li>
                    <li>Free custom domain</li>
                    <li>All previous features</li>
                    <li>Full feature package as agreed</li>
                </ul>
            </div>
        </div>
    </section>

    <section id="portfolio">
        <div class="section-title">
            <h2>Our Demo Websites Portfolio</h2>
            <p>Take a look at 5 to 6 sample websites we've built.</p>
        </div>
        <div class="portfolio-grid">
            <div class="portfolio-item">Demo 1: Green Living Eco Store</div>
            <div class="portfolio-item">Demo 2: TechPulse Corporate Web</div>
            <div class="portfolio-item">Demo 3: UrbanFashion E-Commerce</div>
            <div class="portfolio-item">Demo 4: Creative Art Portfolio</div>
            <div class="portfolio-item">Demo 5: Elite Real Estate Portal</div>
            <div class="portfolio-item">Demo 6: Foodie Restaurant Landing</div>
        </div>
    </section>

    <section id="testimonials" style="background: #FFFFFF;">
        <div class="section-title">
            <h2>Client Testimonials</h2>
            <p>What our clients say about our work</p>
        </div>
        <div class="testimonials-grid">
            <div class="testimonial-card">
                <p>"DevCraft Studio delivered an amazing website for our store. The design is clean, fast and exactly what we needed."</p>
                <div class="client-name">- Ayesha Khan ⭐⭐⭐⭐⭐</div>
            </div>
            <div class="testimonial-card">
                <p>"Professional, responsive and easy to work with. Highly recommended for a reliable web development team."</p>
                <div class="client-name">- Usman Raza (Founder Tech) ⭐⭐⭐⭐⭐</div>
            </div>
            <div class="testimonial-card">
                <p>"Great service and on-time delivery. They understood our vision and turned it into a beautiful website."</p>
                <div class="client-name">- Sarah Malik (Owner) ⭐⭐⭐⭐⭐</div>
            </div>
        </div>
    </section>

    <section id="contact">
        <div class="section-title">
            <h2>Get In Touch</h2>
            <p>Ready to build your dream website? Contact us today!</p>
        </div>
        <div style="text-align: center; font-size: 1.1rem; margin-bottom: 25px;">
            <p><strong>Phone / WhatsApp:</strong> <span style="color: var(--secondary);">0303-4812714</span></p>
            <p><strong>Email:</strong> info@devcraftstudio.com</p>
            <p><strong>Location:</strong> Lahore, Pakistan</p>
        </div>
        <div style="background: #FFFFFF; padding: 20px; border-radius: 8px; max-width: 700px; margin: 0 auto; box-shadow: 0 4px 6px rgba(0,0,0,0.05);">
            <h3 style="color: var(--primary); margin-bottom: 8px; font-size: 1.2rem;">Terms & Conditions & Package Notes</h3>
            <ul style="color: var(--text-dark); padding-left: 18px; font-size: 0.9rem; line-height: 1.7;">
                <li>Editing rounds mein free limit ke andar product/content updates shamil hain.</li>
                <li>Sirf wohi features included honge jo har package ke sath wazeh tor par list kiye gaye hain.</li>
            </ul>
        </div>
    </section>

    <footer>
        <h3>DEVCRAFT STUDIO</h3>
        <p>Your Vision, Our Code. All Rights Reserved © 2026</p>
    </footer>

</body>
</html>
