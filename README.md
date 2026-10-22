<!DOCTYPE html>
<html lang="id">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Violet White Logo Preview</title>
    <link rel="stylesheet" href="colors.css" />
    <style>
      * { box-sizing: border-box; }

      body {
        margin: 0;
        min-height: 100vh;
        display: grid;
        place-items: center;
        background: linear-gradient(135deg, #f5f3ff 0%, #e9d5ff 100%);
        font-family: Arial, Helvetica, sans-serif;
        color: var(--ink);
      }

      .card {
        width: min(900px, 90vw);
        background: rgba(255, 255, 255, 0.8);
        backdrop-filter: blur(10px);
        border: 1px solid rgba(124, 58, 237, 0.15);
        border-radius: 32px;
        box-shadow: var(--shadow-soft);
        padding: 48px 40px;
      }

      .logo-wrap {
        display: flex;
        align-items: center;
        gap: 32px;
        flex-wrap: wrap;
        justify-content: center;
      }

      .mark {
        position: relative;
        width: 150px;
        height: 150px;
        border-radius: 34px;
        background: linear-gradient(135deg, var(--violet-800), var(--violet-500));
        box-shadow: 0 22px 50px rgba(91, 33, 182, 0.35);
        overflow: hidden;
      }

      .mark::before {
        content: "";
        position: absolute;
        width: 102px;
        height: 102px;
        background: var(--white);
        border-radius: 28px;
        left: 24px;
        top: 24px;
        transform: rotate(45deg);
      }

      .mark::after {
        content: "";
        position: absolute;
        width: 48px;
        height: 48px;
        background: linear-gradient(135deg, var(--violet-600), var(--violet-400));
        border-radius: 18px;
        right: 24px;
        bottom: 24px;
        box-shadow: inset 0 0 0 7px rgba(255,255,255,0.9);
      }

      .brand {
        display: flex;
        flex-direction: column;
        gap: 8px;
      }

      .brand-title {
        font-size: clamp(2.2rem, 5vw, 4rem);
        line-height: 1;
        font-weight: 800;
        letter-spacing: 0.12em;
        color: var(--violet-800);
      }

      .brand-sub {
        font-size: 0.9rem;
        letter-spacing: 0.28em;
        text-transform: uppercase;
        color: var(--violet-500);
        font-weight: 700;
      }

      .tagline {
        margin-top: 18px;
        font-size: 1rem;
        letter-spacing: 0.08em;
        text-transform: uppercase;
        color: var(--ink-soft);
      }

      .swatches {
        margin-top: 30px;
        display: flex;
        gap: 14px;
        justify-content: center;
        flex-wrap: wrap;
      }

      .swatch {
        width: 78px;
        height: 78px;
        border-radius: 20px;
        border: 2px solid rgba(17, 24, 39, 0.05);
        box-shadow: 0 8px 20px rgba(0,0,0,0.04);
      }

      .s1 { background: var(--violet-900); }
      .s2 { background: var(--violet-700); }
      .s3 { background: var(--violet-500); }
      .s4 { background: var(--violet-200); }
      .s5 { background: var(--white); }
    </style>
  </head>
  <body>
    <div class="card">
      <div class="logo-wrap">
        <div class="mark" aria-label="Logo mark"></div>

        <div class="brand">
          <div class="brand-title">VIOLET</div>
          <div class="brand-sub">White Studio</div>
          <div class="tagline">Modern brand identity</div>
        </div>
      </div>

      <div class="swatches" aria-label="Color palette">
        <div class="swatch s1" title="#2e1065"></div>
        <div class="swatch s2" title="#5b21b6"></div>
        <div class="swatch s3" title="#7c3aed"></div>
        <div class="swatch s4" title="#c4b5fd"></div>
        <div class="swatch s5" title="#ffffff"></div>
      </div>
    </div>
  </body>
</html>
