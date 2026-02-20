<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Everyday Work and Industrial Modernity: Labour, Space, and Urban Life in London, Ontario (1910–1930)</title>
  <style>
    :root {
      --bg: #07080c;
      --panel: #0f121b;
      --panel2: #0c0f17;
      --text: #f0f1f3;
      --muted: #b7bcc9;
      --line: #22283a;
      --accent: #8aa4ff;
      --shadow: 0 10px 30px rgba(0,0,0,0.5);
      --radius: 18px;
    }
    * { box-sizing: border-box; }
    body {
      margin: 0;
      font-family: ui-sans-serif, system-ui, -apple-system, Segoe UI, Roboto, Helvetica, Arial;
      background: radial-gradient(1200px 600px at 20% 0%, rgba(138,164,255,0.12), transparent 55%),
                  radial-gradient(900px 500px at 90% 10%, rgba(255,255,255,0.06), transparent 60%),
                  var(--bg);
      color: var(--text);
      line-height: 1.55;
    }
    a { color: var(--accent); text-decoration: none; }
    a:hover { text-decoration: underline; }
    .wrap { max-width: 1120px; margin: 0 auto; padding: 0 20px; }
    header {
      padding: 54px 0 22px;
    }
    .hero {
      background: linear-gradient(180deg, rgba(255,255,255,0.04), rgba(255,255,255,0.01));
      border: 1px solid var(--line);
      border-radius: var(--radius);
      padding: 26px 22px 18px;
      box-shadow: var(--shadow);
    }
    h1 {
      margin: 0;
      font-size: clamp(30px, 3.2vw, 46px);
      letter-spacing: -0.02em;
      line-height: 1.1;
    }
    .subtitle {
      margin-top: 8px;
      color: var(--muted);
      font-size: 15.5px;
    }
    .statement {
      margin-top: 14px;
      color: var(--text);
      max-width: 95ch;
      font-size: 15.5px;
    }
    .meta {
      display: flex;
      flex-wrap: wrap;
      gap: 10px 14px;
      margin-top: 16px;
      padding-top: 14px;
      border-top: 1px solid var(--line);
      color: var(--muted);
      font-size: 13px;
    }
    .pill {
      border: 1px solid var(--line);
      background: rgba(255,255,255,0.02);
      padding: 6px 10px;
      border-radius: 999px;
    }
    nav {
      margin-top: 14px;
      display: flex;
      flex-wrap: wrap;
      gap: 10px;
    }
    nav a {
      display: inline-flex;
      align-items: center;
      gap: 8px;
      padding: 8px 12px;
      border-radius: 999px;
      border: 1px solid var(--line);
      background: rgba(255,255,255,0.02);
      color: var(--text);
      font-size: 13px;
    }
    nav a:hover { background: rgba(138,164,255,0.08); text-decoration: none; }
    main { padding: 18px 0 70px; }
    section {
      margin-top: 26px;
      padding: 18px;
      border: 1px solid var(--line);
      border-radius: var(--radius);
      background: rgba(255,255,255,0.02);
      box-shadow: var(--shadow);
    }
    h2 {
      margin: 0;
      font-size: 20px;
      letter-spacing: -0.01em;
    }
    .blurb {
      margin: 8px 0 14px;
      color: var(--muted);
      max-width: 95ch;
      font-size: 14.5px;
    }
    .grid {
      display: grid;
      grid-template-columns: repeat(auto-fill, minmax(220px, 1fr));
      gap: 12px;
    }
    figure {
      margin: 0;
      border: 1px solid var(--line);
      border-radius: 14px;
      overflow: hidden;
      background: var(--panel);
    }
    figure button {
      all: unset;
      cursor: zoom-in;
      display: block;
      width: 100%;
    }
    figure img {
      width: 100%;
      height: 210px;
      object-fit: cover;
      display: block;
      background: var(--panel2);
    }
    figcaption {
      padding: 10px 12px 12px;
      color: var(--muted);
      font-size: 13px;
    }
    .cap-title {
      color: var(--text);
      font-weight: 650;
      margin-bottom: 4px;
    }
    .placeholder {
      margin-top: 6px;
      font-size: 12.5px;
      color: var(--muted);
      opacity: 0.95;
    }
    .callout {
      margin-top: 14px;
      padding: 12px 12px;
      border: 1px dashed var(--line);
      border-radius: 14px;
      color: var(--muted);
      background: rgba(255,255,255,0.01);
      font-size: 13px;
    }
    footer {
      margin-top: 26px;
      color: var(--muted);
      font-size: 13px;
      padding: 18px 0 0;
    }
    /* Lightbox */
    .lightbox {
      position: fixed;
      inset: 0;
      background: rgba(0,0,0,0.78);
      display: none;
      align-items: center;
      justify-content: center;
      padding: 24px;
      z-index: 999;
    }
    .lightbox.open { display: flex; }
    .lb-card {
      width: min(1100px, 96vw);
      background: #0a0c12;
      border: 1px solid var(--line);
      border-radius: var(--radius);
      overflow: hidden;
      box-shadow: var(--shadow);
    }
    .lb-top {
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding: 12px 14px;
      border-bottom: 1px solid var(--line);
      color: var(--muted);
      font-size: 13px;
    }
    .lb-close {
      cursor: pointer;
      border: 1px solid var(--line);
      background: rgba(255,255,255,0.02);
      color: var(--text);
      padding: 6px 10px;
      border-radius: 999px;
    }
    .lb-img {
      width: 100%;
      max-height: 74vh;
      object-fit: contain;
      display: block;
      background: #05060a;
    }
    .lb-cap {
      padding: 12px 14px 16px;
      border-top: 1px solid var(--line);
      color: var(--muted);
      font-size: 13px;
    }
    .lb-cap strong { color: var(--text); }
  </style>
