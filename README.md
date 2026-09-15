<!DOCTYPE html>
<html lang="vi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

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
                radial-gradient(circle at 50% 0%, #063457 0%, transparent 35%),
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
            justify-content: space-between;
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

        .nav-links {
            display: flex;
            gap: 30px;
            list-style: none;
        }

        .nav-links a {
            color: #d9efff;
            text-decoration: none;
            font-weight: 600;
            letter-spacing: 1px;
            transition: .3s;
        }

        .nav-links a:hover {
            color: var(--blue-light);
            text-shadow: 0 0 12px var(--blue);
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
                    rgba(21,
