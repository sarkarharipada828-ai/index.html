<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Dream N Dress - Men's Fashion</title>
  
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@500;600;700&family=Inter:wght@300;400;500;600&display=swap" rel="stylesheet">

  <style>
    :root {
      --bg-dark: #0f0f0f;
      --bg-darker: #080808;
      --text-light: #f5f5f5;
      --text-muted: #b0b0b0;
      --gold: #d4af37;
      --gold-dark: #b8972e;
    }

    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    html {
      scroll-behavior: smooth;
    }

    body {
      font-family: 'Inter', sans-serif;
      background-color: var(--bg-dark);
      color: var(--text-light);
      line-height: 1.6;
      overflow-x: hidden;
    }

    h1, h2, h3, h4 {
      font-family: 'Playfair Display', serif;
      font-weight: 600;
    }

    /* ─── Floating WhatsApp Button ─── */
    .whatsapp-float {
      position: fixed;
      width: 60px;
      height: 60px;
      bottom: 30px;
      right: 30px;
      background: #25D366;
      color: white;
      border-radius: 50%;
      text-align: center;
      font-size: 38px;
      box-shadow: 2px 4px 12px rgba(0,0,0,0.4);
      z-index: 1000;
      display: flex;
      align-items: center;
      justify-content: center;
      transition: all 0.3s ease;
    }

    .whatsapp-float:hover {
      transform: scale(1.12);
      background: #20b955;
    }

    /* ─── Navigation ─── */
    nav {
      position: fixed;
      top: 0;
      width: 100%;
      z-index: 900;
      background: rgba(8,8,8,0.92);
      backdrop-filter: blur(10px);
      border-bottom: 1px solid rgba(212,175,55,0.12);
      transition: all 0.4s ease;
    }

    nav.scrolled {
      background: rgba(8,8,8,0.98);
      box-shadow: 0 4px 25px rgba(0,0,0,0.6);
    }

    .nav-container {
      max-width: 1400px;
      margin: 0 auto;
      padding: 1.1rem 5%;
      display: flex;
      justify-content: space-between;
      align-items: center;
    }

    .logo {
      font-size: 1.9rem;
      font-weight: 700;
      color: var(--gold);
      letter-spacing: 1px;
    }

    .nav-links {
      display: flex;
      gap: 2.4rem;
      list-style: none;
    }

    .nav-links a {
      color: var(--text-light);
      text-decoration: none;
      font-weight: 500;
      transition: all 0.3s ease;
      position: relative;
    }

    .nav-links a::after {
      content: '';
      position: absolute;
      width: 0;
      height: 2px;
      bottom: -6px;
      left: 0;
      background-color: var(--gold);
      transition: width 0.35s ease;
    }

    .nav-links a:hover::after,
    .nav-links a.active::after {
      width: 100%;
    }

    .nav-links a:hover,
    .nav-links a.active {
      color: var(--gold);
    }

    /* ─── Hero ─── */
    #home {
      height: 100vh;
      min-height: 720px;
      background: linear-gradient(rgba(0,0,0,0.68), rgba(0,0,0,0.78)),
                  url('https://images.unsplash.com/photo-1552374196-1ab2a1c593e8?auto=format&fit=crop&q=80&w=1974') center center / cover no-repeat;
      display: flex;
      align-items: center;
      justify-content: center;
      text-align: center;
      position: relative;
    }

    .hero-content {
      max-width: 900px;
      padding: 0 5%;
    }

    .hero-content h1 {
      font-size: clamp(3.5rem, 9vw, 7.2rem);
      color: white;
      margin-bottom: 1.2rem;
      letter-spacing: 2px;
      text-shadow: 0 6px 25px rgba(0,0,0,0.8);
    }

    .hero-content p {
      font-size: clamp(1.3rem, 4vw, 1.8rem);
      color: var(--text-muted);
      margin-bottom: 2.5rem;
      max-width: 680px;
      margin-left: auto;
      margin-right: auto;
    }

    .btn {
      display: inline-block;
      padding: 0.95rem 2.6rem;
      background: var(--gold);
      color: #0f0f0f;
      text-decoration: none;
      font-weight: 600;
      border-radius: 50px;
      transition: all 0.35s ease;
      border: 2px solid var(--gold);
    }

    .btn:hover {
      background: transparent;
      color: var(--gold);
      transform: translateY(-3px);
      box-shadow: 0 10px 30px rgba(212,175,55,0.25);
    }

    /* ─── Sections ─── */
    section {
      padding: 120px 5% 100px;
      max-width: 1400px;
      margin: 0 auto;
    }

    h2 {
      font-size: clamp(2.8rem, 7vw, 5rem);
      text-align: center;
      margin-bottom: 1.2rem;
      color: var(--gold);
    }

    .section-subtitle {
      text-align: center;
      color: var(--text-muted);
      font-size: 1.25rem;
      max-width: 680px;
      margin: 0 auto 4rem;
    }

    /* Products Grid */
    .products-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
      gap: 2.2rem;
      margin-top: 3rem;
    }

    .product-card {
      background: #111;
      border-radius: 12px;
      overflow: hidden;
      transition: all 0.4s ease;
      border: 1px solid #222;
    }

    .product-card:hover {
      transform: translateY(-12px);
      border-color: var(--gold);
      box-shadow: 0 20px 40px rgba(0,0,0,0.5);
    }

    .product-img {
      height: 380px;
      background-size: cover;
      background-position: center;
    }

    .product-info {
      padding: 1.6rem;
      text-align: center;
    }

    .product-info h3 {
      font-size: 1.4rem;
      margin-bottom: 0.6rem;
    }

    .price {
      color: var(--gold);
      font-size: 1.3rem;
      font-weight: 600;
    }

    /* Gallery */
    .gallery-grid {
      display: grid;
      grid-template-columns: repeat# index.html