</head>
<body>
  <header class="wrap">
    <div class="hero">
      <h1>Everyday Work and Industrial Modernity</h1>
      <div class="subtitle">Labour, Space, and Urban Life in London, Ontario (1910–1930)</div>
      <p class="statement">This exhibition explores how everyday work shaped urban life in London, Ontario between 1910 and 1930. Drawing on archival photographs from Western Archives (Access to Memory), it examines factories, workshops, and commercial interiors as environments where labour, technology, and social organization intersected. Inspired by online archival exhibitions that treat photographs as historical evidence—rather than simple illustration—this project foregrounds how work becomes visible through space: machines, counters, tools, and bodies arranged for production. Across four sections, the photographs reveal the material conditions of labour and the ways industrial modernity reorganized the city’s everyday rhythms.</p>
      <div class="meta">
        <span class="pill">Format: Online Exhibition</span>
        <span class="pill">Items: 23 archival photographs</span>
        <span class="pill">Date range: 1910–1930</span>
        <span class="pill">Built: 2026-02-20</span>
      </div>
      <nav>
        <a href="#s1">1 · Work in Public</a>
        <a href="#s2">2 · Collective Identity</a>
        <a href="#s3">3 · Work with Machines</a>
        <a href="#s4">4 · Work as Skill</a>
      </nav>
      <div class="callout">Editing tip: Replace each placeholder caption with the official archival title, date, and reference code from your Archive Tracker or AtoM record page.</div>
    </div>
  </header>

  <main class="wrap">
