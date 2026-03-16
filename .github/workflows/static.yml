<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Le Sutureur d'Ab&#238;mes - ALLAL Mouaadh Wassim</title>
    <meta name="description" content="Le Sutureur d'Ab&#238;mes, Tome Premier. Un roman de ALLAL Mouaadh Wassim entre Tlemcen et Washington.">
    <link rel="icon" type="image/svg+xml" href="data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 64 64'%3E%3Crect width='64' height='64' rx='12' fill='%23080810'/%3E%3Cpath d='M8 32 Q20 20 32 20 Q44 20 56 32 Q44 44 32 44 Q20 44 8 32Z' fill='%232a2214' stroke='%23d4a857' stroke-width='1.5'/%3E%3Ccircle cx='32' cy='32' r='8' fill='%238a7033'/%3E%3Ccircle cx='32' cy='32' r='5' fill='%233a1515'/%3E%3Ccircle cx='32' cy='32' r='2.5' fill='%238b2020'/%3E%3Ccircle cx='34' cy='30.5' r='1.2' fill='%23e8c06a'/%3E%3C/svg%3E">
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:ital,wght@0,400;0,500;0,600;0,700;0,800;1,400;1,500;1,600&family=Outfit:wght@200;300;400;500;600&display=swap" rel="stylesheet">
    <style>
        *, *::before, *::after { margin: 0; padding: 0; box-sizing: border-box; }

        :root {
            --gold: #d4a857;
            --gold-bright: #f0d68a;
            --gold-dim: #8a7033;
            --red-deep: #6b1a1a;
            --red-glow: #a83232;
            --bg: #060609;
            --bg-raised: #0c0c12;
            --bg-card: #10101a;
            --text: #c8c8d0;
            --text-bright: #eaeaf0;
            --text-dim: #6a6a78;
            --serif: 'Playfair Display', Georgia, serif;
            --sans: 'Outfit', system-ui, sans-serif;
        }

        html { scroll-behavior: smooth; }

        body {
            font-family: var(--sans);
            background: var(--bg);
            color: var(--text);
            line-height: 1.7;
            overflow-x: hidden;
            -webkit-font-smoothing: antialiased;
        }

        ::selection { background: rgba(212,168,87,0.3); color: #fff; }
        ::-webkit-scrollbar { width: 4px; }
        ::-webkit-scrollbar-track { background: var(--bg); }
        ::-webkit-scrollbar-thumb { background: var(--gold-dim); border-radius: 2px; }

        /* NAV */
        .nav {
            position: fixed; top: 0; left: 0; right: 0; z-index: 100;
            padding: 1.2rem 3rem;
            display: flex; justify-content: space-between; align-items: center;
            transition: background 0.4s, padding 0.4s, backdrop-filter 0.4s;
        }
        .nav.scrolled {
            background: rgba(6,6,9,0.88);
            backdrop-filter: blur(20px);
            -webkit-backdrop-filter: blur(20px);
            padding: 0.8rem 3rem;
            border-bottom: 1px solid rgba(212,168,87,0.08);
        }
        .nav-logo {
            font-family: var(--serif); font-size: 1rem; font-weight: 600;
            color: var(--gold); text-decoration: none; letter-spacing: 0.02em;
        }
        .nav-links { display: flex; gap: 2rem; }
        .nav-links a {
            font-size: 0.72rem; font-weight: 400; letter-spacing: 0.12em;
            text-transform: uppercase; color: var(--text-dim);
            text-decoration: none; transition: color 0.3s;
        }
        .nav-links a:hover { color: var(--gold); }

        .wrap { max-width: 1200px; margin: 0 auto; padding: 0 3rem; }

        @media (max-width: 768px) {
            .nav { padding: 1rem 1.5rem; }
            .nav.scrolled { padding: 0.7rem 1.5rem; }
            .nav-links { display: none; }
            .wrap { padding: 0 1.5rem; }
        }

        /* HERO */
        .hero {
            height: 100vh; min-height: 700px;
            display: flex; align-items: center; justify-content: center;
            position: relative; overflow: hidden;
        }
        .hero-bg { position: absolute; inset: 0; z-index: 0; }
        .hero-bg canvas { width: 100%; height: 100%; display: block; }
        .hero-overlay {
            position: absolute; inset: 0; z-index: 1;
            background: radial-gradient(ellipse 50% 70% at 50% 50%, transparent, var(--bg));
        }
        .hero-content {
            position: relative; z-index: 2;
            text-align: center; max-width: 800px; padding: 0 2rem;
        }
        .hero-author-name {
            font-family: var(--sans); font-size: 0.7rem; font-weight: 400;
            letter-spacing: 0.4em; text-transform: uppercase; color: var(--gold);
            margin-bottom: 2rem; opacity: 0; animation: fu 1s 0.3s ease forwards;
        }
        .hero-title {
            font-family: var(--serif);
            font-size: clamp(3rem, 8vw, 7rem);
            font-weight: 800; color: #fff; line-height: 0.95;
            letter-spacing: -0.02em; margin-bottom: 1rem;
            opacity: 0; animation: fu 1.2s 0.5s ease forwards;
        }
        .hero-title span {
            display: block;
            background: linear-gradient(135deg, #fff 30%, var(--gold-bright) 100%);
            -webkit-background-clip: text; -webkit-text-fill-color: transparent;
            background-clip: text;
        }
        .hero-tome {
            font-family: var(--serif);
            font-size: clamp(0.9rem, 2vw, 1.3rem);
            font-weight: 400; font-style: italic; color: var(--gold);
            margin-bottom: 3rem; opacity: 0; animation: fu 1s 0.8s ease forwards;
        }
        .hero-line {
            width: 50px; height: 1px; background: var(--gold);
            margin: 0 auto 2rem;
            opacity: 0; animation: fu 1s 1s ease forwards;
        }
        .hero-quote {
            font-family: var(--serif);
            font-size: clamp(0.95rem, 1.8vw, 1.15rem);
            font-style: italic; color: var(--text-dim);
            max-width: 480px; margin: 0 auto 3rem; line-height: 1.9;
            opacity: 0; animation: fu 1s 1.1s ease forwards;
        }
        .btn-gold {
            display: inline-flex; align-items: center; gap: 0.8rem;
            padding: 1rem 2.5rem;
            font-family: var(--sans); font-size: 0.75rem; font-weight: 500;
            letter-spacing: 0.2em; text-transform: uppercase;
            color: var(--bg);
            background: linear-gradient(135deg, var(--gold), var(--gold-bright));
            text-decoration: none; border: none; cursor: pointer;
            transition: transform 0.3s, box-shadow 0.3s;
        }
        .btn-gold.hero-anim { opacity: 0; animation: fu 1s 1.3s ease forwards; }
        .btn-gold:hover {
            transform: translateY(-3px);
            box-shadow: 0 10px 40px rgba(212,168,87,0.25);
        }
        .btn-gold svg { width: 14px; height: 14px; transition: transform 0.3s; }
        .btn-gold:hover svg { transform: translateX(4px); }

        /* ORDER BUTTON — pulse glow */
        .btn-order {
            display: inline-flex; align-items: center; gap: 0.8rem;
            padding: 1rem 2.8rem;
            font-family: var(--sans); font-size: 0.78rem; font-weight: 600;
            letter-spacing: 0.18em; text-transform: uppercase;
            color: #fff;
            background: linear-gradient(135deg, var(--red-deep), #8b2020 60%, var(--red-glow));
            border: 1px solid rgba(212,168,87,0.3);
            text-decoration: none; cursor: pointer;
            position: relative; overflow: hidden;
            transition: transform 0.3s, box-shadow 0.3s;
            animation: orderPulse 3s ease-in-out infinite;
        }
        .btn-order::before {
            content: ''; position: absolute; inset: -1px;
            background: linear-gradient(135deg, var(--gold), transparent 50%, var(--gold));
            opacity: 0; transition: opacity 0.4s;
            z-index: 0;
        }
        .btn-order:hover::before { opacity: 0.15; }
        .btn-order:hover {
            transform: translateY(-3px) scale(1.03);
            box-shadow: 0 10px 50px rgba(168,50,50,0.35), 0 0 30px rgba(212,168,87,0.15);
        }
        .btn-order span { position: relative; z-index: 1; }
        .btn-order svg { width: 16px; height: 16px; position: relative; z-index: 1; transition: transform 0.3s; }
        .btn-order:hover svg { transform: translateX(4px); }
        .btn-order.hero-anim { opacity: 0; animation: fu 1s 1.5s ease forwards, orderPulse 3s 2.5s ease-in-out infinite; }
        @keyframes orderPulse {
            0%, 100% { box-shadow: 0 0 0 rgba(168,50,50,0); }
            50% { box-shadow: 0 0 30px rgba(168,50,50,0.25), 0 0 60px rgba(212,168,87,0.08); }
        }
        .hero-buttons { display: flex; gap: 1.2rem; justify-content: center; flex-wrap: wrap; }

        /* NAV ORDER LINK */
        .nav-links .nav-order {
            color: var(--gold) !important;
            padding: 0.35rem 1rem;
            border: 1px solid var(--gold-dim);
            font-weight: 500 !important;
            transition: background 0.3s, color 0.3s, border-color 0.3s;
        }
        .nav-links .nav-order:hover {
            background: var(--gold);
            color: var(--bg) !important;
            border-color: var(--gold);
        }

        /* ORDER SECTION */
        .order-section {
            padding: 8rem 0; position: relative; overflow: hidden;
        }
        .order-section::before {
            content: ''; position: absolute; inset: 0;
            background:
                radial-gradient(ellipse 60% 50% at 50% 50%, rgba(107,26,26,0.12), transparent),
                linear-gradient(135deg, rgba(212,168,87,0.04), transparent 40%, rgba(107,26,26,0.06));
            border-top: 1px solid rgba(212,168,87,0.08);
            border-bottom: 1px solid rgba(212,168,87,0.08);
        }
        .order-inner {
            position: relative; text-align: center; max-width: 650px; margin: 0 auto;
        }
        .order-icon {
            width: 56px; height: 56px; margin: 0 auto 2rem;
            border: 2px solid var(--gold-dim); border-radius: 50%;
            display: flex; align-items: center; justify-content: center;
            background: var(--bg-card);
        }
        .order-icon svg { width: 24px; height: 24px; color: var(--gold); }
        .order-title {
            font-family: var(--serif);
            font-size: clamp(1.8rem, 4vw, 3rem);
            font-weight: 700; color: #fff; line-height: 1.2;
            margin-bottom: 1.5rem;
        }
        .order-sub {
            font-size: 1.05rem; color: var(--text);
            line-height: 1.9; margin-bottom: 2.5rem;
        }
        .order-details {
            display: flex; justify-content: center; gap: 3rem;
            margin-bottom: 3rem; flex-wrap: wrap;
        }
        .order-detail {
            text-align: center;
        }
        .order-detail-value {
            font-family: var(--serif); font-size: 1.4rem;
            font-weight: 700; color: var(--gold);
        }
        .order-detail-label {
            font-size: 0.65rem; letter-spacing: 0.15em;
            text-transform: uppercase; color: var(--text-dim); margin-top: 0.3rem;
        }
        .btn-order-big {
            display: inline-flex; align-items: center; gap: 1rem;
            padding: 1.2rem 3.5rem;
            font-family: var(--sans); font-size: 0.85rem; font-weight: 600;
            letter-spacing: 0.18em; text-transform: uppercase;
            color: #fff;
            background: linear-gradient(135deg, var(--red-deep), #8b2020 60%, var(--red-glow));
            border: 1px solid rgba(212,168,87,0.3);
            text-decoration: none; cursor: pointer;
            transition: transform 0.3s, box-shadow 0.3s;
            animation: orderPulse 3s ease-in-out infinite;
        }
        .btn-order-big:hover {
            transform: translateY(-3px) scale(1.03);
            box-shadow: 0 12px 50px rgba(168,50,50,0.35), 0 0 40px rgba(212,168,87,0.15);
        }
        .btn-order-big svg { width: 18px; height: 18px; transition: transform 0.3s; }
        .btn-order-big:hover svg { transform: translateX(5px); }

        /* PRICING BADGES */
        .order-pricing {
            display: flex; justify-content: center; gap: 2rem;
            margin-bottom: 3rem; flex-wrap: wrap;
        }
        .pricing-card {
            background: var(--bg-card);
            border: 1px solid rgba(212,168,87,0.1);
            padding: 1.8rem 2.2rem; text-align: center;
            min-width: 200px; position: relative; overflow: hidden;
            transition: border-color 0.3s, transform 0.3s;
        }
        .pricing-card:hover {
            border-color: rgba(212,168,87,0.2);
            transform: translateY(-3px);
        }
        .pricing-card.featured {
            border-color: rgba(212,168,87,0.25);
        }
        .pricing-card.featured::after {
            content: 'GRATUIT'; position: absolute; top: 10px; right: -28px;
            background: linear-gradient(135deg, var(--gold), var(--gold-bright));
            color: var(--bg); font-size: 0.55rem; font-weight: 700;
            letter-spacing: 0.1em; padding: 0.25rem 2rem;
            transform: rotate(35deg); z-index: 1;
        }
        .pricing-format {
            font-family: var(--sans); font-size: 0.6rem; font-weight: 500;
            letter-spacing: 0.2em; text-transform: uppercase;
            color: var(--gold); margin-bottom: 0.6rem;
        }
        .pricing-price {
            font-family: var(--serif); font-size: 1.8rem; font-weight: 700;
            color: #fff; margin-bottom: 0.4rem;
        }
        .pricing-note {
            font-size: 0.8rem; color: var(--text-dim); line-height: 1.6;
        }

        .hero-scroll {
            position: absolute; bottom: 2.5rem; left: 50%;
            transform: translateX(-50%); z-index: 2;
            display: flex; flex-direction: column; align-items: center; gap: 0.6rem;
            opacity: 0; animation: fu 1s 1.6s ease forwards;
        }
        .hero-scroll span {
            font-size: 0.6rem; letter-spacing: 0.2em;
            text-transform: uppercase; color: var(--text-dim);
        }
        .scroll-bar {
            width: 1px; height: 40px;
            background: linear-gradient(to bottom, var(--gold), transparent);
            animation: sp 2s ease-in-out infinite;
        }
        @keyframes sp { 0%,100% { opacity: 0.3; transform: scaleY(0.6); } 50% { opacity: 1; transform: scaleY(1); } }
        @keyframes fu { from { opacity: 0; transform: translateY(30px); } to { opacity: 1; transform: translateY(0); } }

        /* SECTION */
        .stag {
            font-family: var(--sans); font-size: 0.65rem; font-weight: 500;
            letter-spacing: 0.3em; text-transform: uppercase; color: var(--gold-dim);
            margin-bottom: 1rem;
        }
        .stitle {
            font-family: var(--serif);
            font-size: clamp(2rem, 4vw, 3.2rem);
            font-weight: 700; color: #fff; line-height: 1.15; margin-bottom: 1.5rem;
        }

        /* SYNOPSIS */
        .synopsis { padding: 10rem 0; position: relative; }
        .synopsis::before {
            content: ''; position: absolute; top: 0; left: 50%;
            transform: translateX(-50%); width: 1px; height: 80px;
            background: linear-gradient(to bottom, transparent, var(--gold-dim));
        }
        .synopsis-layout {
            display: grid; grid-template-columns: 5fr 6fr;
            gap: 6rem; align-items: center;
        }
        .book-3d { perspective: 1200px; display: flex; justify-content: center; }
        .book-cover {
            width: 300px; height: 450px; position: relative;
            transform-style: preserve-3d;
            transform: rotateY(-12deg) rotateX(2deg);
            transition: transform 0.6s ease;
        }
        .book-cover:hover { transform: rotateY(-3deg) rotateX(1deg); }
        .book-front {
            position: absolute; inset: 0;
            background: linear-gradient(160deg, #12121e, #0a0a14 50%, #161625);
            border: 1px solid rgba(212,168,87,0.15);
            border-radius: 2px 8px 8px 2px;
            display: flex; flex-direction: column;
            align-items: center; justify-content: center;
            text-align: center; padding: 2.5rem;
            box-shadow: 0 30px 80px rgba(0,0,0,0.6), 0 0 1px rgba(212,168,87,0.15),
                        inset 0 0 80px rgba(212,168,87,0.02);
            backface-visibility: hidden;
        }
        .book-front::before {
            content: ''; position: absolute; left: 0; top: 8%; bottom: 8%;
            width: 2px;
            background: linear-gradient(to bottom, transparent, var(--gold), transparent);
            opacity: 0.2;
        }
        .book-front::after {
            content: ''; position: absolute;
            top: 10%; left: 10%; right: 10%; bottom: 10%;
            border: 1px solid rgba(212,168,87,0.06);
            pointer-events: none;
        }
        .book-spine {
            position: absolute; left: -30px; top: 0; width: 30px; height: 100%;
            background: linear-gradient(to right, #0a0a10, #101018);
            transform: rotateY(90deg); transform-origin: right;
            border-radius: 4px 0 0 4px;
            box-shadow: -5px 0 20px rgba(0,0,0,0.4);
        }
        .book-pages {
            position: absolute; right: -8px; top: 4px; width: 8px; height: calc(100% - 8px);
            background: linear-gradient(to right, #d0c8b8, #e8e0d0, #c8c0b0);
            border-radius: 0 2px 2px 0; transform: translateZ(-1px);
        }
        .bf-author {
            font-family: var(--sans); font-size: 0.55rem;
            letter-spacing: 0.35em; text-transform: uppercase;
            color: var(--gold); margin-bottom: 2rem;
        }
        .bf-title {
            font-family: var(--serif); font-size: 1.8rem; font-weight: 700;
            color: #fff; line-height: 1.15; margin-bottom: 0.6rem;
        }
        .bf-sub {
            font-family: var(--serif); font-size: 0.85rem;
            font-style: italic; color: var(--gold); margin-bottom: 2.5rem;
        }
        .bf-line { width: 40px; height: 1px; background: var(--gold-dim); margin-bottom: 1.2rem; }
        .bf-type {
            font-family: var(--sans); font-size: 0.55rem;
            letter-spacing: 0.25em; text-transform: uppercase;
            color: var(--text-dim);
        }
        .synopsis-body .sp {
            font-size: 1.05rem; color: var(--text);
            line-height: 2; margin-bottom: 1.5rem;
        }
        .synopsis-body .sp-accent {
            font-family: var(--serif); font-size: 1.15rem; font-style: italic;
            color: var(--gold-bright);
            border-left: 2px solid var(--gold); padding-left: 1.5rem;
            margin-top: 2rem; line-height: 1.9;
        }

        /* QUOTE */
        .quote-band { padding: 6rem 0; position: relative; overflow: hidden; }
        .quote-band::before {
            content: ''; position: absolute; inset: 0;
            background: linear-gradient(135deg, rgba(107,26,26,0.08), rgba(212,168,87,0.04) 50%, rgba(107,26,26,0.08));
            border-top: 1px solid rgba(212,168,87,0.06);
            border-bottom: 1px solid rgba(212,168,87,0.06);
        }
        .quote-band .wrap { position: relative; text-align: center; }
        .quote-band blockquote {
            font-family: var(--serif);
            font-size: clamp(1.3rem, 3vw, 2rem);
            font-style: italic; font-weight: 400; color: #fff;
            max-width: 650px; margin: 0 auto; line-height: 1.8;
        }
        .quote-band cite {
            display: block; margin-top: 1.5rem;
            font-family: var(--sans); font-size: 0.7rem; font-style: normal;
            font-weight: 500; letter-spacing: 0.2em; text-transform: uppercase;
            color: var(--gold);
        }

        /* EXTRACTS */
        .extracts { padding: 10rem 0; }
        .extracts-hd { text-align: center; margin-bottom: 4rem; }
        .extract-card {
            background: var(--bg-card);
            border: 1px solid rgba(255,255,255,0.03);
            padding: 3rem; margin-bottom: 1.5rem;
            position: relative; overflow: hidden;
            transition: border-color 0.4s, transform 0.4s, box-shadow 0.4s;
        }
        .extract-card:hover {
            border-color: rgba(212,168,87,0.12);
            transform: translateY(-4px);
            box-shadow: 0 20px 60px rgba(0,0,0,0.3);
        }
        .extract-card::before {
            content: ''; position: absolute; top: 0; left: 0;
            width: 3px; height: 100%;
            background: linear-gradient(to bottom, var(--gold), transparent);
            opacity: 0; transition: opacity 0.4s;
        }
        .extract-card:hover::before { opacity: 1; }
        .extract-label {
            font-family: var(--sans); font-size: 0.6rem; font-weight: 500;
            letter-spacing: 0.25em; text-transform: uppercase;
            color: var(--gold-dim); margin-bottom: 1.2rem;
        }
        .extract-text {
            font-family: var(--serif); font-size: 1.15rem;
            font-style: italic; line-height: 2; color: var(--text-bright);
        }

        /* CHARACTERS */
        .chars { padding: 10rem 0; }
        .chars-hd { text-align: center; margin-bottom: 4rem; }
        .chars-sub {
            font-size: 1rem; color: var(--text-dim);
            max-width: 500px; margin: 0 auto;
        }
        .chars-grid {
            display: grid; grid-template-columns: repeat(3, 1fr); gap: 1.5rem;
        }
        .char-card {
            background: var(--bg-card);
            border: 1px solid rgba(255,255,255,0.03);
            padding: 2.5rem 2rem; position: relative; overflow: hidden;
            transition: border-color 0.4s, transform 0.4s, box-shadow 0.4s;
        }
        .char-card:hover {
            border-color: rgba(212,168,87,0.12);
            transform: translateY(-5px);
            box-shadow: 0 25px 60px rgba(0,0,0,0.3);
        }
        .char-bar {
            width: 32px; height: 3px; margin-bottom: 1.5rem;
            transition: width 0.4s;
        }
        .char-card:hover .char-bar { width: 50px; }
        .char-name {
            font-family: var(--serif); font-size: 1.4rem;
            font-weight: 600; color: #fff; margin-bottom: 0.3rem;
        }
        .char-role {
            font-family: var(--sans); font-size: 0.65rem; font-weight: 500;
            letter-spacing: 0.2em; text-transform: uppercase;
            color: var(--gold); margin-bottom: 1.2rem;
        }
        .char-desc {
            font-size: 0.9rem; color: var(--text-dim); line-height: 1.8;
        }

        /* TOC */
        .toc { padding: 10rem 0; }
        .toc-hd { text-align: center; margin-bottom: 4rem; }
        .toc-grid { display: grid; grid-template-columns: repeat(3, 1fr); gap: 0; }
        .toc-item {
            padding: 2rem 2.5rem;
            border: 1px solid rgba(255,255,255,0.03);
            margin: -0.5px;
            display: flex; align-items: baseline; gap: 1.2rem;
            transition: background 0.3s, border-color 0.3s;
            cursor: default;
        }
        .toc-item:hover {
            background: var(--bg-card);
            border-color: rgba(212,168,87,0.08); z-index: 1;
        }
        .toc-num {
            font-family: var(--serif); font-size: 1.8rem; font-weight: 700;
            color: var(--gold-dim); min-width: 40px; transition: color 0.3s;
        }
        .toc-item:hover .toc-num { color: var(--gold); }
        .toc-name { font-family: var(--serif); font-size: 1.05rem; color: var(--text); }

        /* AUTHOR */
        .author { padding: 10rem 0; }
        .author-layout {
            display: grid; grid-template-columns: 1fr 2fr;
            gap: 5rem; align-items: center;
        }
        .author-portrait { display: flex; justify-content: center; }
        .author-ring {
            width: 200px; height: 200px; border-radius: 50%;
            position: relative; display: flex;
            align-items: center; justify-content: center;
        }
        .author-ring::before {
            content: ''; position: absolute; inset: -2px; border-radius: 50%;
            background: conic-gradient(var(--gold), transparent 40%, var(--gold-dim) 70%, transparent);
            opacity: 0.3; animation: rr 12s linear infinite;
        }
        @keyframes rr { to { transform: rotate(360deg); } }
        .author-ring-inner {
            width: 100%; height: 100%; border-radius: 50%;
            background: linear-gradient(135deg, var(--bg-card), var(--bg-raised));
            display: flex; align-items: center; justify-content: center;
            font-family: var(--serif); font-size: 4.5rem; font-weight: 700;
            color: var(--gold); position: relative; z-index: 1;
        }
        .author-text h2 {
            font-family: var(--serif);
            font-size: clamp(1.6rem, 3vw, 2.2rem);
            font-weight: 600; color: #fff; margin-bottom: 1.5rem;
        }
        .author-text p {
            font-size: 1rem; line-height: 2; color: var(--text); margin-bottom: 1rem;
        }
        .author-pull {
            font-family: var(--serif); font-size: 1.1rem; font-style: italic;
            color: var(--gold-bright);
            border-left: 2px solid var(--gold); padding-left: 1.5rem;
            margin-top: 2rem; line-height: 1.9;
        }

        /* FINALE */
        .finale { padding: 8rem 0 6rem; text-align: center; position: relative; }
        .finale::before {
            content: ''; position: absolute; bottom: 0; left: 0; right: 0;
            height: 300px;
            background: linear-gradient(to top, rgba(212,168,87,0.03), transparent);
            pointer-events: none;
        }
        .finale-title {
            font-family: var(--serif);
            font-size: clamp(1.6rem, 3.5vw, 2.8rem);
            font-weight: 700; color: #fff; line-height: 1.3;
            margin-bottom: 1.5rem;
        }
        .finale-sub {
            font-size: 1rem; color: var(--text-dim);
            max-width: 550px; margin: 0 auto 3rem; line-height: 1.9;
        }

        .footer {
            padding: 3rem 0; text-align: center;
            border-top: 1px solid rgba(255,255,255,0.03);
        }
        .footer p { font-size: 0.75rem; color: var(--text-dim); letter-spacing: 0.05em; }

        /* REVEAL */
        .rv {
            opacity: 0; transform: translateY(50px);
            transition: opacity 0.9s cubic-bezier(0.23,1,0.32,1),
                        transform 0.9s cubic-bezier(0.23,1,0.32,1);
        }
        .rv.show { opacity: 1; transform: translateY(0); }
        .rv-d1 { transition-delay: 0.1s; }
        .rv-d2 { transition-delay: 0.2s; }
        .rv-d3 { transition-delay: 0.3s; }
        .rv-d4 { transition-delay: 0.4s; }
        .rv-d5 { transition-delay: 0.5s; }

        @media (max-width: 1024px) {
            .chars-grid { grid-template-columns: repeat(2, 1fr); }
            .toc-grid { grid-template-columns: repeat(2, 1fr); }
        }
        @media (max-width: 768px) {
            .synopsis-layout { grid-template-columns: 1fr; gap: 4rem; }
            .book-3d { order: -1; }
            .book-cover { width: 240px; height: 360px; }
            .chars-grid { grid-template-columns: 1fr; }
            .toc-grid { grid-template-columns: 1fr 1fr; }
            .author-layout { grid-template-columns: 1fr; text-align: center; gap: 3rem; }
            .extract-card { padding: 2rem; }
            .char-card { padding: 2rem 1.5rem; }
        }
        @media (max-width: 480px) {
            .toc-grid { grid-template-columns: 1fr; }
            .book-cover { width: 200px; height: 300px; }
            .bf-title { font-size: 1.4rem; }
        }
    </style>
</head>
<body>

<nav class="nav" id="nav">
    <a href="#top" class="nav-logo">Le Sutureur d'Ab&#238;mes</a>
    <div class="nav-links">
        <a href="#synopsis">Synopsis</a>
        <a href="#extraits">Extraits</a>
        <a href="#personnages">Personnages</a>
        <a href="#chapitres">Chapitres</a>
        <a href="#auteur">L'auteur</a>
        <a href="https://forms.gle/5oy5MfgtQsom2P9TA" class="nav-order" target="_blank" rel="noopener noreferrer">Commander</a>
    </div>
</nav>

<section class="hero" id="top">
    <div class="hero-bg"><canvas id="heroCanvas"></canvas></div>
    <div class="hero-overlay"></div>
    <div class="hero-content">
        <p class="hero-author-name">ALLAL MOUAADH WASSIM</p>
        <h1 class="hero-title"><span>Le Sutureur<br>d'Ab&#238;mes</span></h1>
        <p class="hero-tome">Tome Premier - La Geste du Retardataire</p>
        <div class="hero-line"></div>
        <p class="hero-quote">
            "Il y a des blessures que l'on ne recoud pas.<br>
            On apprend a marcher avec."
        </p>
        <div class="hero-buttons">
            <a href="https://forms.gle/5oy5MfgtQsom2P9TA" class="btn-order hero-anim" target="_blank" rel="noopener noreferrer">
                <span>Commander le roman &mdash; Ebook gratuit</span>
                <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M3 3h2l.4 2M7 13h10l4-8H5.4M7 13L5.4 5M7 13l-2.293 2.293c-.63.63-.184 1.707.707 1.707H17m0 0a2 2 0 100 4 2 2 0 000-4zm-8 2a2 2 0 100 4 2 2 0 000-4z"/></svg>
            </a>
            <a href="#synopsis" class="btn-gold hero-anim">
                D&#233;couvrir le roman
                <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M5 12h14M12 5l7 7-7 7"/></svg>
            </a>
        </div>
    </div>
    <div class="hero-scroll">
        <span>D&#233;filer</span>
        <div class="scroll-bar"></div>
    </div>
</section>

<section class="synopsis" id="synopsis">
    <div class="wrap">
        <div class="synopsis-layout">
            <div class="book-3d rv">
                <div class="book-cover">
                    <div class="book-spine"></div>
                    <div class="book-front">
                        <p class="bf-author">ALLAL MOUAADH WASSIM</p>
                        <p class="bf-title">Le Sutureur<br>d'Ab&#238;mes</p>
                        <p class="bf-sub">La Geste du Retardataire</p>
                        <div class="bf-line"></div>
                        <p class="bf-type">Roman</p>
                    </div>
                    <div class="book-pages"></div>
                </div>
            </div>
            <div class="synopsis-body">
                <p class="stag rv">Synopsis</p>
                <h2 class="stitle rv rv-d1">Le 6 octobre, Yanis Belkhodja<br>est chass&#233; de chez lui.</h2>
                <p class="sp rv rv-d2">Vingt-trois ans. Un sac de sport. Un oeil gauche qui voit ce que personne ne devrait voir. Sa grand-m&#232;re l'accueille dans la vieille maison du quartier des Oliviers, &#224; Tlemcen - une maison de chaux et de sel, coll&#233;e &#224; une ruine que les voisins &#233;vitent sans savoir pourquoi.</p>
                <p class="sp rv rv-d3">Puis vient la nuit du 14 novembre. Le silence. Les animaux en fuite. Les chats qui convergent vers sa porte comme vers un sanctuaire. Et l'oeil de Yanis qui se met &#224; briller.</p>
                <p class="sp rv rv-d4">De Washington, une &#233;quipe de scientifiques observe. Ils ont les donn&#233;es, les cartes, les algorithmes. Ce qu'ils n'ont pas, c'est une explication. Alors ils viennent &#224; Tlemcen.</p>
                <p class="sp-accent rv rv-d5">Ce que Yanis porte en lui pourrait sauver le monde. Ou le d&#233;truire. Il faudra choisir. Et le prix du choix n'est pas celui qu'on croit.</p>
            </div>
        </div>
    </div>
</section>

<section class="quote-band">
    <div class="wrap rv">
        <blockquote>
            "La nuit, quand tu ne dors pas,<br>
            c'est que quelqu'un quelque part prie pour toi.<br>
            Ou contre toi."
        </blockquote>
        <cite>Lalla Fatma Mered</cite>
    </div>
</section>

<section class="extracts" id="extraits">
    <div class="wrap">
        <div class="extracts-hd">
            <p class="stag rv">Premi&#232;res pages</p>
            <h2 class="stitle rv rv-d1">Entrez dans le roman</h2>
        </div>

        <div class="extract-card rv">
            <p class="extract-label">Chapitre I - L'Exil du 6 Octobre</p>
            <p class="extract-text">Le 6 octobre, le ciel de Tlemcen prit la couleur d'une plaie qui refuse de cicatriser. Un rouge plus sourd, plus ancien que les cr&#233;puscules d'automne qui descendent des plateaux du Tell pour balayer les ruelles de la vieille ville... Yanis Belkhodja marchait. Il marchait comme marchent les b&#234;tes que l'on soul&#232;ve du sol natal et que l'on repose ailleurs, les pattes stupides de ne plus reconna&#238;tre la terre.</p>
        </div>

        <div class="extract-card rv">
            <p class="extract-label">Chapitre III - Le Silence</p>
            <p class="extract-text">Ce samedi soir de novembre, il faisait un froid de lame. Un froid qui voulait quelque chose. Pas les intemp&#233;ries - une volont&#233;, une direction, l'avant-garde d'une arm&#233;e dont les troupes n'avaient pas encore franchi l'horizon.</p>
        </div>

        <div class="extract-card rv">
            <p class="extract-label">Chapitre XI - La Transfiguration</p>
            <p class="extract-text">C'est arriv&#233; pendant le go&#251;ter. Pas pendant une s&#233;ance de mesure ni une transmission des djinns. Non. C'est arriv&#233; pendant le go&#251;ter - ce moment b&#234;te et doux de la journ&#233;e o&#249; Rosa apportait des biscuits et du chocolat chaud et o&#249; l'&#233;quipe se retrouvait pour quinze minutes de normalit&#233; vol&#233;es &#224; l'ab&#238;me...</p>
        </div>
    </div>
</section>

<section class="chars" id="personnages">
    <div class="wrap">
        <div class="chars-hd">
            <p class="stag rv">Les voix du roman</p>
            <h2 class="stitle rv rv-d1">Personnages</h2>
            <p class="chars-sub rv rv-d2">Six destins li&#233;s par un fil invisible, entre Tlemcen et Washington.</p>
        </div>

        <div class="chars-grid">
            <div class="char-card rv">
                <div class="char-bar" style="background:var(--gold)"></div>
                <h3 class="char-name">Yanis Belkhodja</h3>
                <p class="char-role">Le Sutureur</p>
                <p class="char-desc">Vingt-trois ans, un oeil d'ambre qui voit l'invisible. Chass&#233; par son p&#232;re, accueilli par sa grand-m&#232;re, il d&#233;couvre qu'il est le dernier d'une lign&#233;e capable de recoudre un monde qui se d&#233;chire. Son nom, en tamazight, signifie "celui que Dieu a donn&#233;".</p>
            </div>

            <div class="char-card rv rv-d1">
                <div class="char-bar" style="background:var(--red-glow)"></div>
                <h3 class="char-name">Lalla Fatma Mered</h3>
                <p class="char-role">La Gardienne</p>
                <p class="char-desc">Quatre-vingt-sept ans. Des mains de racine et de parchemin. Des yeux vert d'eau. Elle trace des cercles de sel chaque matin, br&#251;le du benjoin chaque vendredi, et attend depuis trente-deux ans que Yanis franchisse sa porte. Son mot ultime : "Amana."</p>
            </div>

            <div class="char-card rv rv-d2">
                <div class="char-bar" style="background:#c87533"></div>
                <h3 class="char-name">Elena Vasquez</h3>
                <p class="char-role">La Scientifique</p>
                <p class="char-desc">Cinquante-deux ans, n&#233;e au Guatemala. Directrice du PRACA &#224; Washington. Elle a vu, &#224; huit ans, les animaux pr&#233;dire un s&#233;isme que personne n'a &#233;cout&#233;. Depuis, elle &#233;coute. Et ce qu'elle entend dans ses donn&#233;es la m&#232;ne droit &#224; Tlemcen.</p>
            </div>

            <div class="char-card rv rv-d3">
                <div class="char-bar" style="background:var(--gold-dim)"></div>
                <h3 class="char-name">Nassima Berrahma</h3>
                <p class="char-role">L'Ancre</p>
                <p class="char-desc">Ce que les po&#232;tes arabes auraient appel&#233; une "lune de jour". Epouse de l'oncle Sofiane, elle est le fil qui rattache Yanis &#224; sa propre humanit&#233; - par les appels du soir, les g&#226;teaux au miel et l'odeur de jasmin.</p>
            </div>

            <div class="char-card rv rv-d4">
                <div class="char-bar" style="background:#5a6a5a"></div>
                <h3 class="char-name">Ammi Redouane</h3>
                <p class="char-role">La Voix du quartier</p>
                <p class="char-desc">Herboriste au souk de Tlemcen. Barbe blanche, regard malicieux, proverbes arabes dont la pertinence explose dans l'esprit comme des bombes &#224; retardement de sagesse. Il sait des choses. Depuis tr&#232;s longtemps.</p>
            </div>

            <div class="char-card rv rv-d5">
                <div class="char-bar" style="background:#2a2a3a"></div>
                <h3 class="char-name">Karim Belkhodja</h3>
                <p class="char-role">Le P&#232;re absent</p>
                <p class="char-desc">"Tu n'es plus mon fils." Quatre mots. C'est tout ce qu'il faut pour tuer un fils sans le toucher. On ne conna&#238;t de lui que sa voix et sa sentence. Il est le trou noir du roman - invisible, mais sa gravit&#233; d&#233;forme tout.</p>
            </div>
        </div>
    </div>
</section>

<section class="toc" id="chapitres">
    <div class="wrap">
        <div class="toc-hd">
            <p class="stag rv">Douze chapitres</p>
            <h2 class="stitle rv rv-d1">Table des mati&#232;res</h2>
        </div>
        <div class="toc-grid">
            <div class="toc-item rv"><span class="toc-num">I</span><span class="toc-name">L'Exil du 6 Octobre</span></div>
            <div class="toc-item rv"><span class="toc-num">II</span><span class="toc-name">La Maison des Oliviers</span></div>
            <div class="toc-item rv"><span class="toc-num">III</span><span class="toc-name">Le Silence</span></div>
            <div class="toc-item rv"><span class="toc-num">IV</span><span class="toc-name">La Mar&#233;e des Cr&#233;atures</span></div>
            <div class="toc-item rv"><span class="toc-num">V</span><span class="toc-name">Les Gardiens du Sel</span></div>
            <div class="toc-item rv"><span class="toc-num">VI</span><span class="toc-name">Les Yeux de Washington</span></div>
            <div class="toc-item rv"><span class="toc-num">VII</span><span class="toc-name">L'Enqu&#234;te de Tlemcen</span></div>
            <div class="toc-item rv"><span class="toc-num">VIII</span><span class="toc-name">La Vision des Tombes</span></div>
            <div class="toc-item rv"><span class="toc-num">IX</span><span class="toc-name">Le Nouveau Monde</span></div>
            <div class="toc-item rv"><span class="toc-num">X</span><span class="toc-name">La Langue de Basalte</span></div>
            <div class="toc-item rv"><span class="toc-num">XI</span><span class="toc-name">La Transfiguration</span></div>
            <div class="toc-item rv"><span class="toc-num">XII</span><span class="toc-name">Le Verrou</span></div>
        </div>
    </div>
</section>

<section class="author" id="auteur">
    <div class="wrap">
        <div class="author-layout">
            <div class="author-portrait rv">
                <div class="author-ring">
                    <div class="author-ring-inner">A</div>
                </div>
            </div>
            <div class="author-text">
                <p class="stag rv">L'auteur</p>
                <h2 class="rv rv-d1">ALLAL Mouaadh Wassim</h2>
                <p class="rv rv-d2">Vingt-trois ans. Etudiant en langue fran&#231;aise &#224; l'Universit&#233; d'Abou Bakr Belkaid de Tlemcen. Le Sutureur d'Ab&#238;mes est son premier roman.</p>
                <p class="rv rv-d3">N&#233; entre deux mondes - celui, visible, des rues de Tlemcen, du th&#233; &#224; la menthe et des feuilletons du soir, et celui, invisible, des r&#233;cits murmur&#233;s par les grands-m&#232;res apr&#232;s le d&#238;ner. Les histoires de djinns, de Zouhri, de maisons qui respirent et de morts qui veillent.</p>
                <p class="author-pull rv rv-d4">"Le lecteur qui entre ici doit savoir qu'on ne ressort pas tout &#224; fait le m&#234;me de la maison des Oliviers. Vous &#234;tes pr&#233;venus."</p>
            </div>
        </div>
    </div>
</section>

<section class="order-section" id="commander">
    <div class="wrap">
        <div class="order-inner">
            <div class="order-icon rv">
                <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.5"><path d="M12 6.253v13m0-13C10.832 5.477 9.246 5 7.5 5S4.168 5.477 3 6.253v13C4.168 18.477 5.754 18 7.5 18s3.332.477 4.5 1.253m0-13C13.168 5.477 14.754 5 16.5 5c1.747 0 3.332.477 4.5 1.253v13C19.832 18.477 18.247 18 16.5 18c-1.746 0-3.332.477-4.5 1.253"/></svg>
            </div>
            <p class="stag rv">Obtenez votre exemplaire</p>
            <h2 class="order-title rv rv-d1">Commandez<br>Le Sutureur d'Ab&#238;mes</h2>
            <p class="order-sub rv rv-d2">Le roman est offert en format num&#233;rique. Pour le format papier, seul le co&#251;t d'impression est &#224; votre charge. L'aventure entre Tlemcen et Washington n'attend que vous.</p>
            <div class="order-pricing rv rv-d3">
                <div class="pricing-card featured">
                    <p class="pricing-format">Ebook / PDF</p>
                    <p class="pricing-price">Gratuit</p>
                    <p class="pricing-note">Format num&#233;rique<br>envoy&#233; par email</p>
                </div>
                <div class="pricing-card">
                    <p class="pricing-format">Format Physique</p>
                    <p class="pricing-price">Prix d'impression</p>
                    <p class="pricing-note">Broch&#233; A5 &mdash; 176 pages<br>vous ne payez que l'imprimeur</p>
                </div>
            </div>
            <div class="order-details rv rv-d3">
                <div class="order-detail">
                    <div class="order-detail-value">176</div>
                    <div class="order-detail-label">Pages</div>
                </div>
                <div class="order-detail">
                    <div class="order-detail-value">12</div>
                    <div class="order-detail-label">Chapitres</div>
                </div>
                <div class="order-detail">
                    <div class="order-detail-value">A5</div>
                    <div class="order-detail-label">Format</div>
                </div>
                <div class="order-detail">
                    <div class="order-detail-value">Tome I</div>
                    <div class="order-detail-label">Premier volume</div>
                </div>
            </div>
            <a href="https://forms.gle/5oy5MfgtQsom2P9TA" class="btn-order-big rv rv-d4" target="_blank" rel="noopener noreferrer">
                Commander maintenant
                <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M5 12h14M12 5l7 7-7 7"/></svg>
            </a>
        </div>
    </div>
</section>

<section class="finale">
    <div class="wrap rv">
        <p class="stag">Le fil ne se rompt pas</p>
        <h2 class="finale-title">Entre Tlemcen et Washington,<br>une course contre l'apocalypse commence.</h2>
        <p class="finale-sub">Entre le mysticisme des veill&#233;es alg&#233;riennes et la froideur des laboratoires am&#233;ricains, entre le sel de Lalla Fatma et les &#233;crans du PRACA.</p>
        <a href="#top" class="btn-gold">
            Revenir en haut
            <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M12 19V5M5 12l7-7 7 7"/></svg>
        </a>
    </div>
</section>

<footer class="footer">
    <div class="wrap">
        <p>2026 ALLAL Mouaadh Wassim - Le Sutureur d'Ab&#238;mes, Tome Premier.</p>
    </div>
</footer>

<script>
(function() {
    var nav = document.getElementById('nav');
    window.addEventListener('scroll', function() {
        if (window.pageYOffset > 80) nav.classList.add('scrolled');
        else nav.classList.remove('scrolled');
    });

    var rvs = document.querySelectorAll('.rv');
    var obs = new IntersectionObserver(function(entries) {
        entries.forEach(function(e) { if (e.isIntersecting) e.target.classList.add('show'); });
    }, { threshold: 0.1, rootMargin: '0px 0px -40px 0px' });
    rvs.forEach(function(el) { obs.observe(el); });

    var c = document.getElementById('heroCanvas');
    var ctx = c.getContext('2d');
    var w, h, pts, mx, my;

    function sz() { w = c.width = c.offsetWidth; h = c.height = c.offsetHeight; }
    sz();
    window.addEventListener('resize', sz);
    mx = w / 2; my = h / 2;
    document.addEventListener('mousemove', function(e) { mx = e.clientX; my = e.clientY; });

    pts = [];
    var n = Math.min(80, Math.floor(w * h / 15000));
    for (var i = 0; i < n; i++) {
        pts.push({
            x: Math.random() * w, y: Math.random() * h,
            vx: (Math.random() - 0.5) * 0.3, vy: (Math.random() - 0.5) * 0.3,
            r: Math.random() * 1.5 + 0.5, a: Math.random() * 0.5 + 0.1
        });
    }

    function frame() {
        ctx.clearRect(0, 0, w, h);

        var g = ctx.createRadialGradient(w * 0.5, h * 0.45, 0, w * 0.5, h * 0.45, w * 0.35);
        g.addColorStop(0, 'rgba(212,168,87,0.04)');
        g.addColorStop(0.5, 'rgba(107,26,26,0.02)');
        g.addColorStop(1, 'transparent');
        ctx.fillStyle = g;
        ctx.fillRect(0, 0, w, h);

        var mg = ctx.createRadialGradient(mx, my, 0, mx, my, 200);
        mg.addColorStop(0, 'rgba(212,168,87,0.03)');
        mg.addColorStop(1, 'transparent');
        ctx.fillStyle = mg;
        ctx.fillRect(0, 0, w, h);

        for (var i = 0; i < pts.length; i++) {
            var p = pts[i];
            p.x += p.vx; p.y += p.vy;
            if (p.x < 0) p.x = w; if (p.x > w) p.x = 0;
            if (p.y < 0) p.y = h; if (p.y > h) p.y = 0;

            ctx.beginPath();
            ctx.arc(p.x, p.y, p.r, 0, Math.PI * 2);
            ctx.fillStyle = 'rgba(212,168,87,' + p.a + ')';
            ctx.fill();

            for (var j = i + 1; j < pts.length; j++) {
                var q = pts[j];
                var dx = p.x - q.x, dy = p.y - q.y;
                var d = Math.sqrt(dx * dx + dy * dy);
                if (d < 120) {
                    ctx.beginPath(); ctx.moveTo(p.x, p.y); ctx.lineTo(q.x, q.y);
                    ctx.strokeStyle = 'rgba(212,168,87,' + (0.06 * (1 - d / 120)) + ')';
                    ctx.lineWidth = 0.5; ctx.stroke();
                }
            }

            var dmx = mx - p.x, dmy = my - p.y;
            var dd = Math.sqrt(dmx * dmx + dmy * dmy);
            if (dd < 200) {
                ctx.beginPath(); ctx.moveTo(p.x, p.y); ctx.lineTo(mx, my);
                ctx.strokeStyle = 'rgba(212,168,87,' + (0.08 * (1 - dd / 200)) + ')';
                ctx.lineWidth = 0.4; ctx.stroke();
            }
        }
        requestAnimationFrame(frame);
    }
    frame();

    var bc = document.querySelector('.book-cover');
    if (bc) {
        var bp = bc.parentElement;
        window.addEventListener('mousemove', function(e) {
            var r = bp.getBoundingClientRect();
            var cx = r.left + r.width / 2, cy = r.top + r.height / 2;
            var dx = (e.clientX - cx) / r.width, dy = (e.clientY - cy) / r.height;
            bc.style.transform = 'rotateY(' + (-12 + dx * 8) + 'deg) rotateX(' + (2 + dy * -4) + 'deg)';
        });
    }
})();
</script>

</body>
</html>
