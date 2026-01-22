# davidirl.github.io

<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>O Caminho da Aprovação — Livro em PDF</title>
  <meta name="description" content="O Caminho da Aprovação: um livro completo sobre método, inteligência prática e maturidade emocional para concursos públicos. Acesso imediato em PDF." />
  <style>
    :root {
      --bg1: #071a2b;
      --bg2: #0b2b2a;
      --card: rgba(255,255,255,0.08);
      --card2: rgba(255,255,255,0.10);
      --text: #eaf2ff;
      --muted: rgba(234,242,255,0.75);
      --muted2: rgba(234,242,255,0.60);
      --accent: #5eead4;   /* teal */
      --accent2: #93c5fd;  /* soft blue */
      --good: #86efac;
      --warn: #fde68a;
      --shadow: 0 18px 45px rgba(0,0,0,0.35);
      --radius: 16px;
      --radius2: 22px;
      --max: 1080px;
    }

    * { box-sizing: border-box; }

    body {
      margin: 0;
      font-family: ui-sans-serif, system-ui, -apple-system, Segoe UI, Roboto, Arial, "Apple Color Emoji", "Segoe UI Emoji";
      color: var(--text);
      line-height: 1.65;
      background:
        radial-gradient(1200px 700px at 10% 10%, rgba(94,234,212,0.16), transparent 60%),
        radial-gradient(900px 600px at 85% 20%, rgba(147,197,253,0.14), transparent 55%),
        radial-gradient(900px 700px at 40% 90%, rgba(167,139,250,0.12), transparent 60%),
        linear-gradient(135deg, var(--bg1), var(--bg2));
      min-height: 100vh;
    }

    a { color: inherit; }

    .container {
      max-width: var(--max);
      margin: 0 auto;
      padding: 0 20px;
    }

    /* Top bar */
    .topbar {
      position: sticky;
      top: 0;
      z-index: 20;
      backdrop-filter: blur(10px);
      background: rgba(7, 26, 43, 0.55);
      border-bottom: 1px solid rgba(255,255,255,0.08);
    }
    .topbar-inner {
      display: flex;
      align-items: center;
      justify-content: space-between;
      gap: 14px;
      padding: 14px 0;
    }
    .brand {
      display: flex;
      align-items: center;
      gap: 10px;
      text-decoration: none;
    }
    .brand-badge {
      width: 34px;
      height: 34px;
      border-radius: 10px;
      background: linear-gradient(135deg, rgba(94,234,212,0.85), rgba(147,197,253,0.85));
      box-shadow: 0 10px 25px rgba(0,0,0,0.25);
    }
    .brand strong {
      letter-spacing: 0.2px;
      font-size: 0.98rem;
    }
    nav {
      display: none;
      gap: 16px;
      font-size: 0.95rem;
      color: var(--muted);
    }
    nav a {
      text-decoration: none;
      opacity: 0.9;
    }
    nav a:hover { opacity: 1; color: var(--text); }

    .btn {
      display: inline-flex;
      align-items: center;
      justify-content: center;
      gap: 10px;
      padding: 12px 18px;
      border-radius: 999px;
      border: 1px solid rgba(255,255,255,0.14);
      text-decoration: none;
      font-weight: 650;
      letter-spacing: 0.2px;
      transition: transform .12s ease, background .12s ease, border-color .12s ease;
      user-select: none;
      white-space: nowrap;
    }

    .btn:hover { transform: translateY(-1px); border-color: rgba(255,255,255,0.22); }

    .btn-primary {
      background: linear-gradient(135deg, rgba(94,234,212,0.95), rgba(147,197,253,0.95));
      color: rgba(4, 18, 22, 0.98);
      box-shadow: 0 14px 34px rgba(0,0,0,0.22);
    }

    .btn-ghost {
      background: rgba(255,255,255,0.06);
      color: var(--text);
    }

    /* Hero */
    .hero {
      padding: 64px 0 36px;
    }

    .hero-grid {
      display: grid;
      grid-template-columns: 1fr;
      gap: 22px;
      align-items: start;
    }

    .kicker {
      display: inline-flex;
      align-items: center;
      gap: 10px;
      padding: 8px 12px;
      border-radius: 999px;
      background: rgba(255,255,255,0.06);
      border: 1px solid rgba(255,255,255,0.10);
      color: var(--muted);
      font-size: 0.95rem;
      width: fit-content;
    }

    .dot {
      width: 9px; height: 9px;
      border-radius: 50%;
      background: var(--accent);
      box-shadow: 0 0 0 6px rgba(94,234,212,0.18);
    }

    h1 {
      margin: 14px 0 10px;
      font-size: clamp(2.2rem, 4.2vw, 3.2rem);
      line-height: 1.08;
      letter-spacing: -0.6px;
    }

    .hero p {
      margin: 0;
      max-width: 62ch;
      color: var(--muted);
      font-size: 1.06rem;
    }

    .hero-actions {
      display: flex;
      flex-wrap: wrap;
      gap: 12px;
      margin-top: 22px;
    }

    .trust {
      display: flex;
      flex-wrap: wrap;
      gap: 10px;
      margin-top: 18px;
      color: var(--muted2);
      font-size: 0.95rem;
    }

    .pill {
      padding: 8px 12px;
      border-radius: 999px;
      border: 1px solid rgba(255,255,255,0.10);
      background: rgba(255,255,255,0.05);
    }

    .card {
      background: var(--card);
      border: 1px solid rgba(255,255,255,0.10);
      border-radius: var(--radius2);
      box-shadow: var(--shadow);
    }

    .book {
      padding: 18px;
      position: relative;
      overflow: hidden;
    }

    .book::before {
      content: "";
      position: absolute;
      inset: -120px -120px auto auto;
      width: 260px;
      height: 260px;
      background: radial-gradient(circle at 30% 30%, rgba(94,234,212,0.35), transparent 60%);
      filter: blur(10px);
    }

    .book-inner {
      display: grid;
      grid-template-columns: 1fr;
      gap: 14px;
      position: relative;
      z-index: 1;
    }

    .book-title {
      font-weight: 800;
      font-size: 1.2rem;
      letter-spacing: -0.2px;
      margin: 0;
    }

    .book-sub {
      margin: 0;
      color: var(--muted);
    }

    .mini-grid {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 10px;
      margin-top: 10px;
    }

    .mini {
      padding: 12px 12px;
      border-radius: 14px;
      background: rgba(255,255,255,0.06);
      border: 1px solid rgba(255,255,255,0.10);
      color: var(--muted);
      font-size: 0.95rem;
    }

    .mini strong { color: var(--text); }

    /* Sections */
    section {
      padding: 42px 0;
    }

    .section-head {
      display: flex;
      flex-direction: column;
      gap: 10px;
      margin-bottom: 18px;
    }

    .section-head h2 {
      margin: 0;
      font-size: 1.85rem;
      letter-spacing: -0.4px;
    }

    .section-head p {
      margin: 0;
      color: var(--muted);
      max-width: 74ch;
    }

    .grid {
      display: grid;
      grid-template-columns: 1fr;
      gap: 14px;
    }

    .feature {
      padding: 18px;
      border-radius: var(--radius);
      background: var(--card);
      border: 1px solid rgba(255,255,255,0.10);
    }

    .feature h3 {
      margin: 0 0 8px;
      font-size: 1.05rem;
      letter-spacing: -0.2px;
    }

    .feature p {
      margin: 0;
      color: var(--muted);
    }

    .two {
      display: grid;
      grid-template-columns: 1fr;
      gap: 14px;
    }

    .list {
      margin: 0;
      padding-left: 18px;
      color: var(--muted);
    }

    .list li { margin: 10px 0; }

    /* Pricing */
    .pricing {
      padding: 22px;
    }

    .price {
      display: flex;
      align-items: baseline;
      gap: 10px;
      margin: 6px 0 14px;
    }

    .price .value {
      font-size: 2.4rem;
      font-weight: 900;
      letter-spacing: -0.8px;
    }

    .price .note {
      color: var(--muted);
    }

    .fine {
      color: var(--muted2);
      font-size: 0.95rem;
      margin-top: 12px;
    }

    /* FAQ */
    details {
      background: rgba(255,255,255,0.06);
      border: 1px solid rgba(255,255,255,0.10);
      border-radius: 14px;
      padding: 14px 14px;
    }

    summary {
      cursor: pointer;
      font-weight: 700;
      color: var(--text);
      list-style: none;
    }

    summary::-webkit-details-marker { display: none; }

    details p {
      margin: 10px 0 0;
      color: var(--muted);
    }

    /* Footer */
    footer {
      padding: 34px 0 60px;
      border-top: 1px solid rgba(255,255,255,0.08);
      background: rgba(2,6,23,0.25);
    }

    .footer-grid {
      display: grid;
      grid-template-columns: 1fr;