<section id="s1">
      <h2>Work in Public: Small Businesses and Retail Interiors</h2>
      <p class="blurb">Shops and small businesses made labour visible in public. Counters, displays, and decorated interiors show how commerce blended workplace and social space—often family-run, seasonal, and tied to neighbourhood routines.</p>
      <div class="grid">

        <figure>
          <button class="open" data-src="assets/AFC_341-S3-I12_141.jpg" data-title="Work in Public: Small Businesses and Retail Interiors — Item 1" data-cap="Retail or service interior; a workplace designed for visibility and exchange.">
            <img src="assets/AFC_341-S3-I12_141.jpg" alt="Work in Public: Small Businesses and Retail Interiors — Item 1">
          </button>
          <figcaption>
            <div class="cap-title">Work in Public: Small Businesses and Retail Interiors — Item 1</div>
            <div>Retail or service interior; a workplace designed for visibility and exchange.</div>
            <div class="placeholder">Archival title/date: <em>[replace]</em> · Reference code: <em>[replace]</em></div>
          </figcaption>
        </figure>

        <figure>
          <button class="open" data-src="assets/AFC_341-S3-I14_141.jpg" data-title="Work in Public: Small Businesses and Retail Interiors — Item 2" data-cap="Retail or service interior; a workplace designed for visibility and exchange.">
            <img src="assets/AFC_341-S3-I14_141.jpg" alt="Work in Public: Small Businesses and Retail Interiors — Item 2">
          </button>
          <figcaption>
            <div class="cap-title">Work in Public: Small Businesses and Retail Interiors — Item 2</div>
            <div>Retail or service interior; a workplace designed for visibility and exchange.</div>
            <div class="placeholder">Archival title/date: <em>[replace]</em> · Reference code: <em>[replace]</em></div>
          </figcaption>
        </figure>

        <figure>
          <button class="open" data-src="assets/AFC_341-S3-I16_141.jpg" data-title="Work in Public: Small Businesses and Retail Interiors — Item 3" data-cap="Retail or service interior; a workplace designed for visibility and exchange.">
            <img src="assets/AFC_341-S3-I16_141.jpg" alt="Work in Public: Small Businesses and Retail Interiors — Item 3">
          </button>
          <figcaption>
            <div class="cap-title">Work in Public: Small Businesses and Retail Interiors — Item 3</div>
            <div>Retail or service interior; a workplace designed for visibility and exchange.</div>
            <div class="placeholder">Archival title/date: <em>[replace]</em> · Reference code: <em>[replace]</em></div>
          </figcaption>
        </figure>

        <figure>
          <button class="open" data-src="assets/AFC_341-S3-I19_141.jpg" data-title="Work in Public: Small Businesses and Retail Interiors — Item 4" data-cap="Retail or service interior; a workplace designed for visibility and exchange.">
            <img src="assets/AFC_341-S3-I19_141.jpg" alt="Work in Public: Small Businesses and Retail Interiors — Item 4">
          </button>
          <figcaption>
            <div class="cap-title">Work in Public: Small Businesses and Retail Interiors — Item 4</div>
            <div>Retail or service interior; a workplace designed for visibility and exchange.</div>
            <div class="placeholder">Archival title/date: <em>[replace]</em> · Reference code: <em>[replace]</em></div>
          </figcaption>
        </figure>

        <figure>
          <button class="open" data-src="assets/AFC_341-S3-I29_141.jpg" data-title="Work in Public: Small Businesses and Retail Interiors — Item 5" data-cap="Butcher shop interior or retail workspace; tools and products shape the work environment.">
            <img src="assets/AFC_341-S3-I29_141.jpg" alt="Work in Public: Small Businesses and Retail Interiors — Item 5">
          </button>
          <figcaption>
            <div class="cap-title">Work in Public: Small Businesses and Retail Interiors — Item 5</div>
            <div>Butcher shop interior or retail workspace; tools and products shape the work environment.</div>
            <div class="placeholder">Archival title/date: <em>[replace]</em> · Reference code: <em>[replace]</em></div>
          </figcaption>
        </figure>

        <figure>
          <button class="open" data-src="assets/AFC_341-S3-I47_141.jpg" data-title="Work in Public: Small Businesses and Retail Interiors — Item 6" data-cap="Commercial interior emphasizing display, inventory, and customer-facing labour.">
            <img src="assets/AFC_341-S3-I47_141.jpg" alt="Work in Public: Small Businesses and Retail Interiors — Item 6">
          </button>
          <figcaption>
            <div class="cap-title">Work in Public: Small Businesses and Retail Interiors — Item 6</div>
            <div>Commercial interior emphasizing display, inventory, and customer-facing labour.</div>
            <div class="placeholder">Archival title/date: <em>[replace]</em> · Reference code: <em>[replace]</em></div>
          </figcaption>
        </figure>

        <figure>
          <button class="open" data-src="assets/AFC_341-S3-I4_141.jpg" data-title="Work in Public: Small Businesses and Retail Interiors — Item 7" data-cap="Retail or service interior; a workplace designed for visibility and exchange.">
            <img src="assets/AFC_341-S3-I4_141.jpg" alt="Work in Public: Small Businesses and Retail Interiors — Item 7">
          </button>
          <figcaption>
            <div class="cap-title">Work in Public: Small Businesses and Retail Interiors — Item 7</div>
            <div>Retail or service interior; a workplace designed for visibility and exchange.</div>
            <div class="placeholder">Archival title/date: <em>[replace]</em> · Reference code: <em>[replace]</em></div>
          </figcaption>
        </figure>

        <figure>
          <button class="open" data-src="assets/AFC_341-S4-SS1-I38_141.jpg" data-title="Work in Public: Small Businesses and Retail Interiors — Item 8" data-cap="Exterior view connecting work to streetscape and urban circulation.">
            <img src="assets/AFC_341-S4-SS1-I38_141.jpg" alt="Work in Public: Small Businesses and Retail Interiors — Item 8">
          </button>
          <figcaption>
            <div class="cap-title">Work in Public: Small Businesses and Retail Interiors — Item 8</div>
            <div>Exterior view connecting work to streetscape and urban circulation.</div>
            <div class="placeholder">Archival title/date: <em>[replace]</em> · Reference code: <em>[replace]</em></div>
          </figcaption>
        </figure>
      </div>
    </section>
