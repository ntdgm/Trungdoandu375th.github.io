<title>375th PARACHUTE REGIMENT</title>

<style>
    @import url('https://fonts.googleapis.com/css2?family=Rajdhani:wght@400;500;600;700&display=swap');

    :root {
        --bg: #020b16;
        --bg-light: #061a2b;
        --blue: #1597e5;
        --blue-light: #43c8ff;
        --text: #e9f7ff;
        --muted: #9bb6c8;
        --border: rgba(43, 181, 255, 0.25);
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
        font-family: "Rajdhani", sans-serif;
        background:
            radial-gradient(
                circle at 50% 0%,
                #063457 0%,
                transparent 35%
            ),
            linear-gradient(
                180deg,
                #020b16 0%,
                #03111e 50%,
                #020810 100%
            );
        color: var(--text);
        line-height: 1.7;
        overflow-x: hidden;
    }

    /* ================= NAVBAR ================= */

    nav {
        position: fixed;
        top: 0;
        left: 0;
        width: 100%;
        z-index: 1000;

        padding: 18px 7%;

        display: flex;
        justify-content: flex-start;
        align-items: center;

        background: rgba(2, 11, 22, 0.75);
        backdrop-filter: blur(14px);

        border-bottom: 1px solid var(--border);
    }

    .logo {
        font-size: 22px;
        font-weight: 700;
        letter-spacing: 3px;
        color: var(--blue-light);
    }

    /* ================= HERO ================= */

    .hero {
        min-height: 100vh;

        display: flex;
        justify-content: center;
        align-items: center;

        text-align: center;

        padding: 120px 20px 80px;

        position: relative;
    }

    .hero::before {
        content: "";

        position: absolute;
        inset: 0;

        background:
            linear-gradient(
                rgba(21,151,229,.04) 1px,
                transparent 1px
            ),
            linear-gradient(
                90deg,
                rgba(21,151,229,.04) 1px,
                transparent 1px
            );

        background-size: 45px 45px;

        mask-image: linear-gradient(
            to bottom,
            black,
            transparent
        );

        -webkit-mask-image: linear-gradient(
            to bottom,
            black,
            transparent
        );
    }

    .hero-content {
        max-width: 1000px;
        position: relative;
        z-index: 1;
    }

    .badge {
        display: inline-block;

        padding: 8px 18px;

        border: 1px solid var(--border);
        border-radius: 30px;

        color: var(--blue-light);

        letter-spacing: 3px;
        font-size: 14px;

        margin-bottom: 25px;

        background: rgba(21,151,229,.05);

        animation: pulse 3s infinite;
    }

    .hero h1 {
        font-size: clamp(42px, 8vw, 95px);
        line-height: 1;

        letter-spacing: 6px;
        font-weight: 700;

        background: linear-gradient(
            90deg,
            #ffffff,
            #46c9ff,
            #ffffff
        );

        -webkit-background-clip: text;
        -webkit-text-fill-color: transparent;

        text-shadow: 0 0 40px rgba(21,151,229,.25);
    }

    .hero h2 {
        margin-top: 20px;

        color: var(--blue-light);

        font-size: clamp(18px, 3vw, 28px);

        letter-spacing: 5px;
    }

    .hero p {
        max-width: 750px;

        margin: 30px auto;

        color: var(--muted);

        font-size: 18px;
    }

    .hero-button {
        display: inline-block;

        margin-top: 15px;

        padding: 14px 30px;

        color: white;

        text-decoration: none;

        font-weight: 700;
        letter-spacing: 2px;

        border: 1px solid var(--blue);

        background: rgba(21,151,229,.1);

        transition: .3s;
    }

    .hero-button:hover {
        background: var(--blue);

        box-shadow:
            0 0 30px rgba(21,151,229,.5);

        transform: translateY(-3px);
    }

    /* ================= SECTION ================= */

    section {
        padding: 100px 7%;

        max-width: 1250px;

        margin: auto;
    }

    .section-title {
        margin-bottom: 50px;
    }

    .section-title span {
        color: var(--blue-light);

        font-size: 14px;

        letter-spacing: 4px;
    }

    .section-title h2 {
        font-size: 42px;

        margin-top: 8px;

        letter-spacing: 2px;
    }

    .section-title .line {
        margin-top: 15px;

        width: 70px;
        height: 3px;

        background: var(--blue);

        box-shadow:
            0 0 15px var(--blue);
    }

    /* ================= INTRO ================= */

    .intro {
        display: grid;

        grid-template-columns: 1fr 1fr;

        gap: 50px;

        align-items: center;
    }

    .intro-text p {
        color: var(--muted);

        font-size: 18px;

        margin-bottom: 20px;
    }

    .quote {
        padding: 35px;

        border-left: 3px solid var(--blue);

        background:
            linear-gradient(
                90deg,
                rgba(21,151,229,.12),
                transparent
            );

        color: #dff5ff;

        font-size: 22px;

        font-weight: 600;
    }

    /* ================= UNITS ================= */

    .units {
        display: grid;

        grid-template-columns: repeat(2, 1fr);

        gap: 25px;
    }

    .unit-card {
        position: relative;

        padding: 35px;

        background:
            linear-gradient(
                145deg,
                rgba(10,47,73,.75),
                rgba(2,15,27,.9)
            );

        border: 1px solid var(--border);

        transition: .35s;

        overflow: hidden;
    }

    .unit-card::before {
        content: "";

        position: absolute;

        top: 0;
        left: 0;

        width: 100%;
        height: 2px;

        background:
            linear-gradient(
                90deg,
                transparent,
                var(--blue),
                transparent
            );
    }

    .unit-card:hover {
        transform: translateY(-8px);

        border-color: var(--blue);

        box-shadow:
            0 15px 40px rgba(0, 132, 255, .15);
    }

    .unit-number {
        color: var(--blue-light);

        font-size: 14px;

        letter-spacing: 4px;
    }

    .unit-card h3 {
        margin: 10px 0 15px;

        font-size: 28px;
    }

    .unit-card p {
        color: var(--muted);

        font-size: 17px;
    }

    /* ================= CHAIN OF COMMAND ================= */

    .command-section {
        position: relative;
    }

    .command-grid {
        display: grid;

        grid-template-columns: repeat(2, 1fr);

        gap: 25px;
    }

    .command-card {
        position: relative;

        padding: 32px;

        background:
            linear-gradient(
                145deg,
                rgba(10,47,73,.78),
                rgba(2,15,27,.94)
            );

        border: 1px solid var(--border);

        overflow: hidden;

        transition: .35s;
    }

    .command-card::before {
        content: "";

        position: absolute;

        top: 0;
        left: 0;

        width: 100%;
        height: 2px;

        background:
            linear-gradient(
                90deg,
                transparent,
                var(--blue),
                transparent
            );
    }

    .command-card::after {
        content: "";

        position: absolute;

        width: 120px;
        height: 120px;

        right: -60px;
        bottom: -60px;

        border-radius: 50%;

        background:
            rgba(21,151,229,.08);
    }

    .command-card:hover {
        transform: translateY(-7px);

        border-color: var(--blue);

        box-shadow:
            0 15px 40px rgba(0, 132, 255, .16);
    }

    .command-card.full-width {
        grid-column: 1 / -1;
    }

    .command-level {
        color: var(--blue-light);

        font-size: 13px;

        font-weight: 700;

        letter-spacing: 3px;

        margin-bottom: 10px;
    }

    .command-card h3 {
        font-size: 25px;

        letter-spacing: 1px;

        margin-bottom: 15px;
    }

    .command-role {
        color: var(--muted);

        font-size: 16px;

        line-height: 1.7;

        margin-bottom: 22px;
    }

    .command-members {
        border-top:
            1px solid rgba(43,181,255,.15);

        padding-top: 18px;
    }

    .command-member {
        display: flex;

        justify-content: space-between;

        align-items: center;

        gap: 20px;

        padding: 10px 0;

        border-bottom:
            1px solid rgba(255,255,255,.05);
    }

    .command-member:last-child {
        border-bottom: none;
    }

    .command-position {
        color: #8db5ca;

        font-size: 14px;

        letter-spacing: 1px;
    }

    .command-name {
        color: #e9f7ff;

        font-weight: 700;

        text-align: right;

        letter-spacing: 1px;
    }

    /* ================= CTA ================= */

    .cta {
        margin: 50px 7% 100px;

        padding: 70px 30px;

        text-align: center;

        border: 1px solid var(--border);

        background:
            radial-gradient(
                circle at center,
                rgba(21,151,229,.2),
                rgba(2,11,22,.8)
            );
    }

    .cta h2 {
        font-size: 40px;

        letter-spacing: 3px;
    }

    .cta p {
        max-width: 650px;

        margin: 15px auto 30px;

        color: var(--muted);

        font-size: 18px;
    }

    /* ================= FOOTER ================= */

    footer {
        padding: 30px;

        text-align: center;

        border-top: 1px solid var(--border);
