## T — Task & C — Context
*   **Tech Stack:** HTML5 (Strictly Semantic), CSS3 (Modern Flex/Grid).
*   **Approach:** Mobile-first, *zero-dependency* (tanpa framework luar biar *lightweight*).
*   **Target:** Startup Tech Lead yang nyari ketelitian dalam struktur kode.

## C — Constraints
*   **Strict Semantic:** Penggunaan `<section>`, `<article>`, `<header>`, `<nav>`, dan `<footer>`.
*   **No Div-Soup:** `<div>` hanya digunakan jika benar-benar tidak ada elemen semantik yang mewakili fungsi layouting tersebut.
*   **Accessibility:** Wajib ada `alt` text, kontras warna yang pas, dan *focus states*.

## O — Output
HTML dan CSS (Embedded) biar lo bisa langsung *preview* di satu file.

```html
<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Rizki R | Backend Engineer & AI Specialist</title>
    <!-- Font: Plus Jakarta Sans for Headers, Inter for Body -->
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500&family=Plus+Jakarta+Sans:wght@700;800&family=JetBrains+Mono&display=swap" rel="stylesheet">
    <style>
        :root {
            --bg-color: #F8FAFC; /* Ghost White[cite: 1] */
            --text-main: #0F172A; /* Slate Navy[cite: 1] */
            --text-sub: #64748B; /* Steel Gray[cite: 1] */
            --accent: #6366F1;
            --border: #E2E8F0;
        }

        * { margin: 0; padding: 0; box-sizing: border-box; }

        body {
            background-color: var(--bg-color);
            color: var(--text-main);
            font-family: 'Inter', sans-serif;
            line-height: 1.6;
            padding: 1.5rem;
        }

        h1, h2, h3 { font-family: 'Plus Jakarta Sans', sans-serif; }

        /* Header & Hero */
        header {
            padding: 2rem 0;
            border-bottom: 1px solid var(--border);
        }

        .hero h1 { font-size: 2.5rem; letter-spacing: -0.02em; margin-bottom: 0.5rem; }
        .hero p { color: var(--text-sub); font-size: 1.1rem; max-width: 500px; }

        /* Main Content */
        main { max-width: 800px; margin: 0 auto; }

        section { margin: 4rem 0; }
        h2 { font-size: 1.5rem; margin-bottom: 1.5rem; display: flex; align-items: center; gap: 0.5rem; }
        h2::after { content: ""; height: 1px; background: var(--border); flex-grow: 1; }

        /* Project Cards */
        article {
            background: white;
            border: 1px solid var(--border);
            border-radius: 12px;
            padding: 1.5rem;
            margin-bottom: 1.5rem;
            transition: transform 0.2s ease;
        }

        article:hover { transform: translateY(-4px); border-color: var(--accent); }

        .tech-stack {
            font-family: 'JetBrains Mono', monospace;
            font-size: 0.8rem;
            color: var(--accent);
            margin-top: 1rem;
            display: block;
        }

        /* Unique Element: Status API[cite: 1] */
        .api-status {
            background: #1e293b;
            color: #94a3b8;
            padding: 1rem;
            border-radius: 8px;
            font-family: 'JetBrains Mono', monospace;
            font-size: 0.85rem;
            overflow-x: auto;
        }

        .api-status span { color: #38bdf8; }

        /* Mobile First adjustments */
        @media (min-width: 768px) {
            body { padding: 4rem; }
            .hero h1 { font-size: 3.5rem; }
        }
    </style>
</head>
<body>

    <header role="banner">
        <div class="hero">
            <h1>Rizki R.</h1>
            <p>Backend Engineer building scalable systems with Go, Python, and TypeScript. Focused on AI integration and performance.</p>
        </div>
    </header>

    <main>
        <!-- Unique Element Section -->
        <section id="status">
            <h2>Current Status</h2>
            <pre class="api-status">
<code>{
  "status": "<span>Looking for opportunities</span>",
  "stack": ["Go", "FastAPI", "PostgreSQL"],
  "latest_focus": "Quantum-Resistant Auth"
}</code></pre>
        </section>

        <section id="projects">
            <h2>Selected Projects</h2>
            
            <article>
                <h3>Quantum-Resistant Auth Service</h3>
                <p>Designed a secure authentication layer using Go to demonstrate proactive security against future computing threats.</p>
                <span class="tech-stack">Go • PostgreSQL • Redis</span>
            </article>

            <article>
                <h3>AI-Driven Sentiment Pipeline</h3>
                <p>An automated pipeline that scrapes crypto news and generates real-time sentiment analysis via LLMs.</p>
                <span class="tech-stack">Python • FastAPI • OpenAI API</span>
            </article>
        </section>

        <section id="skills">
            <h2>Skills & Tools</h2>
            <p><strong>Languages:</strong> Go, Python, JavaScript, TypeScript.</p>
            <p><strong>Infrastructure:</strong> PostgreSQL, Docker, Linux (Debian).</p>
        </section>
    </main>

    <footer role="contentinfo">
        <p>&copy; 2026 Rizki R. Built with semantic HTML.</p>
    </footer>

</body>
</html>
```