<section id="s2">
      <h2>Work as Collective Identity: The Industrial Workforce</h2>
      <p class="blurb">Group portraits emphasize labour as collective identity. Rather than highlighting individuals, the image frames workers as a coordinated workforce—a social formation created by industrial organization.</p>
      <div class="grid">

        <figure>
          <button class="open" data-src="assets/AFC_341-S8-I5_141.jpg" data-title="Work as Collective Identity: The Industrial Workforce — Item 1" data-cap="Group portrait of workers; labour represented as collective participation.">
            <img src="assets/AFC_341-S8-I5_141.jpg" alt="Work as Collective Identity: The Industrial Workforce — Item 1">
          </button>
          <figcaption>
            <div class="cap-title">Work as Collective Identity: The Industrial Workforce — Item 1</div>
            <div>Group portrait of workers; labour represented as collective participation.</div>
            <div class="placeholder">Archival title/date: <em>[replace]</em> · Reference code: <em>[replace]</em></div>
          </figcaption>
        </figure>
      </div>
    </section>
<section id="s3">
      <h2>Work with Machines: Factory Interiors and Mechanized Systems</h2>
      <p class="blurb">These photographs place workers inside machine-centered environments. Belts, frames, and production equipment structure the scene, revealing how industrial modernity reorganized bodies, time, and space for output and efficiency.</p>
      <div class="grid">

        <figure>
          <button class="open" data-src="assets/AFC_341-S8-I10_141.jpg" data-title="Work with Machines: Factory Interiors and Mechanized Systems — Item 1" data-cap="Factory interior showing workers positioned within machinery and production systems.">
            <img src="assets/AFC_341-S8-I10_141.jpg" alt="Work with Machines: Factory Interiors and Mechanized Systems — Item 1">
          </button>
          <figcaption>
            <div class="cap-title">Work with Machines: Factory Interiors and Mechanized Systems — Item 1</div>
            <div>Factory interior showing workers positioned within machinery and production systems.</div>
            <div class="placeholder">Archival title/date: <em>[replace]</em> · Reference code: <em>[replace]</em></div>
          </figcaption>
        </figure>

        <figure>
          <button class="open" data-src="assets/AFC_341-S8-I11_141.jpg" data-title="Work with Machines: Factory Interiors and Mechanized Systems — Item 2" data-cap="Factory interior showing workers positioned within machinery and production systems.">
            <img src="assets/AFC_341-S8-I11_141.jpg" alt="Work with Machines: Factory Interiors and Mechanized Systems — Item 2">
          </button>
          <figcaption>
            <div class="cap-title">Work with Machines: Factory Interiors and Mechanized Systems — Item 2</div>
            <div>Factory interior showing workers positioned within machinery and production systems.</div>
            <div class="placeholder">Archival title/date: <em>[replace]</em> · Reference code: <em>[replace]</em></div>
          </figcaption>
        </figure>

        <figure>
          <button class="open" data-src="assets/AFC_341-S8-I16_141.jpg" data-title="Work with Machines: Factory Interiors and Mechanized Systems — Item 3" data-cap="Factory interior showing workers positioned within machinery and production systems.">
            <img src="assets/AFC_341-S8-I16_141.jpg" alt="Work with Machines: Factory Interiors and Mechanized Systems — Item 3">
          </button>
          <figcaption>
            <div class="cap-title">Work with Machines: Factory Interiors and Mechanized Systems — Item 3</div>
            <div>Factory interior showing workers positioned within machinery and production systems.</div>
            <div class="placeholder">Archival title/date: <em>[replace]</em> · Reference code: <em>[replace]</em></div>
          </figcaption>
        </figure>

        <figure>
          <button class="open" data-src="assets/AFC_341-S8-I17_141.jpg" data-title="Work with Machines: Factory Interiors and Mechanized Systems — Item 4" data-cap="Factory interior showing workers positioned within machinery and production systems.">
            <img src="assets/AFC_341-S8-I17_141.jpg" alt="Work with Machines: Factory Interiors and Mechanized Systems — Item 4">
          </button>
          <figcaption>
            <div class="cap-title">Work with Machines: Factory Interiors and Mechanized Systems — Item 4</div>
            <div>Factory interior showing workers positioned within machinery and production systems.</div>
            <div class="placeholder">Archival title/date: <em>[replace]</em> · Reference code: <em>[replace]</em></div>
          </figcaption>
        </figure>

        <figure>
          <button class="open" data-src="assets/AFC_341-S8-I18_141.jpg" data-title="Work with Machines: Factory Interiors and Mechanized Systems — Item 5" data-cap="Factory interior showing workers positioned within machinery and production systems.">
            <img src="assets/AFC_341-S8-I18_141.jpg" alt="Work with Machines: Factory Interiors and Mechanized Systems — Item 5">
          </button>
          <figcaption>
            <div class="cap-title">Work with Machines: Factory Interiors and Mechanized Systems — Item 5</div>
            <div>Factory interior showing workers positioned within machinery and production systems.</div>
            <div class="placeholder">Archival title/date: <em>[replace]</em> · Reference code: <em>[replace]</em></div>
          </figcaption>
        </figure>

        <figure>
          <button class="open" data-src="assets/AFC_341-S8-I19_141.jpg" data-title="Work with Machines: Factory Interiors and Mechanized Systems — Item 6" data-cap="Factory interior showing workers positioned within machinery and production systems.">
            <img src="assets/AFC_341-S8-I19_141.jpg" alt="Work with Machines: Factory Interiors and Mechanized Systems — Item 6">
          </button>
          <figcaption>
            <div class="cap-title">Work with Machines: Factory Interiors and Mechanized Systems — Item 6</div>
            <div>Factory interior showing workers positioned within machinery and production systems.</div>
            <div class="placeholder">Archival title/date: <em>[replace]</em> · Reference code: <em>[replace]</em></div>
          </figcaption>
        </figure>

        <figure>
          <button class="open" data-src="assets/AFC_341-S8-I20_141.jpg" data-title="Work with Machines: Factory Interiors and Mechanized Systems — Item 7" data-cap="Factory interior showing workers positioned within machinery and production systems.">
            <img src="assets/AFC_341-S8-I20_141.jpg" alt="Work with Machines: Factory Interiors and Mechanized Systems — Item 7">
          </button>
          <figcaption>
            <div class="cap-title">Work with Machines: Factory Interiors and Mechanized Systems — Item 7</div>
            <div>Factory interior showing workers positioned within machinery and production systems.</div>
            <div class="placeholder">Archival title/date: <em>[replace]</em> · Reference code: <em>[replace]</em></div>
          </figcaption>
        </figure>

        <figure>
          <button class="open" data-src="assets/AFC_341-S8-I21_141.jpg" data-title="Work with Machines: Factory Interiors and Mechanized Systems — Item 8" data-cap="Factory interior showing workers positioned within machinery and production systems.">
            <img src="assets/AFC_341-S8-I21_141.jpg" alt="Work with Machines: Factory Interiors and Mechanized Systems — Item 8">
          </button>
          <figcaption>
            <div class="cap-title">Work with Machines: Factory Interiors and Mechanized Systems — Item 8</div>
            <div>Factory interior showing workers positioned within machinery and production systems.</div>
            <div class="placeholder">Archival title/date: <em>[replace]</em> · Reference code: <em>[replace]</em></div>
          </figcaption>
        </figure>

        <figure>
          <button class="open" data-src="assets/AFC_341-S8-I29_141.jpg" data-title="Work with Machines: Factory Interiors and Mechanized Systems — Item 9" data-cap="Factory interior showing workers positioned within machinery and production systems.">
            <img src="assets/AFC_341-S8-I29_141.jpg" alt="Work with Machines: Factory Interiors and Mechanized Systems — Item 9">
          </button>
          <figcaption>
            <div class="cap-title">Work with Machines: Factory Interiors and Mechanized Systems — Item 9</div>
            <div>Factory interior showing workers positioned within machinery and production systems.</div>
            <div class="placeholder">Archival title/date: <em>[replace]</em> · Reference code: <em>[replace]</em></div>
          </figcaption>
        </figure>

        <figure>
          <button class="open" data-src="assets/AFC_341-S8-I2_141.jpg" data-title="Work with Machines: Factory Interiors and Mechanized Systems — Item 10" data-cap="Factory interior showing workers positioned within machinery and production systems.">
            <img src="assets/AFC_341-S8-I2_141.jpg" alt="Work with Machines: Factory Interiors and Mechanized Systems — Item 10">
          </button>
          <figcaption>
            <div class="cap-title">Work with Machines: Factory Interiors and Mechanized Systems — Item 10</div>
            <div>Factory interior showing workers positioned within machinery and production systems.</div>
            <div class="placeholder">Archival title/date: <em>[replace]</em> · Reference code: <em>[replace]</em></div>
          </figcaption>
        </figure>

        <figure>
          <button class="open" data-src="assets/AFC_341-S8-I3_141.jpg" data-title="Work with Machines: Factory Interiors and Mechanized Systems — Item 11" data-cap="Factory interior showing workers positioned within machinery and production systems.">
            <img src="assets/AFC_341-S8-I3_141.jpg" alt="Work with Machines: Factory Interiors and Mechanized Systems — Item 11">
          </button>
          <figcaption>
            <div class="cap-title">Work with Machines: Factory Interiors and Mechanized Systems — Item 11</div>
            <div>Factory interior showing workers positioned within machinery and production systems.</div>
            <div class="placeholder">Archival title/date: <em>[replace]</em> · Reference code: <em>[replace]</em></div>
          </figcaption>
        </figure>

        <figure>
          <button class="open" data-src="assets/AFC_341-S8-I9_141.jpg" data-title="Work with Machines: Factory Interiors and Mechanized Systems — Item 12" data-cap="Factory interior showing workers positioned within machinery and production systems.">
            <img src="assets/AFC_341-S8-I9_141.jpg" alt="Work with Machines: Factory Interiors and Mechanized Systems — Item 12">
          </button>
          <figcaption>
            <div class="cap-title">Work with Machines: Factory Interiors and Mechanized Systems — Item 12</div>
            <div>Factory interior showing workers positioned within machinery and production systems.</div>
            <div class="placeholder">Archival title/date: <em>[replace]</em> · Reference code: <em>[replace]</em></div>
          </figcaption>
        </figure>
      </div>
    </section>
<section id="s4">
      <h2>Work as Skill: Craft, Repair, and Material Transformation</h2>
      <p class="blurb">Workshop scenes foreground embodied skill: tools, heat, and hands-on expertise. Here, labour appears as craft and material transformation—a reminder that modern cities relied on both mechanized systems and specialized manual knowledge.</p>
      <div class="grid">

        <figure>
          <button class="open" data-src="assets/AFC_341-S16-I2_141.jpg" data-title="Work as Skill: Craft, Repair, and Material Transformation — Item 1" data-cap="Workshop/forge scene highlighting skilled manual labour and material transformation.">
            <img src="assets/AFC_341-S16-I2_141.jpg" alt="Work as Skill: Craft, Repair, and Material Transformation — Item 1">
          </button>
          <figcaption>
            <div class="cap-title">Work as Skill: Craft, Repair, and Material Transformation — Item 1</div>
            <div>Workshop/forge scene highlighting skilled manual labour and material transformation.</div>
            <div class="placeholder">Archival title/date: <em>[replace]</em> · Reference code: <em>[replace]</em></div>
          </figcaption>
        </figure>

        <figure>
          <button class="open" data-src="assets/AFC_341-S16-I3_141.jpg" data-title="Work as Skill: Craft, Repair, and Material Transformation — Item 2" data-cap="Workshop/forge scene highlighting skilled manual labour and material transformation.">
            <img src="assets/AFC_341-S16-I3_141.jpg" alt="Work as Skill: Craft, Repair, and Material Transformation — Item 2">
          </button>
          <figcaption>
            <div class="cap-title">Work as Skill: Craft, Repair, and Material Transformation — Item 2</div>
            <div>Workshop/forge scene highlighting skilled manual labour and material transformation.</div>
            <div class="placeholder">Archival title/date: <em>[replace]</em> · Reference code: <em>[replace]</em></div>
          </figcaption>
        </figure>
      </div>
    </section>

    <footer>
      <p><strong>Credits &amp; Use</strong><br/>
      Images are sourced from Western Archives (Access to Memory) and are included here for course-related research/curation purposes.
      Please follow Western Archives’ reproduction and citation guidelines for any public sharing beyond the course context.</p>

      <p><strong>Suggested citation format (edit):</strong><br/>
      Western Archives, University of Western Ontario, <em>[Collection name]</em>, <em>[Reference code]</em>, <em>[Item title]</em>, <em>[Date]</em>.</p>
    </footer>
  </main>

  <div class="lightbox" id="lightbox" aria-hidden="true">
    <div class="lb-card" role="dialog" aria-modal="true">
      <div class="lb-top">
        <div id="lbTitle">Image</div>
        <button class="lb-close" id="lbClose" aria-label="Close">Close</button>
      </div>
      <img class="lb-img" id="lbImg" src="" alt="">
      <div class="lb-cap" id="lbCap"></div>
    </div>
  </div>

  <script>
    const lb = document.getElementById('lightbox');
    const lbImg = document.getElementById('lbImg');
    const lbTitle = document.getElementById('lbTitle');
    const lbCap = document.getElementById('lbCap');
    const lbClose = document.getElementById('lbClose');

    function openLightbox(src, title, cap) {
      lb.classList.add('open');
      lb.setAttribute('aria-hidden', 'false');
      lbImg.src = src;
      lbImg.alt = title || 'Image';
      lbTitle.textContent = title || 'Image';
      lbCap.innerHTML = '<strong>' + (title || 'Image') + '</strong><br/>' + (cap || '');
    }

    function closeLightbox() {
      lb.classList.remove('open');
      lb.setAttribute('aria-hidden', 'true');
      lbImg.src = '';
    }

    document.querySelectorAll('button.open').forEach(btn => {
      btn.addEventListener('click', () => {
        openLightbox(btn.dataset.src, btn.dataset.title, btn.dataset.cap);
      });
    });

    lbClose.addEventListener('click', closeLightbox);
    lb.addEventListener('click', (e) => {
      if (e.target === lb) closeLightbox();
    });
    document.addEventListener('keydown', (e) => {
      if (e.key === 'Escape') closeLightbox();
    });
  </script>
</body>
</html>
