<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0">
    <meta name="apple-mobile-web-app-capable" content="yes">
    <meta name="apple-mobile-web-app-status-bar-style" content="black-translucent">
    <meta name="apple-mobile-web-app-capable" content="yes">
    <meta name="theme-color" content="#F4F0E6">
    <title>Kino. Ici, on rencontre vraiment.</title>
    <link href="https://fonts.googleapis.com/css2?family=Syne:wght@400;700;800&family=DM+Mono:wght@400;500&family=Newsreader:ital,wght@0,400;0,500;1,400;1,600&display=swap" rel="stylesheet">
    <script src="https://cdn.jsdelivr.net/npm/@supabase/supabase-js@2"></script>
    <style>
    *, *::before, *::after {
        box-sizing: border-box;
        margin: 0;
        padding: 0;
        -webkit-tap-highlight-color: transparent;
    }

    :root {
        --black: #0A0A0A;
        --white: #F5F3EE;
        --line: #1E1E1E;
        --line2: #2A2A2A;
        --accent: #C8FF00;
        --red: #FF3C3C;
        --blue: #7878FF;
        --ink: #F5F3EE;
        --ink2: #B8B5AF;
        --ink3: #555555;
        --font-serif: 'Newsreader', Georgia, serif;
        --font-sans: 'Syne', sans-serif;
        --font-mono: 'DM Mono', monospace;
        --nav-h: 72px;
    }

    html, body {
        height: 100%;
        height: 100dvh;
        margin: 0;
        padding: 0;
        background: #F4F0E6;
        color: #1A1208;
        font-family: var(--font-serif);
        overflow: hidden;
    }

    #app {
        width: 100%;
        max-width: 430px;
        height: 100dvh;
        margin: 0 auto;
        position: relative;
        overflow: hidden;
        background: #F4F0E6;
    }/* ── SCREENS ── */

    .screen {
        position: absolute;
        inset: 0;
        display: flex;
        flex-direction: column;
        opacity: 0;
        pointer-events: none;
        transform: translateX(28px);
        transition: all .35s cubic-bezier(.4, 0, .2, 1);
        overflow-y: auto;
        -webkit-overflow-scrolling: touch;
        z-index: 10;
    }

    .screen.active {
        opacity: 1;
        pointer-events: all;
        transform: translateX(0);
        z-index: 15;
    }

    .screen.exit {
        opacity: 0;
        transform: translateX(-28px);
    }

    .tab-screen {
        position: absolute;
        inset: 0;
        bottom: calc(var(--nav-h) + env(safe-area-inset-bottom));
        display: flex;
        flex-direction: column;
        opacity: 0;
        pointer-events: none;
        transition: opacity .25s;
        overflow-y: auto;
    }

    .tab-screen.active {
        opacity: 1;
        pointer-events: all;
    }/* ── BOTTOM NAV ── */

    .bottom-nav {
        position: absolute;
        bottom: 0;
        left: 0;
        right: 0;
        height: calc(var(--nav-h) + env(safe-area-inset-bottom));
        background: #F4F0E6;
        border-top: 1px solid #C8BEA8 !important;
        border-top: 1px solid #D8D0BC;
        display: none;
        align-items: center;
        justify-content: space-around;
        padding-bottom: env(safe-area-inset-bottom);
        z-index: 100;
    }

    .bottom-nav.visible {
        display: flex;
    }

    .nav-btn {
        display: flex;
        flex-direction: column;
        align-items: center;
        gap: 4px;
        background: none;
        border: none;
        cursor: pointer;
        padding: 8px 20px;
        flex: 1;
    }

    .nav-icon {
        font-size: 20px;
        line-height: 1;
    }

    .nav-label {
        font-family: var(--font-mono);
        font-size: 9px;
        letter-spacing: .08em;
        text-transform: uppercase;
        color: #9A9080;
        transition: color .2s;
    }

    .nav-btn.active .nav-label {
        color: #1E3A2F;
    }

    .nav-dot {
        width: 4px;
        height: 4px;
        border-radius: 50%;
        background: #1E3A2F;
        margin-top: 2px;
        display: none;
    }

    .nav-btn.active .nav-dot {
        display: block;
    }/* ── BUTTONS ── */

    .btn {
        width: 100%;
        padding: 15px 24px;
        border: none;
        font-family: var(--font-sans);
        font-size: 13px;
        font-weight: 700;
        letter-spacing: .08em;
        text-transform: uppercase;
        cursor: pointer;
        transition: all .2s;
        border-radius: 50px;
    }

    .btn:active {
        transform: scale(.97);
    }

    .btn-primary {
        background: #1E3A2F;
        color: #F4F0E6;
    }

    .btn-primary:hover {
        background: #2D5A42;
    }

    .btn-outline {
        background: transparent;
        color: #5A4E3A;
        border: 1px solid #C8BEA8;
    }

    .btn-outline:hover {
        border-color: #5A4E3A;
        color: #1A1208;
    }

    .btn-ghost {
        width: 100%;
        background: none;
        border: none;
        font-family: var(--font-mono);
        font-size: 11px;
        letter-spacing: .08em;
        text-transform: uppercase;
        color: #9A9080;
        cursor: pointer;
        padding: 12px;
        text-decoration: underline;
        transition: color .2s;
    }

    .btn-ghost:hover {
        color: #1A1208;
    }

    .pref-chip {
        background: transparent;
        border: 1px solid #C8BEA8;
        border-radius: 50px;
        padding: 6px 14px;
        font-family: 'DM Mono', monospace;
        font-size: 10px;
        letter-spacing: .06em;
        text-transform: uppercase;
        color: #5A4E3A;
        cursor: pointer;
        transition: all .2s;
    }

    .pref-chip.active {
        background: #1E3A2F;
        border-color: #1E3A2F;
        color: #FDF8F4;
    }

    .btn-danger {
        background: transparent;
        border: 1px solid #D8D0BC;
        color: #8B2635;
        font-family: var(--font-mono);
        font-size: 11px;
        letter-spacing: .08em;
        text-transform: uppercase;
        padding: 12px;
        border-radius: 2px;
        cursor: pointer;
        width: 100%;
        transition: all .2s;
        margin-top: 8px;
    }

    .btn-danger:hover {
        border-color: var(--red);
    }/* ── INPUTS ── */

    .input {
        width: 100%;
        padding: 14px 0;
        background: transparent;
        border: none;
        border-bottom: 1px solid #C8BEA8;
        color: #1A1208;
        font-family: var(--font-serif);
        font-size: 16px;
        font-style: italic;
        outline: none;
        transition: border-color .2s;
    }

    .input:focus {
        border-color: #1E3A2F;
    }

    .input::placeholder {
        color: #B0A890;
    }/* ── OTP ── */

    .otp-wrap {
        display: flex;
        gap: 6px;
        justify-content: center;
        margin: 28px 0;
    }

    .otp-digit {
        width: 36px;
        height: 52px;
        background: #EAE4D4;
        border: 1px solid #C8BEA8;
        border-radius: 12px;
        color: #1A1208;
        font-family: var(--font-sans);
        font-weight: 800;
        font-size: 1.4rem;
        text-align: center;
        outline: none;
        transition: border-color .2s;
        caret-color: var(--accent);
    }

    .otp-digit:focus {
        border-color: #1E3A2F;
    }/* ── TOAST ── */

    .toast {
        position: fixed;
        bottom: calc(var(--nav-h) + env(safe-area-inset-bottom) + 16px);
        left: 50%;
        transform: translateX(-50%);
        background: #1A1208;
        color: #F4F0E6;
        padding: 10px 20px;
        border-radius: 2px;
        font-family: var(--font-mono);
        font-size: 12px;
        letter-spacing: .04em;
        white-space: nowrap;
        z-index: 300;
        opacity: 0;
        transition: opacity .3s;
        pointer-events: none;
    }

    .toast.show {
        opacity: 1;
    }/* ── SHARED ── */

    .pg-head {
        padding: 52px 28px 24px;
        flex-shrink: 0;
    }

    .pg-eye {
        font-family: var(--font-mono);
        font-size: 11px;
        letter-spacing: .1em;
        text-transform: uppercase;
        color: #9A9080;
        margin-bottom: 12px;
    }

    .pg-title {
        font-family: var(--font-sans);
        font-weight: 800;
        font-size: 2.2rem;
        line-height: .95;
        letter-spacing: -.02em;
        text-transform: uppercase;
        color: #1A1208;
    }

    .pg-title em {
        font-style: italic;
        font-family: var(--font-serif);
        font-weight: 400;
        color: #5A4E3A;
    }

    .pg-sub {
        font-size: 14px;
        color: #5A4E3A;
        font-style: italic;
        margin-top: 8px;
        line-height: 1.6;
    }

    .pg-foot {
        padding: 8px 28px 44px;
        display: flex;
        flex-direction: column;
        gap: 10px;
        flex-shrink: 0;
    }

    .segs {
        display: flex;
        gap: 4px;
        margin-bottom: 20px;
    }

    .seg {
        height: 1px;
        flex: 1;
        background: #C8BEA8;
        transition: background .3s;
    }

    .seg.on {
        background: #1E3A2F;
    }

    .form-body {
        padding: 8px 28px 16px;
        display: flex;
        flex-direction: column;
        gap: 24px;
    }

    .flbl {
        font-family: var(--font-mono);
        font-size: 10px;
        letter-spacing: .1em;
        text-transform: uppercase;
        color: #9A9080;
        margin-bottom: 4px;
    }

    .g-grid {
        display: flex;
        gap: 8px;
    }

    .g-opt {
        flex: 1;
        padding: 12px 6px;
        text-align: center;
        background: transparent;
        border: 1px solid #C8BEA8;
        border-radius: 2px;
        font-family: var(--font-mono);
        font-size: 11px;
        letter-spacing: .06em;
        text-transform: uppercase;
        color: #5A4E3A;
        cursor: pointer;
        transition: all .2s;
    }

    .g-opt.sel {
        border-color: #1E3A2F;
        color: #1E3A2F;
        background: rgba(232, 98, 42, .06);
    }

    .rech-list {
        padding: 8px 28px 16px;
        display: flex;
        flex-direction: column;
        gap: 8px;
    }

    .rech-item {
        display: flex;
        align-items: center;
        gap: 14px;
        padding: 16px 18px;
        background: transparent;
        border: 1px solid #C8BEA8;
        border-radius: 2px;
        cursor: pointer;
        transition: all .2s;
        text-align: left;
    }

    .rech-item:hover, .rech-item.sel {
        border-color: #1E3A2F;
        background: rgba(232, 98, 42, .06);
    }

    .rech-ico {
        width: 40px;
        height: 40px;
        border-radius: 2px;
        background: var(--line);
        display: flex;
        align-items: center;
        justify-content: center;
        font-size: 18px;
        color: #9A9080;
        flex-shrink: 0;
    }

    .rech-lbl {
        font-family: var(--font-sans);
        font-size: 14px;
        font-weight: 700;
        color: #1A1208;
        text-transform: uppercase;
        letter-spacing: .04em;
    }

    .rech-sub {
        font-family: var(--font-serif);
        font-size: 12px;
        font-style: italic;
        color: #9A9080;
        margin-top: 2px;
    }

    .rech-chk {
        margin-left: auto;
        width: 22px;
        height: 22px;
        border: 1px solid #C8BEA8;
        border-radius: 2px;
        flex-shrink: 0;
        display: flex;
        align-items: center;
        justify-content: center;
        font-size: 11px;
        color: transparent;
        transition: all .2s;
        font-family: var(--font-mono);
    }

    .rech-item.sel .rech-chk {
        background: #1E3A2F;
        border-color: #1E3A2F;
        color: #FDF8F4;
    }/* ── HOME ── */

    #s-home {
        background: #F4F0E6;
        overflow: hidden;
        justify-content: space-between;
    }

    .home-top {
        padding: 52px 28px 0;
        flex: 1;
        display: flex;
        flex-direction: column;
        justify-content: center;
    }

    .home-logo {
        font-family: var(--font-sans);
        font-weight: 800;
        font-size: 13px;
        letter-spacing: .1em;
        text-transform: uppercase;
        color: #9A9080;
        margin-bottom: 40px;
    }

    .home-logo span {
        color: #1E3A2F;
    }

    .h-title {
        font-family: var(--font-sans);
        font-weight: 800;
        font-size: clamp(3rem, 15vw, 4.8rem);
        line-height: .92;
        letter-spacing: -.03em;
        text-transform: uppercase;
        color: #1A1208;
        margin-bottom: 20px;
    }

    .h-title em {
        font-style: italic;
        font-family: var(--font-serif);
        font-weight: 400;
        color: #5A4E3A;
    }

    .h-sub {
        font-size: 1rem;
        color: #5A4E3A;
        line-height: 1.65;
        font-style: italic;
        max-width: 300px;
        margin-bottom: 32px;
    }

    .home-pill {
        display: inline-flex;
        align-items: center;
        gap: 8px;
        border: 1px solid #C8BEA8;
        padding: 7px 14px;
        border-radius: 2px;
        margin-bottom: 36px;
    }

    .pulse {
        width: 7px;
        height: 7px;
        border-radius: 50%;
        background: #1E3A2F;
        animation: pulse 2s infinite;
    }

    @keyframes pulse {
        0%, 100% {
            opacity: 1;
            transform:scale(1)
        }

        50% {
            opacity: .4;
            transform: scale(.7)
        }
    }

    .pill-txt {
        font-family: var(--font-mono);
        font-size: 11px;
        letter-spacing: .06em;
        text-transform: uppercase;
        color: #9A9080;
    }

    .home-bot {
        padding: 0 28px 44px;
        display: flex;
        flex-direction: column;
        gap: 10px;
        border-top: 1px solid #C8BEA8;
        padding-top: 20px;
    }/* ── FLASH CARDS ── */

    #s-questions {
        overflow: hidden;
        background: #F4F0E6;
    }

    .q-wrap {
        padding: 20px 20px 16px;
        display: flex;
        flex-direction: column;
        height: 100%;
        min-height: 0;
    }

    .q-header {
        flex-shrink: 0;
        margin-bottom: 16px;
    }

    .qbars {
        display: flex;
        gap: 3px;
        margin-bottom: 10px;
    }

    .qb {
        height: 1px;
        flex: 1;
        background: #C8BEA8;
        transition: background .4s;
    }

    .qb.done {
        background: #1E3A2F;
    }

    .qb.now {
        background: #C8A890;
    }

    .qmeta {
        display: flex;
        justify-content: space-between;
        align-items: center;
    }

    .qmeta-left {
        font-family: var(--font-mono);
        font-size: 10px;
        letter-spacing: .1em;
        text-transform: uppercase;
        color: #9A9080;
    }

    .qmeta-right {
        font-family: var(--font-mono);
        font-size: 11px;
        color: #9A9080;
    }

    .card-stack {
        flex: 1;
        position: relative;
        display: flex;
        align-items: center;
        justify-content: center;
        min-height: 260px;
    }

    .flash-card {
        position: absolute;
        width: 100%;
        max-width: 340px;
        height: 270px;
        background: #EAE4D4;
        border: 1px solid #C8BEA8;
        border-radius: 4px;
        padding: 1.6rem;
        display: flex;
        flex-direction: column;
        justify-content: space-between;
        cursor: grab;
        user-select: none;
        transition: transform .08s ease;
        will-change: transform;
    }

    .flash-card:active {
        cursor: grabbing;
    }

    .flash-card.behind-1 {
        transform: translateY(10px) scale(0.96);
        z-index: 1;
        pointer-events: none;
    }

    .flash-card.behind-2 {
        transform: translateY(20px) scale(0.92);
        z-index: 0;
        pointer-events: none;
    }

    .flash-card.top {
        z-index: 10;
    }

    .vote-overlay {
        position: absolute;
        inset: 0;
        border-radius: 4px;
        opacity: 0;
        pointer-events: none;
        display: flex;
        align-items: center;
        justify-content: center;
        transition: opacity .1s;
    }

    .vote-yes {
        background: rgba(232, 98, 42, .12);
        border: 2px solid var(--accent);
    }

    .vote-no {
        background: rgba(192, 57, 43, .08);
        border: 2px solid var(--red);
    }

    .vote-maybe {
        background: rgba(91, 110, 174, .08);
        border: 2px solid var(--blue);
    }

    .vote-label {
        font-family: var(--font-sans);
        font-weight: 800;
        font-size: 1.5rem;
        letter-spacing: .04em;
        text-transform: uppercase;
    }

    .vote-yes .vote-label {
        color: #1E3A2F;
    }

    .vote-no .vote-label {
        color: var(--red);
    }

    .vote-maybe .vote-label {
        color: var(--blue);
    }

    .card-num {
        font-family: var(--font-mono);
        font-size: 10px;
        letter-spacing: .1em;
        text-transform: uppercase;
        color: #9A9080;
    }

    .card-body {
        flex: 1;
        display: flex;
        align-items: center;
        padding: .6rem 0;
    }

    .card-text {
        font-family: var(--font-serif);
        font-size: 1.2rem;
        font-style: italic;
        line-height: 1.5;
        color: #1A1208;
    }

    .card-theme {
        font-family: var(--font-mono);
        font-size: 10px;
        letter-spacing: .08em;
        text-transform: uppercase;
        color: #B0A890;
    }

    .fly-right {
        animation: flyRight .38s cubic-bezier(.4, 0, .2, 1) forwards;
    }

    .fly-left {
        animation: flyLeft .38s cubic-bezier(.4, 0, .2, 1) forwards;
    }

    .fly-up {
        animation: flyUp .38s cubic-bezier(.4, 0, .2, 1) forwards;
    }

    @keyframes flyRight {
        to {
            transform: translateX(150%) rotate(22deg);
            opacity: 0;
        }
    }

    @keyframes flyLeft {
        to {
            transform: translateX(-150%) rotate(-22deg);
            opacity: 0;
        }
    }

    @keyframes flyUp {
        to {
            transform: translateY(-110%) scale(.85);
            opacity: 0;
        }
    }

    .q-actions {
        flex-shrink: 0;
        display: flex;
        justify-content: center;
        gap: 12px;
        padding: 12px 0 4px;
    }

    .action-btn {
        display: flex;
        flex-direction: column;
        align-items: center;
        gap: 5px;
        background: transparent;
        border: 1px solid #C8BEA8;
        padding: .65rem 1.3rem;
        cursor: pointer;
        transition: all .2s;
        border-radius: 2px;
        min-width: 76px;
    }

    .action-icon {
        font-size: 1rem;
    }

    .action-label {
        font-family: var(--font-mono);
        font-size: 10px;
        letter-spacing: .06em;
        text-transform: uppercase;
        color: #9A9080;
    }

    .btn-no:hover {
        border-color: var(--red);
    }

    .btn-no:hover .action-label {
        color: var(--red);
    }

    .btn-maybe:hover {
        border-color: var(--blue);
    }

    .btn-maybe:hover .action-label {
        color: var(--blue);
    }

    .btn-yes:hover {
        border-color: var(--accent);
    }

    .btn-yes:hover .action-label {
        color: var(--accent);
    }

    .qhint {
        text-align: center;
        font-family: var(--font-mono);
        font-size: 10px;
        letter-spacing: .06em;
        text-transform: uppercase;
        color: #B0A890;
        padding-bottom: 4px;
    }/* ── TABS ── */

    #tab-accueil {
        background: #F4F0E6;
    }

    .accueil-head {
        padding: 52px 24px 16px;
        border-bottom: 1px solid #C8BEA8;
        flex-shrink: 0;
        background: #F4F0E6;
    }

    .accueil-logo {
        font-family: var(--font-sans);
        font-weight: 800;
        font-size: 1rem;
        letter-spacing: .08em;
        text-transform: uppercase;
        color: #1A1208;
    }

    .accueil-logo span {
        color: #1E3A2F;
    }

    .accueil-sub {
        font-family: var(--font-mono);
        font-size: 10px;
        letter-spacing: .08em;
        text-transform: uppercase;
        color: #9A9080;
        margin-top: 4px;
    }

    #tab-matchs {
        background: #F4F0E6;
    }

    .matchs-head {
        padding: 52px 24px 16px;
        border-bottom: 1px solid #C8BEA8;
        flex-shrink: 0;
        background: #F4F0E6;
    }

    .matchs-title {
        font-family: var(--font-sans);
        font-weight: 800;
        font-size: 1.8rem;
        letter-spacing: -.02em;
        text-transform: uppercase;
        color: #1A1208;
    }

    .matchs-list {
        padding: 16px 24px;
        display: flex;
        flex-direction: column;
        gap: 10px;
    }

    .match-card {
        background: #EAE4D4;
        border: 1px solid #C8BEA8;
        border-radius: 2px;
        padding: 18px;
        cursor: pointer;
        transition: border-color .2s;
    }

    .match-card:hover {
        border-color: var(--accent);
    }

    .match-card-top {
        display: flex;
        align-items: center;
        gap: 14px;
        margin-bottom: 12px;
    }

    .match-av {
        width: 44px;
        height: 44px;
        border-radius: 2px;
        background: #1E3A2F;
        display: flex;
        align-items: center;
        justify-content: center;
        font-family: var(--font-sans);
        font-weight: 800;
        font-size: 1.1rem;
        color: var(--black);
        flex-shrink: 0;
    }

    .match-name {
        font-family: var(--font-sans);
        font-weight: 700;
        font-size: 1rem;
        letter-spacing: .02em;
        text-transform: uppercase;
        color: #1A1208;
    }

    .match-score {
        margin-left: auto;
        font-family: var(--font-sans);
        font-weight: 800;
        font-size: 1.3rem;
        color: #1E3A2F;
    }

    .match-score span {
        font-family: var(--font-mono);
        font-size: 10px;
        color: #9A9080;
    }

    .match-bar {
        height: 2px;
        background: #C8BEA8;
        border-radius: 1px;
        overflow: hidden;
        margin-bottom: 10px;
    }

    .match-bar-fill {
        height: 100%;
        background: #1E3A2F;
        border-radius: 1px;
    }

    .match-status {
        font-family: var(--font-mono);
        font-size: 10px;
        letter-spacing: .07em;
        text-transform: uppercase;
        color: #9A9080;
    }

    .match-empty {
        padding: 48px 24px;
        text-align: center;
    }

    .match-empty-title {
        font-family: var(--font-sans);
        font-weight: 800;
        font-size: 1.2rem;
        text-transform: uppercase;
        letter-spacing: -.01em;
        margin-bottom: 8px;
    }

    .match-empty-sub {
        font-size: 14px;
        font-style: italic;
        color: #5A4E3A;
        line-height: 1.6;
    }

    .match-detail {
        position: absolute;
        inset: 0;
        bottom: calc(var(--nav-h) + env(safe-area-inset-bottom));
        background: #F4F0E6;
        z-index: 50;
        display: none;
        flex-direction: column;
        overflow-y: auto;
        transform: translateY(100%);
        transition: transform .35s cubic-bezier(.4, 0, .2, 1);
    }

    .match-detail.open {
        display: flex;
        transform: translateY(0);
    }

    .detail-head {
        padding: 52px 24px 20px;
        background: #EAE4D4;
        border-bottom: 1px solid #D8D0BC;
        flex-shrink: 0;
    }

    .detail-back {
        font-family: var(--font-mono);
        font-size: 10px;
        letter-spacing: .08em;
        text-transform: uppercase;
        color: #9A9080;
        background: none;
        border: none;
        cursor: pointer;
        margin-bottom: 16px;
        display: flex;
        align-items: center;
        gap: 6px;
    }

    .detail-badge {
        display: inline-flex;
        align-items: center;
        gap: 6px;
        padding: 4px 12px;
        border: 1px solid #1E3A2F;
        border-radius: 2px;
        font-family: var(--font-mono);
        font-size: 10px;
        letter-spacing: .08em;
        text-transform: uppercase;
        color: #1E3A2F;
        margin-bottom: 16px;
    }

    .detail-avs {
        display: flex;
        align-items: center;
        margin-bottom: 16px;
    }

    .detail-av {
        width: 56px;
        height: 56px;
        border-radius: 2px;
        display: flex;
        align-items: center;
        justify-content: center;
        font-family: var(--font-sans);
        font-weight: 800;
        font-size: 1.2rem;
    }

    .detail-av-a {
        background: #1E3A2F;
        color: #FDF8F4;
    }

    .detail-av-b {
        background: #C8BEA8;
        color: #9A9080;
        margin-left: -6px;
    }

    .detail-score {
        font-family: var(--font-sans);
        font-weight: 800;
        font-size: 3rem;
        letter-spacing: -.03em;
        color: #1E3A2F;
        line-height: 1;
    }

    .detail-score sup {
        font-size: 1rem;
        color: #9A9080;
        font-weight: 400;
    }

    .detail-score-lbl {
        font-family: var(--font-mono);
        font-size: 10px;
        color: #9A9080;
        letter-spacing: .08em;
        text-transform: uppercase;
        margin-top: 2px;
    }

    .detail-body {
        padding: 16px 24px;
        display: flex;
        flex-direction: column;
        gap: 10px;
        flex: 1;
    }

    .detail-block {
        background: #EAE4D4;
        border: 1px solid #C8BEA8;
        border-radius: 2px;
        padding: 16px;
    }

    .detail-block-lbl {
        font-family: var(--font-mono);
        font-size: 10px;
        letter-spacing: .1em;
        text-transform: uppercase;
        color: #9A9080;
        margin-bottom: 10px;
    }

    .detail-name {
        font-family: var(--font-sans);
        font-weight: 800;
        font-size: 1.6rem;
        letter-spacing: -.02em;
        text-transform: uppercase;
        color: #1A1208;
    }

    .detail-mystery {
        display: inline-flex;
        align-items: center;
        gap: 6px;
        padding: 4px 10px;
        border: 1px solid #C8BEA8;
        border-radius: 2px;
        font-family: var(--font-mono);
        font-size: 10px;
        letter-spacing: .06em;
        color: #9A9080;
        margin-top: 8px;
    }

    .detail-desc {
        font-size: 13px;
        font-style: italic;
        color: #5A4E3A;
        line-height: 1.6;
        margin-top: 10px;
    }

    .drow {
        display: flex;
        align-items: center;
        gap: 12px;
        padding: 10px 0;
        border-bottom: 1px solid #D8D0BC;
    }

    .drow:last-child {
        border-bottom: none;
        padding-bottom: 0;
    }

    .dico {
        width: 32px;
        height: 32px;
        border-radius: 2px;
        background: #D8D0BC;
        display: flex;
        align-items: center;
        justify-content: center;
        font-size: 13px;
        flex-shrink: 0;
    }

    .dlbl {
        font-family: var(--font-sans);
        font-size: 13px;
        font-weight: 700;
        letter-spacing: .02em;
        color: #1A1208;
    }

    .dsub {
        font-size: 12px;
        font-style: italic;
        color: #9A9080;
        margin-top: 2px;
    }

    .slots {
        display: flex;
        flex-direction: column;
        gap: 8px;
    }

    .slot {
        display: flex;
        align-items: center;
        justify-content: space-between;
        padding: 12px 14px;
        border: 1px solid #C8BEA8;
        border-radius: 2px;
        cursor: pointer;
        transition: all .2s;
    }

    .chat-bubble {
        padding: 12px 16px;
        border-radius: 12px;
        max-width: 85%;
        margin-bottom: 10px;
        font-family: 'Newsreader', serif;
        font-size: 14px;
        font-style: italic;
        line-height: 1.5;
    }

    .chat-bot {
        background: #EAE4D4;
        color: #1A1208;
        border-bottom-left-radius: 2px;
        align-self: flex-start;
    }

    .chat-system {
        background: #1E3A2F;
        color: #FDF8F4;
        font-style: normal;
        font-family: 'DM Mono', monospace;
        font-size: 11px;
        letter-spacing: .04em;
        text-align: center;
        border-radius: 8px;
        width: 100%;
        max-width: 100%;
        margin: 8px 0;
    }

    .chat-slot {
        display: flex;
        align-items: center;
        justify-content: space-between;
        padding: 10px 14px;
        border: 1px solid #C8BEA8;
        border-radius: 50px;
        cursor: pointer;
        transition: all .2s;
        margin-bottom: 6px;
        background: #F4F0E6;
    }

    .chat-slot:hover, .chat-slot.selected {
        border-color: #1E3A2F;
        background: rgba(232, 98, 42, .06);
    }

    .chat-slot.matched {
        background: #1E3A2F;
        border-color: #1E3A2F;
    }

    .chat-slot.matched .slot-label {
        color: #FDF8F4;
    }

    .slot-label {
        font-family: 'Newsreader', serif;
        font-size: 13px;
        font-style: italic;
        color: #1A1208;
    }

    .slot-check {
        width: 18px;
        height: 18px;
        border: 1px solid #C8BEA8;
        border-radius: 2px;
        display: flex;
        align-items: center;
        justify-content: center;
        font-size: 10px;
        color: transparent;
        transition: all .2s;
        flex-shrink: 0;
    }

    .chat-slot.selected .slot-check {
        background: #1E3A2F;
        border-color: #1E3A2F;
        color: #FDF8F4;
    }

    .chat-slot.matched .slot-check {
        background: #F4F0E6;
        border-color: #FDF8F4;
        color: #1E3A2F;
    }

    .slot:hover, .slot.sel {
        border-color: #1E3A2F;
        background: rgba(232, 98, 42, .06);
    }

    .slot-info {
        font-family: var(--font-sans);
        font-weight: 700;
        font-size: 13px;
        letter-spacing: .02em;
    }

    .slot-sub {
        font-family: var(--font-serif);
        font-size: 12px;
        font-style: italic;
        color: #9A9080;
        margin-top: 2px;
    }

    .slot-chk {
        width: 20px;
        height: 20px;
        border: 1px solid #C8BEA8;
        border-radius: 2px;
        display: flex;
        align-items: center;
        justify-content: center;
        font-family: var(--font-mono);
        font-size: 10px;
        color: transparent;
        transition: all .2s;
        flex-shrink: 0;
    }

    .slot.sel .slot-chk {
        background: #1E3A2F;
        border-color: #1E3A2F;
        color: #FDF8F4;
    }

    .detail-foot {
        padding: 8px 24px 24px;
        display: flex;
        flex-direction: column;
        gap: 10px;
        flex-shrink: 0;
    }/* ── PROFIL ── */

    #tab-profil {
        background: #F4F0E6;
    }

    .profil-head {
        padding: 52px 24px 20px;
        border-bottom: 1px solid #C8BEA8;
        flex-shrink: 0;
        background: #F4F0E6;
    }

    .profil-av-wrap {
        display: flex;
        align-items: center;
        gap: 16px;
        margin-bottom: 4px;
    }

    .profil-av {
        width: 56px;
        height: 56px;
        border-radius: 2px;
        background: #1E3A2F;
        display: flex;
        align-items: center;
        justify-content: center;
        font-family: var(--font-sans);
        font-weight: 800;
        font-size: 1.4rem;
        color: #FDF8F4;
    }

    .profil-name {
        font-family: var(--font-sans);
        font-weight: 800;
        font-size: 1.6rem;
        letter-spacing: -.02em;
        text-transform: uppercase;
        color: #1A1208;
    }

    .profil-email {
        font-family: var(--font-mono);
        font-size: 11px;
        color: #9A9080;
        letter-spacing: .04em;
        margin-top: 2px;
    }

    .profil-body {
        padding: 16px 24px;
        display: flex;
        flex-direction: column;
        gap: 6px;
    }

    .profil-section-lbl {
        font-family: var(--font-mono);
        font-size: 10px;
        letter-spacing: .1em;
        text-transform: uppercase;
        color: #9A9080;
        margin: 8px 0 4px;
    }

    .profil-row {
        display: flex;
        align-items: center;
        justify-content: space-between;
        padding: 14px 16px;
        background: #EAE4D4;
        border: 1px solid #C8BEA8;
        border-radius: 2px;
        cursor: pointer;
        transition: border-color .2s;
    }

    .profil-row:hover {
        border-color: #9A9080;
    }

    .profil-row-left {
        font-family: var(--font-sans);
        font-weight: 700;
        font-size: 13px;
        letter-spacing: .02em;
        color: #1A1208;
    }

    .profil-row-right {
        font-family: var(--font-serif);
        font-size: 12px;
        font-style: italic;
        color: #9A9080;
    }

    .profil-stats {
        display: grid;
        grid-template-columns: 1fr 1fr;
        gap: 8px;
        margin-bottom: 4px;
    }

    .profil-stat {
        background: #EAE4D4;
        border: 1px solid #C8BEA8;
        border-radius: 2px;
        padding: 14px;
    }

    .profil-stat-num {
        font-family: var(--font-sans);
        font-weight: 800;
        font-size: 1.6rem;
        letter-spacing: -.02em;
        color: #1E3A2F;
    }

    .profil-stat-lbl {
        font-family: var(--font-mono);
        font-size: 10px;
        letter-spacing: .07em;
        text-transform: uppercase;
        color: #9A9080;
        margin-top: 2px;
    }/* ── ADMIN ── */

    #s-admin {
        background: #F4F0E6;
    }

    .admin-head {
        padding: 52px 24px 20px;
        border-bottom: 1px solid #C8BEA8;
        flex-shrink: 0;
        background: #F4F0E6;
    }

    .admin-body {
        padding: 16px 24px;
        flex: 1;
        overflow-y: auto;
        background: #F4F0E6;
    }

    .admin-stat-grid {
        display: grid;
        grid-template-columns: 1fr 1fr;
        gap: 8px;
        margin-bottom: 20px;
    }

    .astat {
        background: #EAE4D4;
        border: 1px solid #C8BEA8;
        border-radius: 2px;
        padding: 14px;
    }

    .astat-num {
        font-family: var(--font-sans);
        font-weight: 800;
        font-size: 1.8rem;
        letter-spacing: -.02em;
        color: #1E3A2F;
    }

    .astat-lbl {
        font-family: var(--font-mono);
        font-size: 10px;
        color: #9A9080;
        text-transform: uppercase;
        letter-spacing: .07em;
        margin-top: 2px;
    }

    .section-lbl {
        font-family: var(--font-mono);
        font-size: 10px;
        font-weight: 500;
        letter-spacing: .1em;
        text-transform: uppercase;
        color: #9A9080;
        margin-bottom: 10px;
    }

    .user-row {
        display: flex;
        align-items: center;
        gap: 12px;
        padding: 12px 0;
        border-bottom: 1px solid #D8D0BC;
    }

    .user-row:last-child {
        border-bottom: none;
    }

    .user-av {
        width: 36px;
        height: 36px;
        border-radius: 2px;
        background: #EAE4D4;
        display: flex;
        align-items: center;
        justify-content: center;
        font-family: var(--font-sans);
        font-weight: 800;
        font-size: 14px;
        color: #1E3A2F;
        flex-shrink: 0;
    }

    .user-name {
        font-family: var(--font-sans);
        font-size: 13px;
        font-weight: 700;
        color: #1A1208;
        letter-spacing: .02em;
    }

    .user-info {
        font-family: var(--font-serif);
        font-size: 12px;
        font-style: italic;
        color: #9A9080;
        margin-top: 1px;
    }

    .user-badge {
        margin-left: auto;
        font-family: var(--font-mono);
        font-size: 10px;
        padding: 3px 8px;
        border-radius: 2px;
        flex-shrink: 0;
        letter-spacing: .05em;
        text-transform: uppercase;
    }

    .badge-wait {
        background: #EAE4D4;
        color: #9A9080;
    }

    .badge-match {
        border: 1px solid #1E3A2F;
        color: #1E3A2F;
    }

    .spinner {
        width: 18px;
        height: 18px;
        border: 1.5px solid #C8BEA8;
        border-top-color: #1E3A2F;
        border-radius: 50%;
        animation: spin .8s linear infinite;
        margin: 12px auto;
    }

    @keyframes spin {
        to {
            transform: rotate(360deg)
        }
    }

    @keyframes spinO {
        from {
            transform:rotate(0deg)
        }

        to {
            transform: rotate(360deg)
        }
    }

    #ptr-o.spinning {
        animation: spinO .6s linear infinite;
        display: inline-block;
    }
    </style>
</head>
<body>
    <div id="app">
        <div class="toast" id="toast"></div>

        <!-- ══ HOME ══ -->
        <div class="screen active" id="s-home" style="background:#1C1410;overflow:hidden;justify-content:flex-end;">

            <!-- IMAGE FOND PLEIN ÉCRAN -->
            <div style="position:absolute;inset:0;z-index:0;">
                <img src="data:image/png;base64,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" style="width:100%;height:100%;object-fit:cover;object-position:center top;" alt="">
                <!-- Dégradé bas pour lisibilité texte -->
                <div style="position:absolute;inset:0;background:linear-gradient(to bottom, rgba(28,20,16,0.2) 0%, rgba(28,20,16,0) 25%, rgba(28,20,16,0.55) 60%, rgba(28,20,16,0.92) 80%, rgba(28,20,16,1) 100%);"></div>
            </div>

            <!-- LOGO EN HAUT -->
            <div style="position:absolute;top:calc(52px + env(safe-area-inset-top));left:28px;z-index:2;">
                <div style="font-family:'Syne',sans-serif;font-weight:800;font-size:1.1rem;letter-spacing:.08em;text-transform:uppercase;color:#FDF8F4;">
                    Kino
                    <span style="color:#1E3A2F;">.</span>
                </div>
            </div>

            <!-- CONTENU BAS -->
            <div style="position:relative;z-index:2;padding:0 28px 52px;">

                <!-- Pill compteur -->
                <div style="display:inline-flex;align-items:center;gap:8px;border:1px solid rgba(245,243,238,0.3);padding:6px 14px;border-radius:2px;margin-bottom:20px;backdrop-filter:blur(4px);">
                    <div class="pulse"></div>
                    <span style="font-family:'DM Mono',monospace;font-size:11px;letter-spacing:.06em;text-transform:uppercase;color:rgba(245,243,238,0.8);" id="user-count">Paris · Bêta ouvert</span>
                </div>

                <!-- Titre -->
                <div style="font-family:'Syne',sans-serif;font-weight:800;font-size:clamp(2rem,9vw,3.2rem);line-height:.95;letter-spacing:-.03em;text-transform:uppercase;color:#FDF8F4;margin-bottom:10px;">
                    Le dating,
                    <br>
                    <span style="font-style:italic;font-family:'Newsreader',serif;font-weight:400;color:#F4F0E6;">pour de vrai.</span>
                </div>

                <!-- Sous-titre -->
                <p style="font-family:'Newsreader',serif;font-size:1rem;font-style:italic;color:rgba(245,243,238,0.75);line-height:1.55;margin-bottom:32px;">Des rencontres mystère entre hommes basées sur la personnalité et les intérêts communs.</p>

                <!-- CTAs -->
                <div style="display:flex;flex-direction:column;gap:10px;">
                    <button class="btn btn-primary" onclick="goTo('s-signup')" style="font-size:14px;letter-spacing:.06em;">Commencer</button>
                    <button onclick="goTo('s-login')" style="width:100%;padding:15px 24px;background:rgba(245,243,238,0.12);border:1px solid rgba(245,243,238,0.3);border-radius:50px;font-family:'Syne',sans-serif;font-size:13px;font-weight:700;letter-spacing:.08em;text-transform:uppercase;color:#FDF8F4;cursor:pointer;backdrop-filter:blur(4px);transition:all .2s;">J'ai déjà un compte</button>
                    <button class="btn-ghost" onclick="goTo('s-admin-login')" style="color:rgba(245,243,238,0.4);">Accès admin</button>
                </div>

            </div>
        </div>

        <!-- ══ LOGIN ══ -->
        <div class="screen" id="s-login">
            <div class="pg-head" style="flex:1;display:flex;flex-direction:column;justify-content:center">
                <div class="pg-eye">Connexion</div>
                <div class="pg-title">
                    Bon
                    <br>
                    <em>retour.</em>
                </div>
                <p class="pg-sub" style="margin-bottom:32px">Ici, on rencontre vraiment. Content de te revoir.</p>
                <div>
                    <div class="flbl">Email</div>
                    <input class="input" id="login-email" type="email" placeholder="ton@email.com"/>
                </div>
            </div>
            <div class="pg-foot">
                <button class="btn btn-primary" onclick="sendOTP('login')">Recevoir mon code</button>
                <button class="btn btn-outline" onclick="goTo('s-home')">Retour</button>
            </div>
        </div>

        <!-- ══ OTP ══ -->
        <div class="screen" id="s-otp">
            <div class="pg-head" style="flex:1;display:flex;flex-direction:column;justify-content:center">
                <div class="pg-eye">Vérification</div>
                <div class="pg-title">
                    Code
                    <br>
                    <em>reçu ?</em>
                </div>
                <p class="pg-sub" style="margin-bottom:4px">Code envoyé à</p>
                <p style="font-family:var(--font-mono);font-size:12px;color:var(--accent);letter-spacing:.04em;margin-bottom:4px" id="otp-email-display">—</p>
                <p class="pg-sub" style="margin-bottom:0;font-size:12px">Vérifie tes spams si besoin.</p>
                <div class="otp-wrap">
                    <input class="otp-digit" maxlength="1" type="tel" inputmode="numeric"/>
                    <input class="otp-digit" maxlength="1" type="tel" inputmode="numeric"/>
                    <input class="otp-digit" maxlength="1" type="tel" inputmode="numeric"/>
                    <input class="otp-digit" maxlength="1" type="tel" inputmode="numeric"/>
                    <input class="otp-digit" maxlength="1" type="tel" inputmode="numeric"/>
                    <input class="otp-digit" maxlength="1" type="tel" inputmode="numeric"/>
                    <input class="otp-digit" maxlength="1" type="tel" inputmode="numeric"/>
                    <input class="otp-digit" maxlength="1" type="tel" inputmode="numeric"/>
                </div>
            </div>
            <div class="pg-foot">
                <button class="btn btn-primary" onclick="verifyOTP()">Confirmer</button>
                <button class="btn btn-outline" onclick="goTo('s-home')">Annuler</button>
            </div>
        </div>

        <!-- ══ SIGNUP ══ -->
        <div class="screen" id="s-signup">
            <div class="pg-head">
                <div class="segs">
                    <div class="seg on"></div>
                    <div class="seg"></div>
                    <div class="seg"></div>
                </div>
                <div class="pg-eye">Étape 1 · Profil</div>
                <div class="pg-title">
                    On fait
                    <br>
                    <em>connaissance</em>
                </div>
                <p class="pg-sub">Ici, on rencontre vraiment. Commence par toi.</p>
            </div>
            <div class="form-body">
                <div>
                    <div class="flbl">Prénom</div>
                    <input class="input" id="ip" type="text" placeholder="Ton prénom…"/>
                </div>
                <div>
                    <div class="flbl">Âge</div>
                    <input class="input" id="ia" type="number" placeholder="Ton âge" min="18" max="99"/>
                </div>
                <div>
                    <div class="flbl">Email</div>
                    <input class="input" id="ie" type="email" placeholder="ton@email.com"/>
                </div>
                <div>
                    <div class="flbl">Tu es</div>
                    <div class="g-grid">
                        <button class="g-opt" onclick="sg(this,'homme')">Homme</button>
                        <button class="g-opt" onclick="sg(this,'non-binaire')">Non-binaire</button>
                        <button class="g-opt" onclick="sg(this,'autre')">Autre</button>
                    </div>
                </div>
            </div>
            <div class="pg-foot">
                <button class="btn btn-primary" onclick="vsignup()">Continuer</button>
                <button class="btn btn-outline" onclick="goTo('s-home')">Retour</button>
            </div>
        </div>

        <!-- ══ RECHERCHE ══ -->
        <div class="screen" id="s-recherche">
            <div class="pg-head">
                <div class="segs">
                    <div class="seg on"></div>
                    <div class="seg on" style="opacity:.5"></div>
                    <div class="seg"></div>
                </div>
                <div class="pg-eye">Étape 2 · Préférence</div>
                <div class="pg-title">
                    Qui
                    <br>
                    <em>recherches-tu ?</em>
                </div>
                <p class="pg-sub">Filtre absolu — jamais de profil incompatible.</p>
            </div>
            <div class="rech-list">
                <button class="rech-item" onclick="sr(this,'homme')">
                    <div class="rech-ico">♂</div>
                    <div>
                        <div class="rech-lbl">Un homme</div>
                        <div class="rech-sub">Gay, bi, queer</div>
                    </div>
                    <div class="rech-chk">✓</div>
                </button>
                <button class="rech-item" onclick="sr(this,'non-binaire')">
                    <div class="rech-ico" style="font-size:14px">⊕</div>
                    <div>
                        <div class="rech-lbl">Non-binaire</div>
                        <div class="rech-sub">En dehors des cases</div>
                    </div>
                    <div class="rech-chk">✓</div>
                </button>
                <button class="rech-item" onclick="sr(this,'les deux')">
                    <div class="rech-ico" style="font-size:13px">∞</div>
                    <div>
                        <div class="rech-lbl">Peu importe</div>
                        <div class="rech-sub">Ouvert à tout</div>
                    </div>
                    <div class="rech-chk">✓</div>
                </button>
            </div>
            <div class="pg-foot">
                <button class="btn btn-primary" onclick="goTo('s-preferences')">Continuer</button>
                <button class="btn btn-outline" onclick="goTo('s-signup')">Retour</button>
            </div>
        </div>

        <!-- ══ PRÉFÉRENCES (onboarding) ══ -->
        <div class="screen" id="s-preferences">
            <div class="pg-head">
                <div class="segs">
                    <div class="seg on"></div>
                    <div class="seg on"></div>
                    <div class="seg on" style="opacity:.5"></div>
                </div>
                <div class="pg-eye">Étape 3 · Préférences</div>
                <div class="pg-title">
                    Ce que
                    <br>
                    <em>tu cherches</em>
                </div>
                <p class="pg-sub">On affine ta recherche dès le départ.</p>
            </div>
            <div class="form-body" style="gap:20px;">
                <div>
                    <div class="flbl">Genre recherché</div>
                    <div style="display:flex;flex-wrap:wrap;gap:6px;margin-top:8px;" id="onb-genre-chips">
                        <button onclick="toggleOnbGenre(this,'homme')" class="pref-chip">Homme</button>
                        <button onclick="toggleOnbGenre(this,'non-binaire')" class="pref-chip">Non-binaire</button>
                        <button onclick="toggleOnbGenre(this,'trans')" class="pref-chip">Trans</button>
                        <button onclick="toggleOnbGenre(this,'tous')" class="pref-chip active">Tous</button>
                    </div>
                </div>
                <div>
                    <div style="display:flex;justify-content:space-between;align-items:center;margin-bottom:8px;">
                        <div class="flbl" style="margin-bottom:0;">Tranche d&#39;âge</div>
                        <div style="font-family:var(--font-sans);font-weight:700;font-size:13px;color:#1E3A2F;" id="onb-age-label">18 – 45 ans</div>
                    </div>
                    <input type="range" id="onb-age-min" min="18" max="99" value="18" step="1" oninput="updateOnbAge()" style="width:100%;accent-color:#1E3A2F;margin-bottom:8px;">
                    <input type="range" id="onb-age-max" min="18" max="99" value="45" step="1" oninput="updateOnbAge()" style="width:100%;accent-color:#1E3A2F;">
                    <div style="display:flex;justify-content:space-between;margin-top:4px;">
                        <span style="font-family:var(--font-mono);font-size:9px;color:#B0A890;">18 ans</span>
                        <span style="font-family:var(--font-mono);font-size:9px;color:#B0A890;">99 ans</span>
                    </div>
                </div>
                <div>
                    <div class="flbl">Je cherche quelqu&#39;un de</div>
                    <div style="display:flex;flex-wrap:wrap;gap:6px;margin-top:8px;" id="onb-role-chips">
                        <button onclick="toggleOnbRole(this,'actif')" class="pref-chip">Actif</button>
                        <button onclick="toggleOnbRole(this,'passif')" class="pref-chip">Passif</button>
                        <button onclick="toggleOnbRole(this,'versatile')" class="pref-chip">Versatile</button>
                        <button onclick="toggleOnbRole(this,'peu importe')" class="pref-chip active">Peu importe</button>
                    </div>
                </div>
            </div>
            <div class="pg-foot">
                <button class="btn btn-primary" onclick="startQFromPrefs()">Continuer</button>
                <button class="btn btn-outline" onclick="goTo('s-recherche')">Retour</button>
            </div>
        </div>

        <!-- ══ FLASH CARDS (onboarding) ══ -->
        <div class="screen" id="s-questions">
            <div class="q-wrap">
                <div class="q-header">
                    <div class="qbars" id="qbars"></div>
                    <div class="qmeta">
                        <span class="qmeta-left">Flash cards de personnalité</span>
                        <span class="qmeta-right" id="qcount">1 / 15</span>
                    </div>
                </div>
                <div class="card-stack" id="card-stack"></div>
                <div class="q-actions">
                    <button class="action-btn btn-no" onclick="vote('no')">
                        <span class="action-icon">✕</span>
                        <span class="action-label">Non</span>
                    </button>
                    <button class="action-btn btn-maybe" onclick="vote('maybe')">
                        <span class="action-icon">〜</span>
                        <span class="action-label">Peut-être</span>
                    </button>
                    <button class="action-btn btn-yes" onclick="vote('yes')">
                        <span class="action-icon">✓</span>
                        <span class="action-label">Oui</span>
                    </button>
                </div>
                <div class="qhint">← glisse ou utilise les boutons →</div>
            </div>
        </div>

        <!-- ══════════ APP (bottom nav) ══════════ -->

        <!-- TAB ACCUEIL -->
        <div class="tab-screen" id="tab-accueil" style="display:flex;flex-direction:column;">

            <div id="tab-card-area" style="flex:1;display:flex;flex-direction:column;overflow:hidden;">
                <div class="q-wrap" style="padding-top:52px;flex:1;">
                    <div class="q-header">
                        <div class="qbars" id="tab-qbars"></div>
                        <div class="qmeta">
                            <span class="qmeta-left">Flash cards de personnalité</span>
                            <span class="qmeta-right" id="tab-qcount">1 / 15</span>
                        </div>
                    </div>
                    <div class="card-stack" id="tab-card-stack"></div>
                    <div class="q-actions">
                        <button class="action-btn btn-no" onclick="tabVote('no')">
                            <span class="action-icon">✕</span>
                            <span class="action-label">Non</span>
                        </button>
                        <button class="action-btn btn-maybe" onclick="tabVote('maybe')">
                            <span class="action-icon">〜</span>
                            <span class="action-label">Peut-être</span>
                        </button>
                        <button class="action-btn btn-yes" onclick="tabVote('yes')">
                            <span class="action-icon">✓</span>
                            <span class="action-label">Oui</span>
                        </button>
                    </div>
                    <div class="qhint">← glisse ou utilise les boutons →</div>
                </div>
            </div>
            <div id="tab-done" style="display:none;padding:48px 24px;text-align:center">
                <div style="font-size:2.5rem;margin-bottom:20px">✓</div>
                <div style="font-family:var(--font-sans);font-weight:800;font-size:1.3rem;text-transform:uppercase;letter-spacing:-.01em;margin-bottom:8px">Cartes complétées</div>
                <p style="font-size:14px;font-style:italic;color:#5A4E3A;line-height:1.6">Ici, on rencontre vraiment. Consulte l'onglet Matchs — on cherche quelqu'un pour toi.</p>
            </div>
        </div>

        <!-- TAB MATCHS -->
        <div class="tab-screen" id="tab-matchs" style="display:flex;flex-direction:column;">
            <div class="matchs-head">
                <div class="matchs-title">Matchs</div>
            </div>
            <div id="matchs-content" class="matchs-list" style="flex:1;overflow-y:auto;"></div>

            <!-- CHAT INTERFACE -->
            <div id="chat-screen" style="display:none;position:absolute;inset:0;bottom:var(--nav-h);background:#F4F0E6;flex-direction:column;">
                <!-- Chat header -->
                <div style="padding:52px 20px 14px;border-bottom:1px solid #D8D0BC;background:#F4F0E6;flex-shrink:0;">
                    <button onclick="closeChat()" style="font-family:'DM Mono',monospace;font-size:10px;letter-spacing:.08em;text-transform:uppercase;color:#9A9080;background:none;border:none;cursor:pointer;margin-bottom:10px;display:flex;align-items:center;gap:6px;">← Retour</button>
                    <div style="display:flex;align-items:center;gap:12px;">
                        <div style="width:40px;height:40px;border-radius:2px;background:#1E3A2F;display:flex;align-items:center;justify-content:center;font-family:'Syne',sans-serif;font-weight:800;font-size:1rem;color:#FDF8F4;" id="chat-av">?</div>
                        <div>
                            <div style="font-family:'Syne',sans-serif;font-weight:700;font-size:14px;letter-spacing:.02em;color:#1A1208;" id="chat-title">Assistant de —</div>
                            <div style="font-family:'DM Mono',monospace;font-size:10px;letter-spacing:.06em;text-transform:uppercase;color:#9A9080;">Organisation du rendez-vous</div>
                        </div>
                    </div>
                </div>
                <!-- Chat messages -->
                <div id="chat-messages" style="flex:1;overflow-y:auto;padding:16px 20px;display:flex;flex-direction:column;gap:4px;"></div>
                <!-- Confirm button -->
                <div id="chat-foot" style="padding:12px 20px 24px;border-top:1px solid #D8D0BC;display:none;flex-shrink:0;">
                    <button onclick="confirmSlots()" style="width:100%;padding:14px;background:#1E3A2F;border:none;border-radius:50px;font-family:'Syne',sans-serif;font-weight:700;font-size:12px;letter-spacing:.06em;text-transform:uppercase;color:#FDF8F4;cursor:pointer;">Confirmer mes disponibilités</button>
                </div>
            </div>
        </div>

        <!-- TAB PROFIL -->
        <div class="tab-screen" id="tab-profil">
            <div class="profil-head">
                <div class="profil-av-wrap">
                    <div class="profil-av" id="profil-av">?</div>
                    <div>
                        <div class="profil-name" id="profil-name">—</div>
                        <div class="profil-email" id="profil-email">—</div>
                    </div>
                </div>
            </div>
            <div class="profil-body">
                <div class="profil-stats">
                    <div class="profil-stat">
                        <div class="profil-stat-num" id="profil-stat-cards">—</div>
                        <div class="profil-stat-lbl">Cartes répondues</div>
                    </div>
                    <div class="profil-stat">
                        <div class="profil-stat-num" id="profil-stat-matchs">—</div>
                        <div class="profil-stat-lbl">Matchs reçus</div>
                    </div>
                </div>
                <div class="profil-section-lbl">Mon profil</div>
                <div class="profil-row">
                    <span class="profil-row-left">Prénom</span>
                    <span class="profil-row-right" id="profil-row-prenom">—</span>
                </div>
                <div class="profil-row">
                    <span class="profil-row-left">Âge</span>
                    <span class="profil-row-right" id="profil-row-age">—</span>
                </div>
                <div class="profil-row">
                    <span class="profil-row-left">Je suis</span>
                    <span class="profil-row-right" id="profil-row-genre">—</span>
                </div>

                <div class="profil-section-lbl" style="margin-top:16px;">Je cherche</div>

                <!-- Genre recherché -->
                <div style="background:#EAE4D4;border:1px solid #C8BEA8;border-radius:2px;padding:14px 16px;">
                    <div style="font-family:'DM Mono',monospace;font-size:10px;letter-spacing:.1em;text-transform:uppercase;color:#9A9080;margin-bottom:10px;">Genre</div>
                    <div style="display:flex;flex-wrap:wrap;gap:6px;" id="genre-chips">
                        <button onclick="toggleGenreChip(this,'homme')" class="pref-chip">Homme</button>
                        <button onclick="toggleGenreChip(this,'non-binaire')" class="pref-chip">Non-binaire</button>
                        <button onclick="toggleGenreChip(this,'trans')" class="pref-chip">Trans</button>
                        <button onclick="toggleGenreChip(this,'tous')" class="pref-chip">Tous</button>
                    </div>
                </div>

                <!-- Tranche d'âge -->
                <div style="background:#EAE4D4;border:1px solid #C8BEA8;border-radius:2px;padding:14px 16px;">
                    <div style="display:flex;justify-content:space-between;align-items:center;margin-bottom:12px;">
                        <div style="font-family:'DM Mono',monospace;font-size:10px;letter-spacing:.1em;text-transform:uppercase;color:#9A9080;">Tranche d'âge</div>
                        <div style="font-family:'Syne',sans-serif;font-weight:700;font-size:13px;color:#1E3A2F;" id="age-range-label">18 – 45 ans</div>
                    </div>
                    <div style="margin-bottom:8px;">
                        <input type="range" id="age-min" min="18" max="99" value="18" step="1" oninput="updateAgeRange()" style="width:100%;accent-color:#1E3A2F;margin-bottom:6px;">
                        <input type="range" id="age-max" min="18" max="99" value="45" step="1" oninput="updateAgeRange()" style="width:100%;accent-color:#1E3A2F;">
                    </div>
                    <div style="display:flex;justify-content:space-between;">
                        <span style="font-family:'DM Mono',monospace;font-size:9px;color:#B0A890;letter-spacing:.06em;">18 ans</span>
                        <span style="font-family:'DM Mono',monospace;font-size:9px;color:#B0A890;letter-spacing:.06em;">99 ans</span>
                    </div>
                </div>

                <!-- Rôle -->
                <div style="background:#EAE4D4;border:1px solid #C8BEA8;border-radius:2px;padding:14px 16px;">
                    <div style="font-family:'DM Mono',monospace;font-size:10px;letter-spacing:.1em;text-transform:uppercase;color:#9A9080;margin-bottom:10px;">Je cherche quelqu'un de</div>
                    <div style="display:flex;gap:6px;flex-wrap:wrap;" id="role-chips">
                        <button onclick="toggleRoleChip(this,'actif')" class="pref-chip">Actif</button>
                        <button onclick="toggleRoleChip(this,'passif')" class="pref-chip">Passif</button>
                        <button onclick="toggleRoleChip(this,'versatile')" class="pref-chip">Versatile</button>
                        <button onclick="toggleRoleChip(this,'peu importe')" class="pref-chip">Peu importe</button>
                    </div>
                </div>

                <button onclick="savePreferences()" style="background:#1E3A2F;border:none;border-radius:2px;padding:13px;font-family:'Syne',sans-serif;font-weight:700;font-size:12px;letter-spacing:.06em;text-transform:uppercase;color:#FDF8F4;cursor:pointer;width:100%;margin-top:4px;">Sauvegarder mes préférences</button>

                <div class="profil-section-lbl" style="margin-top:16px;">Compte</div>
                <div class="profil-row" onclick="goTo('s-admin-login')">
                    <span class="profil-row-left">Accès admin</span>
                    <span class="profil-row-right">→</span>
                </div>
                <button class="btn-danger" onclick="logout()">Se déconnecter</button>
            </div>
        </div>

        <!-- BOTTOM NAV -->
        <nav class="bottom-nav" id="bottom-nav">
            <button class="nav-btn active" id="nav-accueil" onclick="switchTab('accueil')">
                <span class="nav-icon">⊞</span>
                <span class="nav-label">Accueil</span>
                <div class="nav-dot"></div>
            </button>
            <button class="nav-btn" id="nav-matchs" onclick="switchTab('matchs')">
                <span class="nav-icon">✦</span>
                <span class="nav-label">Matchs</span>
                <div class="nav-dot"></div>
            </button>
            <button class="nav-btn" id="nav-profil" onclick="switchTab('profil')">
                <span class="nav-icon">◎</span>
                <span class="nav-label">Profil</span>
                <div class="nav-dot"></div>
            </button>
        </nav>

        <!-- ══ ADMIN LOGIN ══ -->
        <div class="screen" id="s-admin-login">
            <div class="pg-head" style="flex:1;justify-content:center;display:flex;flex-direction:column">
                <div class="pg-eye">Accès réservé</div>
                <div class="pg-title">
                    Dashboard
                    <br>
                    <em>admin</em>
                </div>
                <p class="pg-sub" style="margin-bottom:28px">Gérez vos utilisateurs et matchs.</p>
                <input class="input" id="admin-pw" type="password" placeholder="Mot de passe admin"/>
            </div>
            <div class="pg-foot">
                <button class="btn btn-primary" onclick="adminLogin()">Accéder</button>
                <button class="btn btn-outline" onclick="goTo('s-home')">Retour</button>
            </div>
        </div>

        <!-- ══ ADMIN ══ -->
        <div class="screen" id="s-admin">
            <div class="admin-head">
                <div style="display:flex;justify-content:space-between;align-items:flex-start">
                    <div>
                        <div style="font-family:var(--font-mono);font-size:10px;letter-spacing:.1em;text-transform:uppercase;color:#1E3A2F;margin-bottom:6px">Kino.</div>
                        <div style="font-family:var(--font-sans);font-weight:800;font-size:1.6rem;letter-spacing:-.02em;text-transform:uppercase">Dashboard</div>
                    </div>
                    <button onclick="loadAdmin()" style="background:var(--line2);border:none;border-radius:2px;width:36px;height:36px;cursor:pointer;font-size:16px;color:#1A1208">↻</button>
                </div>
            </div>
            <div class="admin-body">
                <div class="admin-stat-grid">
                    <div class="astat">
                        <div class="astat-num" id="stat-users">–</div>
                        <div class="astat-lbl">Inscrits</div>
                    </div>
                    <div class="astat">
                        <div class="astat-num" id="stat-matches">–</div>
                        <div class="astat-lbl">Matchs</div>
                    </div>
                    <div class="astat">
                        <div class="astat-num" id="stat-waiting">–</div>
                        <div class="astat-lbl">En attente</div>
                    </div>
                    <div class="astat">
                        <div class="astat-num" id="stat-accepted">–</div>
                        <div class="astat-lbl">Acceptés</div>
                    </div>
                </div>
                <div class="section-lbl">Utilisateurs récents</div>
                <div id="admin-users">
                    <div class="spinner"></div>
                </div>
                <div style="margin-top:20px" class="section-lbl">Actions</div>
                <button class="btn btn-primary" onclick="runMatching()" style="margin-bottom:10px">Lancer le matching</button>
                <button class="btn btn-outline" onclick="goTo('s-home')">Retour à l'app</button>
            </div>
        </div>

    </div>
    <!-- #app -->
    <script>
    /* ══ SUPABASE ══ */
    const {createClient} = supabase;
    const sb = createClient(
    'https://kbekoqwcvacwcrzwftir.supabase.co',
    'eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJzdXBhYmFzZSIsInJlZiI6ImtiZWtvcXdjdmFjd2NyendmdGlyIiwicm9sZSI6ImFub24iLCJpYXQiOjE3NzYwODYzNzUsImV4cCI6MjA5MTY2MjM3NX0.gYrzVsno2UZeT_9P6moFMUbubqxXNagG5yXIaACejvg'
    );
    const ADMIN_PASSWORD = '@@Loris002@@';

    /* ══ CARDS DATA ══ */
    // 15 cartes socle obligatoires
    const CARDS_CORE = [
    {
        t: "Je préfère une soirée calme à la maison plutôt qu\'une sortie en boîte.",
        theme: "Mode de vie"
    },
    {
        t: "J\'ai besoin de temps seul pour me ressourcer après avoir vu du monde.",
        theme: "Énergie"
    },
    {
        t: "Je peux parler pendant des heures d\'un sujet qui me passionne.",
        theme: "Communication"
    },
    {
        t: "Je suis plutôt matinal qu\'oiseau de nuit.",
        theme: "Rythme"
    },
    {
        t: "La fidélité, c\'est non-négociable pour moi.",
        theme: "Valeurs"
    },
    {
        t: "Je préfère voyager hors des sentiers battus plutôt que dans les resorts.",
        theme: "Voyages"
    },
    {
        t: "Je préfère un vrai repas cuisiné à un restaurant fancy.",
        theme: "Quotidien"
    },
    {
        t: "J\'assume facilement mes émotions face à quelqu\'un de proche.",
        theme: "Émotions"
    },
    {
        t: "Je lis — livres, articles, peu importe, mais je lis.",
        theme: "Culture"
    },
    {
        t: "L\'humour est indispensable dans une relation.",
        theme: "Relation"
    },
    {
        t: "J\'ai une ambition professionnelle clairement définie.",
        theme: "Vie pro"
    },
    {
        t: "Je veux construire quelque chose de durable avec quelqu\'un.",
        theme: "Projet"
    },
    {
        t: "Je suis à l\'aise avec le silence quand on est ensemble.",
        theme: "Intimité"
    },
    {
        t: "Je préfère parler en face à face plutôt que par messages.",
        theme: "Communication"
    },
    {
        t: "Je fais attention à ce que je mange — par choix, pas par obsession.",
        theme: "Corps"
    },
    ];

    // 100 cartes supplémentaires pour affiner
    const CARDS_EXTRA = [
    {
        t: "Je crois aux coups de foudre.",
        theme: "Relation"
    },
    {
        t: "Je préfère une relation lente qui se construit plutôt qu\'une passion intense.",
        theme: "Relation"
    },
    {
        t: "La jalousie, ça m\'est déjà arrivé et je l\'assume.",
        theme: "Relation"
    },
    {
        t: "Je pense qu\'on peut aimer plusieurs personnes à la fois.",
        theme: "Relation"
    },
    {
        t: "Les disputes font partie d\'une relation saine.",
        theme: "Relation"
    },
    {
        t: "J\'ai besoin qu\'on me montre de l\'affection physiquement.",
        theme: "Relation"
    },
    {
        t: "Je préfère qu\'on se dise les choses franchement, même si ça fait mal.",
        theme: "Relation"
    },
    {
        t: "La distance dans un couple, ça peut fonctionner.",
        theme: "Relation"
    },
    {
        t: "Je fais confiance naturellement, sans avoir à y travailler.",
        theme: "Relation"
    },
    {
        t: "L\'indépendance dans un couple, c\'est aussi important que la complicité.",
        theme: "Relation"
    },
    {
        t: "J\'aime organiser des dîners chez moi.",
        theme: "Social"
    },
    {
        t: "Je préfère avoir peu d\'amis proches plutôt que beaucoup de connaissances.",
        theme: "Social"
    },
    {
        t: "Je suis à l\'aise pour aborder quelqu\'un que je ne connais pas.",
        theme: "Social"
    },
    {
        t: "Les réseaux sociaux me pèsent plus qu\'ils ne m\'apportent.",
        theme: "Social"
    },
    {
        t: "Je préfère les petites soirées intimes aux grandes fêtes.",
        theme: "Social"
    },
    {
        t: "Mon cercle social et ma relation amoureuse, je les garde bien séparés.",
        theme: "Social"
    },
    {
        t: "Je suis souvent celui qui fait le premier pas.",
        theme: "Social"
    },
    {
        t: "J\'ai besoin d\'être entouré régulièrement pour me sentir bien.",
        theme: "Social"
    },
    {
        t: "L\'argent ne me motive pas vraiment — c\'est le sens qui compte.",
        theme: "Argent"
    },
    {
        t: "Je dépense facilement pour des expériences plutôt que des objets.",
        theme: "Argent"
    },
    {
        t: "J\'ai un projet entrepreneurial en tête.",
        theme: "Argent"
    },
    {
        t: "Le succès professionnel est une priorité dans ma vie.",
        theme: "Argent"
    },
    {
        t: "Je préfère la stabilité financière à la prise de risque.",
        theme: "Argent"
    },
    {
        t: "Je pense souvent à mon futur financier.",
        theme: "Argent"
    },
    {
        t: "Je fais du sport régulièrement — au moins 3 fois par semaine.",
        theme: "Corps"
    },
    {
        t: "Le sommeil, c\'est sacré — je ne transige pas là-dessus.",
        theme: "Corps"
    },
    {
        t: "Je consomme de l\'alcool de manière occasionnelle seulement.",
        theme: "Corps"
    },
    {
        t: "Je fume ou j\'ai fumé.",
        theme: "Corps"
    },
    {
        t: "Mon apparence physique m\'importe — pas par vanité, par respect de moi.",
        theme: "Corps"
    },
    {
        t: "Le bien-être mental est aussi important que la santé physique.",
        theme: "Corps"
    },
    {
        t: "Je médite ou j\'ai des pratiques de mindfulness.",
        theme: "Corps"
    },
    {
        t: "Je vais au cinéma seul parfois — et j\'aime ça.",
        theme: "Culture"
    },
    {
        t: "La musique occupe une vraie place dans mon quotidien.",
        theme: "Culture"
    },
    {
        t: "Je joue à des jeux vidéo ou j\'en ai joué sérieusement.",
        theme: "Culture"
    },
    {
        t: "J\'aime les musées, mais pas tous — j\'ai des goûts précis.",
        theme: "Culture"
    },
    {
        t: "La politique m\'intéresse et j\'ai des convictions claires.",
        theme: "Culture"
    },
    {
        t: "Je regarde des séries en VO.",
        theme: "Culture"
    },
    {
        t: "J\'écoute des podcasts régulièrement.",
        theme: "Culture"
    },
    {
        t: "Je vais à des expos ou des événements culturels seul si besoin.",
        theme: "Culture"
    },
    {
        t: "La littérature classique m\'intéresse autant que la contemporaine.",
        theme: "Culture"
    },
    {
        t: "J\'ai un domaine de passion que peu de gens autour de moi partagent.",
        theme: "Culture"
    },
    {
        t: "Je voyage pour l\'expérience humaine, pas pour les paysages.",
        theme: "Voyages"
    },
    {
        t: "Je préfère rester longtemps dans un endroit plutôt que d\'en voir beaucoup.",
        theme: "Voyages"
    },
    {
        t: "J\'aime les destinations peu touristiques.",
        theme: "Voyages"
    },
    {
        t: "Je voyage léger — un sac à dos suffit.",
        theme: "Voyages"
    },
    {
        t: "J\'ai déjà voyagé seul et j\'ai adoré ça.",
        theme: "Voyages"
    },
    {
        t: "Je m\'adapte facilement à des conditions de vie différentes.",
        theme: "Voyages"
    },
    {
        t: "Les week-ends spontanés, j\'adore.",
        theme: "Voyages"
    },
    {
        t: "Je veux des enfants — c\'est clair dans ma tête.",
        theme: "Famille"
    },
    {
        t: "Je suis proche de ma famille.",
        theme: "Famille"
    },
    {
        t: "J\'ai une relation complexe avec ma famille, et je l\'assume.",
        theme: "Famille"
    },
    {
        t: "Je veux vivre à Paris encore longtemps.",
        theme: "Famille"
    },
    {
        t: "Je me vois vivre ailleurs qu\'en France dans le futur.",
        theme: "Famille"
    },
    {
        t: "La cohabitation en couple tôt, ça ne me fait pas peur.",
        theme: "Famille"
    },
    {
        t: "Le mariage, ça m\'intéresse — pas juste comme formalité.",
        theme: "Famille"
    },
    {
        t: "Je suis quelqu\'un de têtu — et j\'en suis conscient.",
        theme: "Caractère"
    },
    {
        t: "Je prends les décisions rapidement sans trop hésiter.",
        theme: "Caractère"
    },
    {
        t: "Je suis perfectionniste dans ce qui compte pour moi.",
        theme: "Caractère"
    },
    {
        t: "J\'ai tendance à trop analyser les situations.",
        theme: "Caractère"
    },
    {
        t: "Je m\'ennuie rarement — je trouve toujours quelque chose à faire.",
        theme: "Caractère"
    },
    {
        t: "Je suis quelqu\'un de généreux, parfois au détriment de moi-même.",
        theme: "Caractère"
    },
    {
        t: "J\'ai un humour qui ne plaît pas à tout le monde — et tant mieux.",
        theme: "Caractère"
    },
    {
        t: "Je suis à l\'aise pour parler de moi à quelqu\'un que je viens de rencontrer.",
        theme: "Caractère"
    },
    {
        t: "Je suis curieux de nature — presque tout m\'intéresse.",
        theme: "Caractère"
    },
    {
        t: "J\'ai du mal à demander de l\'aide.",
        theme: "Caractère"
    },
    {
        t: "J\'ai fait une thérapie ou j\'en fais une — sans honte.",
        theme: "Émotions"
    },
    {
        t: "Je sais reconnaître quand je ne vais pas bien.",
        theme: "Émotions"
    },
    {
        t: "J\'exprime facilement ma gratitude aux gens que j\'aime.",
        theme: "Émotions"
    },
    {
        t: "La solitude me ressource — elle ne me pèse pas.",
        theme: "Émotions"
    },
    {
        t: "J\'ai des peurs que je n\'ai pas encore tout à fait surmontées.",
        theme: "Émotions"
    },
    {
        t: "Je pleure facilement devant un film ou une chanson.",
        theme: "Émotions"
    },
    {
        t: "Je suis capable de m\'excuser sincèrement quand j\'ai tort.",
        theme: "Émotions"
    },
    {
        t: "Je fais confiance à mon instinct pour les décisions importantes.",
        theme: "Émotions"
    },
    {
        t: "Mon appartement reflète vraiment qui je suis.",
        theme: "Quotidien"
    },
    {
        t: "Je cuisine régulièrement — pas juste pour survivre.",
        theme: "Quotidien"
    },
    {
        t: "Je suis plutôt ordonné dans mon espace de vie.",
        theme: "Quotidien"
    },
    {
        t: "J\'aime les matinées calmes avant que la journée commence.",
        theme: "Quotidien"
    },
    {
        t: "J\'ai des rituels quotidiens auxquels je tiens.",
        theme: "Quotidien"
    },
    {
        t: "Je préfère les transports en commun à la voiture en ville.",
        theme: "Quotidien"
    },
    {
        t: "J\'achète peu mais je choisis bien.",
        theme: "Quotidien"
    },
    {
        t: "J\'aime prendre le temps de bien manger même seul.",
        theme: "Quotidien"
    },
    {
        t: "La séduction intellectuelle m\'attire autant que la séduction physique.",
        theme: "Intimité"
    },
    {
        t: "Je suis à l\'aise pour parler de sexualité avec quelqu\'un de confiance.",
        theme: "Intimité"
    },
    {
        t: "L\'intimité émotionnelle passe avant l\'intimité physique pour moi.",
        theme: "Intimité"
    },
    {
        t: "Je suis quelqu\'un d\'affectueux — câlins, tendresse, tout ça compte.",
        theme: "Intimité"
    },
    {
        t: "J\'ai des limites claires et je sais les exprimer.",
        theme: "Intimité"
    },
    {
        t: "L\'écologie influence mes choix du quotidien.",
        theme: "Valeurs"
    },
    {
        t: "Je m\'engage ou je me suis engagé pour une cause.",
        theme: "Valeurs"
    },
    {
        t: "Je vote et je pense que ça compte.",
        theme: "Valeurs"
    },
    {
        t: "La spiritualité a une place dans ma vie.",
        theme: "Valeurs"
    },
    {
        t: "Je crois que les gens peuvent changer profondément.",
        theme: "Valeurs"
    },
    {
        t: "L\'honnêteté prime sur la diplomatie pour moi.",
        theme: "Valeurs"
    },
    {
        t: "Je respecte les gens qui pensent différemment de moi.",
        theme: "Valeurs"
    },
    {
        t: "La loyauté envers mes amis est quelque chose que je prends très au sérieux.",
        theme: "Valeurs"
    },
    {
        t: "J\'aime débattre — pas pour gagner, pour comprendre.",
        theme: "Communication"
    },
    {
        t: "Je préfère écrire que parler pour exprimer des choses importantes.",
        theme: "Communication"
    },
    {
        t: "Je déteste les non-dits dans une relation.",
        theme: "Communication"
    },
    {
        t: "Je suis un bon auditeur — les gens viennent naturellement me parler.",
        theme: "Communication"
    },
    ];

    // CARDS = les 15 socle
    const CARDS = CARDS_CORE;

    // Cartes extra non encore répondues, mélangées (15 à la fois)
    function getExtraCards(reponses) {
        const answeredIndexes = new Set((reponses || []).map(r => r.card_index));
        const available = CARDS_EXTRA
        .map((c, i) => ({
            ...c,
            card_index: 1000 + i
        }))
        .filter(c => !answeredIndexes.has(c.card_index));
        for (let i = available.length - 1; i > 0; i--) {
            const j = Math.floor(Math.random() * (i + 1));
            [available[i], available[j]] = [available[j], available[i]];
        }
        return available.slice(0, 15);
    }

    /* ══ STATE ══ */
    const st = {
        genre: null,
        recherche: null,
        reponses: [],
        prenom: '',
        email: '',
        age: 0,
        userId: null,
        authUser: null,
        otpContext: null
    };
    let cardIdx = 0,
        tabCardIdx = 0,
        dragX = 0,
        dragStartX = 0,
        isDragging = false,
        selectedSlot = null;

    const SLOTS = [
    {
        day: 'Samedi 19 avril',
        time: '19h00',
        sub: 'Soirée'
    },
    {
        day: 'Samedi 19 avril',
        time: '20h30',
        sub: 'Soirée tardive'
    },
    {
        day: 'Dimanche 20 avril',
        time: '12h00',
        sub: 'Déjeuner'
    },
    {
        day: 'Dimanche 20 avril',
        time: '17h00',
        sub: 'Après-midi'
    },
    ];

    /* ══ NAV ══ */
    function goBack() {
        // Retourner à l'écran précédent selon le contexte
        if (st.otpContext === 'login')
            goTo('s-login');
        else
            goTo('s-signup');
    }
    function goTo(id) {
        document.querySelectorAll('.screen').forEach(s => {
            if (s.classList.contains('active')) {
                s.classList.add('exit');
                setTimeout(() => s.classList.remove('active', 'exit'), 380);
            }
        });
        setTimeout(() => {
            const target = document.getElementById(id);
            if (target)
                target.classList.add('active');
        }, 50);
    }
    function showApp() {
        document.querySelectorAll('.screen').forEach(s => s.classList.remove('active'));
        document.getElementById('bottom-nav').classList.add('visible');
        switchTab('accueil');
        // Load data sequentially after profile is set
        setTimeout(() => {
            loadProfileData();
            loadMatchs();
            renderTabCards();
        }, 100);
    }
    function switchTab(tab) {
        document.querySelectorAll('.tab-screen').forEach(s => s.classList.remove('active'));
        document.querySelectorAll('.nav-btn').forEach(b => b.classList.remove('active'));
        document.getElementById('tab-' + tab).classList.add('active');
        document.getElementById('nav-' + tab).classList.add('active');
    }
    function showToast(msg, dur=3000) {
        const t = document.getElementById('toast');
        t.textContent = msg;
        t.classList.add('show');
        setTimeout(() => t.classList.remove('show'), dur);
    }

    /* ══ OTP AUTH ══ */
    async function sendOTP(context) {
        const email = (context === 'login' ? document.getElementById('login-email') : document.getElementById('ie')).value.trim();
        if (!email || !email.includes('@')) {
            showToast('Email invalide');
            return;
        }
        st.otpContext = context;
        st.email = email;

        // Vérifier si l'email existe déjà
        const {data: existing} = await sb.from('users').select('id').eq('email', email).limit(1);
        const hasAccount = existing && existing.length > 0;

        if (context === 'signup' && hasAccount) {
            showToast('Tu as déjà un compte Kino !', 3000);
            setTimeout(() => {
                document.getElementById('login-email').value = email;
                goTo('s-login');
                showToast('Entre ton email pour te connecter.');
            }, 1600);
            return;
        }

        if (context === 'login' && !hasAccount) {
            showToast('Pas encore de compte.', 3000);
            setTimeout(() => {
                document.getElementById('ie').value = email;
                goTo('s-signup');
                showToast('Crée ton profil pour commencer.');
            }, 1600);
            return;
        }

        showToast('Envoi du code…', 4000);
        const {error} = await sb.auth.signInWithOtp({
            email,
            options: {
                shouldCreateUser: true
            }
        });
        if (error) {
            showToast('Erreur : ' + error.message);
            return;
        }
        document.getElementById('otp-email-display').textContent = email;
        goTo('s-otp');
        setupOTPInputs();
        showToast('Code envoyé ! Vérifie tes emails.');
    }
    function setupOTPInputs() {
        const digits = document.querySelectorAll('.otp-digit');
        digits.forEach((d, i) => {
            d.value = '';
            d.oninput = () => {
                if (d.value.length === 1 && i < digits.length - 1)
                    digits[i + 1].focus();
            };
            d.onkeydown = (e) => {
                if (e.key === 'Backspace' && !d.value && i > 0)
                    digits[i - 1].focus();
            };
        });
        setTimeout(() => digits[0].focus(), 300);
    }

    async function verifyOTP() {
        const digits = document.querySelectorAll('.otp-digit');
        const token = Array.from(digits).map(d => d.value).join('');
        if (token.length < 8) {
            showToast('Entre les 8 chiffres');
            return;
        }
        showToast('Vérification…', 3000);
        const {data, error} = await sb.auth.verifyOtp({
            email: st.email,
            token,
            type: 'email'
        });
        if (error) {
            showToast('Code incorrect ou expiré');
            return;
        }
        st.authUser = data.user;
        if (st.otpContext === 'login') {
            await loadExistingProfile();
        }
        else {
            goTo('s-recherche');
        }
    }

    async function loadExistingProfile() {
        const {data} = await sb.from('users').select('*').eq('auth_id', st.authUser.id).single();
        if (data) {
            st.userId = data.id;
            st.prenom = data.prenom;
            st.age = data.age;
            st.genre = data.genre;
            st.recherche = data.recherche_genre;
            st.reponses = data.reponses || [];
            showApp();
        } else {
            // Chercher par email aussi
            const {data: byEmail} = await sb.from('users').select('*').eq('email', st.email).single();
            if (byEmail) {
                st.userId = byEmail.id;
                st.prenom = byEmail.prenom;
                st.age = byEmail.age;
                st.genre = byEmail.genre;
                st.recherche = byEmail.recherche_genre;
                st.reponses = byEmail.reponses || [];
                // Mettre à jour auth_id
                await sb.from('users').update({
                    auth_id: st.authUser.id
                }).eq('id', byEmail.id);
                showApp();
            } else {
                goTo('s-signup');
                showToast('Complète ton profil pour continuer');
            }
        }
    }

    /* ══ ONBOARDING PREFS ══ */
    let onbGenres = ['tous'];
    let onbRole = ['peu importe'];

    function toggleOnbGenre(el, val) {
        if (val === 'tous') {
            onbGenres = ['tous'];
            document.querySelectorAll('#onb-genre-chips .pref-chip').forEach(c => {
                c.classList.toggle('active', c.textContent.toLowerCase() === 'tous');
            });
            return;
        }
        onbGenres = onbGenres.filter(g => g !== 'tous');
        document.querySelector('#onb-genre-chips .pref-chip:last-child').classList.remove('active');
        if (onbGenres.includes(val)) {
            onbGenres = onbGenres.filter(g => g !== val);
            el.classList.remove('active');
        } else {
            onbGenres.push(val);
            el.classList.add('active');
        }
        if (onbGenres.length === 0) {
            onbGenres = ['tous'];
            document.querySelector('#onb-genre-chips .pref-chip:last-child').classList.add('active');
        }
    }

    function toggleOnbRole(el, val) {
        onbRole = [val];
        document.querySelectorAll('#onb-role-chips .pref-chip').forEach(c => c.classList.remove('active'));
        el.classList.add('active');
    }

    function updateOnbAge() {
        let min = parseInt(document.getElementById('onb-age-min').value);
        let max = parseInt(document.getElementById('onb-age-max').value);
        if (min > max) {
            if (event.target.id === 'onb-age-min')
                min = max;
            else
                max = min;
            document.getElementById('onb-age-min').value = min;
            document.getElementById('onb-age-max').value = max;
        }
        document.getElementById('onb-age-label').textContent = min + ' – ' + max + ' ans';
    }

    function startQFromPrefs() {
        // Sauvegarder les préférences dans st pour les enregistrer avec le profil
        st.pref_genres = onbGenres;
        st.pref_age_min = parseInt(document.getElementById('onb-age-min').value);
        st.pref_age_max = parseInt(document.getElementById('onb-age-max').value);
        st.pref_roles = onbRole;

        // Pré-remplir la page profil "Je cherche"
        setTimeout(() => {
            // Sync avec les chips du profil
            document.querySelectorAll('#genre-chips .pref-chip').forEach(c => {
                c.classList.toggle('active', onbGenres.includes(c.textContent.toLowerCase()));
            });
            selectedGenres = [...onbGenres];
            document.querySelectorAll('#role-chips .pref-chip').forEach(c => {
                c.classList.toggle('active', onbRole.includes(c.textContent.toLowerCase()));
            });
            selectedRoles = [...onbRole];
            document.getElementById('age-min').value = st.pref_age_min;
            document.getElementById('age-max').value = st.pref_age_max;
            updateAgeRange();
        }, 100);

        startQ();
    }

    /* ══ ONBOARDING PREFS ══ */

    function toggleOnbGenre(el, val) {
        if (val === 'tous') {
            onbGenres = ['tous'];
            document.querySelectorAll('#onb-genre-chips .pref-chip').forEach(c => {
                c.classList.toggle('active', c.textContent.toLowerCase() === 'tous');
            });
            return;
        }
        onbGenres = onbGenres.filter(g => g !== 'tous');
        document.querySelector('#onb-genre-chips .pref-chip:last-child').classList.remove('active');
        if (onbGenres.includes(val)) {
            onbGenres = onbGenres.filter(g => g !== val);
            el.classList.remove('active');
        }
        else {
            onbGenres.push(val);
            el.classList.add('active');
        }
        if (onbGenres.length === 0) {
            onbGenres = ['tous'];
            document.querySelector('#onb-genre-chips .pref-chip:last-child').classList.add('active');
        }
    }

    function toggleOnbRole(el, val) {
        onbRole = [val];
        document.querySelectorAll('#onb-role-chips .pref-chip').forEach(c => c.classList.remove('active'));
        el.classList.add('active');
    }

    function updateOnbAge() {
        let min = parseInt(document.getElementById('onb-age-min').value);
        let max = parseInt(document.getElementById('onb-age-max').value);
        if (min > max) {
            if (event.target.id === 'onb-age-min')
                min = max;
            else
                max = min;
            document.getElementById('onb-age-min').value = min;
            document.getElementById('onb-age-max').value = max;
        }
        document.getElementById('onb-age-label').textContent = min + ' – ' + max + ' ans';
    }

    function startQFromPrefs() {
        st.pref_genres = onbGenres;
        st.pref_age_min = parseInt(document.getElementById('onb-age-min').value);
        st.pref_age_max = parseInt(document.getElementById('onb-age-max').value);
        st.pref_roles = onbRole;
        // Pré-remplir le profil
        setTimeout(() => {
            selectedGenres = [...onbGenres];
            selectedRoles = [...onbRole];
            document.querySelectorAll('#genre-chips .pref-chip').forEach(c => {
                c.classList.toggle('active', onbGenres.includes(c.textContent.toLowerCase()));
            });
            document.querySelectorAll('#role-chips .pref-chip').forEach(c => {
                c.classList.toggle('active', onbRole.includes(c.textContent.toLowerCase()));
            });
            if (document.getElementById('age-min')) {
                document.getElementById('age-min').value = st.pref_age_min;
                document.getElementById('age-max').value = st.pref_age_max;
                updateAgeRange();
            }
        }, 200);
        startQ();
    }

    /* ══ SIGNUP ══ */
    function sg(b, v) {
        st.genre = v;
        document.querySelectorAll('.g-opt').forEach(x => x.classList.remove('sel'));
        b.classList.add('sel');
    }
    function sr(b, v) {
        st.recherche = v;
        document.querySelectorAll('.rech-item').forEach(x => x.classList.remove('sel'));
        b.classList.add('sel');
    }
    function vsignup() {
        const p = document.getElementById('ip').value.trim();
        const a = document.getElementById('ia').value;
        const e = document.getElementById('ie').value.trim();
        if (!p || !a || !e || !st.genre) {
            showToast('Remplis tous les champs');
            return;
        }
        if (parseInt(a) < 18) {
            showToast('Tu dois avoir 18 ans minimum');
            return;
        }
        if (!e.includes('@')) {
            showToast('Email invalide');
            return;
        }
        st.prenom = p;
        st.email = e;
        st.age = parseInt(a);
        sendOTP('signup');
    }
    function startQ() {
        if (!st.recherche) {
            showToast('Indique ce que tu recherches');
            return;
        }
        cardIdx = 0;
        st.reponses = [];
        renderStack('card-stack', 'qbars', 'qcount', cardIdx);
        goTo('s-questions');
    }

    /* ══ CARDS ENGINE ══ */
    function renderStack(stackId, barsId, countId, idx) {
        const stack = document.getElementById(stackId);
        stack.innerHTML = '';
        const bars = document.getElementById(barsId);
        bars.innerHTML = '';
        CARDS.forEach((_, i) => {
            const b = document.createElement('div');
            b.className = 'qb' + (i < idx ? ' done' : i === idx ? ' now' : '');
            bars.appendChild(b);
        });
        document.getElementById(countId).textContent = (idx + 1) + ' / ' + CARDS.length;
        for (let i = Math.min(idx + 2, CARDS.length - 1); i >= idx; i--) {
            if (i >= CARDS.length)
                continue;
            const layer = i - idx;
            const el = document.createElement('div');
            el.className = 'flash-card ' + (layer === 0 ? 'top' : layer === 1 ? 'behind-1' : 'behind-2');
            el.innerHTML = `
                        <div class="vote-overlay vote-yes"><div class="vote-label">Oui</div></div>
                        <div class="vote-overlay vote-no"><div class="vote-label">Non</div></div>
                        <div class="vote-overlay vote-maybe"><div class="vote-label">Peut-être</div></div>
                        <div class="card-num">Carte ${String(i + 1).padStart(2, '0')} — ${CARDS[i].theme}</div>
                        <div class="card-body"><div class="card-text">« ${CARDS[i].t} »</div></div>
                        <div class="card-theme">${CARDS[i].theme.toLowerCase()}</div>`;
            if (layer === 0)
                attachDrag(el, stackId === 'card-stack' ? 'signup' : 'tab');
            stack.appendChild(el);
        }
    }

    function attachDrag(el, ctx) {
        const move = (dx) => {
            el.style.transform = `translateX(${dx}px) rotate(${dx * 0.06}deg)`;
            el.querySelector('.vote-yes').style.opacity = Math.max(0, dx / 80);
            el.querySelector('.vote-no').style.opacity = Math.max(0, -dx / 80);
        };
        const end = (dx) => {
            el.style.transition = '';
            haptic('medium');
            if (dx > 80)
                ctx === 'signup' ? vote('yes') : tabVote('yes');
            else if (dx < -80) {
                haptic('light');
                ctx === 'signup' ? vote('no') : tabVote('no');
            }
            else {
                el.style.transform = '';
                el.querySelectorAll('.vote-overlay').forEach(o => o.style.opacity = 0);
            }
        };
        el.addEventListener('mousedown', e => {
            isDragging = true;
            dragStartX = e.clientX;
            el.style.transition = 'none';
        });
        document.addEventListener('mousemove', e => {
            if (!isDragging)
                return;
            dragX = e.clientX - dragStartX;
            move(dragX);
        });
        document.addEventListener('mouseup', () => {
            if (!isDragging)
                return;
            isDragging = false;
            end(dragX);
            dragX = 0;
        });
        el.addEventListener('touchstart', e => {
            dragStartX = e.touches[0].clientX;
            el.style.transition = 'none';
        }, {
            passive: true
        });
        el.addEventListener('touchmove', e => {
            dragX = e.touches[0].clientX - dragStartX;
            move(dragX);
        }, {
            passive: true
        });
        el.addEventListener('touchend', () => {
            end(dragX);
            dragX = 0;
        });
    }

    function vote(v) {
        if (cardIdx >= CARDS.length)
            return;
        const top = document.querySelector('#card-stack .top');
        if (!top)
            return;
        st.reponses.push({
            card_index: cardIdx,
            vote: v
        });
        top.querySelector('.vote-yes').style.opacity = v === 'yes' ? 1 : 0;
        top.querySelector('.vote-no').style.opacity = v === 'no' ? 1 : 0;
        top.querySelector('.vote-maybe').style.opacity = v === 'maybe' ? 1 : 0;
        top.classList.add(v === 'yes' ? 'fly-right' : v === 'no' ? 'fly-left' : 'fly-up');
        cardIdx++;
        setTimeout(async () => {
            if (cardIdx >= CARDS.length) {
                await saveUser();
                showApp();
            }
            else
                renderStack('card-stack', 'qbars', 'qcount', cardIdx);
        }, 380);
    }

    function tabVote(v) {
        const top = document.querySelector('#tab-card-stack .top');
        if (!top)
            return;
        const coreDone = st.reponses.filter(r => r.card_index < 1000).length >= CARDS_CORE.length;

        if (!coreDone) {
            // Vote sur carte socle
            st.reponses.push({
                card_index: tabCardIdx,
                vote: v
            });
            top.querySelector('.vote-yes').style.opacity = v === 'yes' ? 1 : 0;
            top.querySelector('.vote-no').style.opacity = v === 'no' ? 1 : 0;
            top.querySelector('.vote-maybe').style.opacity = v === 'maybe' ? 1 : 0;
            top.classList.add(v === 'yes' ? 'fly-right' : v === 'no' ? 'fly-left' : 'fly-up');
            tabCardIdx++;
            setTimeout(async () => {
                await updateResponses();
                renderTabCards();
            }, 380);
        } else {
            // Vote sur carte extra
            if (!extraCards || extraCards.length === 0)
                return;
            const card = extraCards[0];
            st.reponses.push({
                card_index: card.card_index,
                vote: v
            });
            top.querySelector('.vote-yes').style.opacity = v === 'yes' ? 1 : 0;
            top.querySelector('.vote-no').style.opacity = v === 'no' ? 1 : 0;
            top.querySelector('.vote-maybe').style.opacity = v === 'maybe' ? 1 : 0;
            top.classList.add(v === 'yes' ? 'fly-right' : v === 'no' ? 'fly-left' : 'fly-up');
            extraCards.shift();
            setTimeout(async () => {
                await updateResponses();
                // renderTabCards va garder le batch existant s'il reste des cartes
                renderTabCards();
            }, 380);
        }
    }

    let extraCards = [];
    let extraCardIdx = 0;

    function renderTabCards() {
        const coreDone = st.reponses.filter(r => r.card_index < 1000).length >= CARDS_CORE.length;

        if (!coreDone) {
            document.getElementById('tab-card-area').style.display = 'flex';
            document.getElementById('tab-done').style.display = 'none';
            tabCardIdx = st.reponses.filter(r => r.card_index < 1000).length;
            renderStack('tab-card-stack', 'tab-qbars', 'tab-qcount', tabCardIdx);
        } else {
            // Socle terminé — afficher les extra
            // NE PAS régénérer extraCards s'il en reste encore — garder le même batch
            if (extraCards.length === 0) {
                // Batch épuisé ou premier appel — charger un nouveau batch
                extraCards = getExtraCards(st.reponses);
            }

            if (extraCards.length === 0) {
                document.getElementById('tab-card-area').style.display = 'none';
                document.getElementById('tab-done').style.display = 'block';
                document.getElementById('tab-done').innerHTML = `
                                <div style="font-size:2.5rem;margin-bottom:20px">✓</div>
                                <div style="font-family:var(--font-sans);font-weight:800;font-size:1.3rem;text-transform:uppercase;letter-spacing:-.01em;margin-bottom:8px;color:#1A1208;">Toutes les cartes répondues !</div>
                                <p style="font-size:14px;font-style:italic;color:#5A4E3A;line-height:1.6;">Tu as répondu à ${st.reponses.length} cartes. Ton profil est très précis — on cherche quelqu’un pour toi.</p>`;
            } else {
                document.getElementById('tab-card-area').style.display = 'flex';
                document.getElementById('tab-done').style.display = 'none';
                renderExtraStack();
            }
        }
    }

    function renderExtraStack() {
        const stack = document.getElementById('tab-card-stack');
        stack.innerHTML = '';
        const bars = document.getElementById('tab-qbars');
        bars.innerHTML = '';

        // Barre de progression extra
        const total = CARDS_EXTRA.length;
        const done = st.reponses.filter(r => r.card_index >= 1000).length;
        for (let i = 0; i < Math.min(extraCards.length, 15); i++) {
            const b = document.createElement('div');
            b.className = 'qb' + (i === 0 ? 'now' : '');
            bars.appendChild(b);
        }
        document.getElementById('tab-qcount').textContent = '';

        for (let i = Math.min(2, extraCards.length - 1); i >= 0; i--) {
            if (i >= extraCards.length)
                continue;
            const card = extraCards[i];
            const layer = i;
            const el = document.createElement('div');
            el.className = 'flash-card ' + (layer === 0 ? 'top' : layer === 1 ? 'behind-1' : 'behind-2');
            el.innerHTML = `
                        <div class="vote-overlay vote-yes"><div class="vote-label">Oui</div></div>
                        <div class="vote-overlay vote-no"><div class="vote-label">Non</div></div>
                        <div class="vote-overlay vote-maybe"><div class="vote-label">Peut-être</div></div>
                        <div class="card-num">Extra — ${card.theme}</div>
                        <div class="card-body"><div class="card-text">« ${card.t} »</div></div>
                        <div class="card-theme">${card.theme.toLowerCase()}</div>`;
            if (layer === 0)
                attachDrag(el, 'tab');
            stack.appendChild(el);
        }
    }

    /* ══ SAVE USER ══ */
    async function saveUser() {
        try {
            const {data, error} = await sb.from('users').insert({
                prenom: st.prenom,
                email: st.email,
                age: st.age,
                genre: st.genre,
                recherche_genre: st.recherche,
                reponses: st.reponses,
                statut_match: 'en_attente',
                auth_id: st.authUser ? st.authUser.id : null,
                created_at: new Date().toISOString(),
                pref_genres: st.pref_genres || ['tous'],
                pref_age_min: st.pref_age_min || 18,
                pref_age_max: st.pref_age_max || 99,
                pref_roles: st.pref_roles || ['peu importe'],
            }).select();
            if (error)
                throw error;
            if (data && data[0]) {
                st.userId = data[0].id;
                showToast('✓ Profil créé !');
            }
        } catch (e) {
            showToast(e.message && (e.message.includes('unique') || e.message.includes('duplicate')) ? 'Email déjà inscrit' : 'Erreur — réessaie');
            console.error(e);
        }
    }
    async function updateResponses() {
        if (!st.userId)
            return;
        await sb.from('users').update({
            reponses: st.reponses
        }).eq('id', st.userId);
    }

    /* ══ PROFILE ══ */
    async function loadProfileData() {
        document.getElementById('profil-av').textContent = st.prenom ? st.prenom.charAt(0).toUpperCase() : '?';
        document.getElementById('profil-name').textContent = st.prenom || '—';
        document.getElementById('profil-email').textContent = st.email || '—';
        document.getElementById('profil-row-prenom').textContent = st.prenom || '—';
        document.getElementById('profil-row-age').textContent = st.age || '—';
        document.getElementById('profil-row-genre').textContent = st.genre || '—';
        document.getElementById('profil-stat-cards').textContent = st.reponses ? st.reponses.length : 0;
        if (st.userId && st.userId !== 'undefined') {
            const {data} = await sb.from('matches').select('id').or(`user_a.eq.${st.userId},user_b.eq.${st.userId}`);
            document.getElementById('profil-stat-matchs').textContent = data ? data.length : 0;
            await loadPreferences();
        }
    }

    /* ══ DETAIL ══ */
    function openDetail(match, name, score) {
        document.getElementById('detail-av-a').textContent = st.prenom ? st.prenom.charAt(0).toUpperCase() : '?';
        document.getElementById('detail-name').textContent = name;
        document.getElementById('detail-score').innerHTML = score + '<sup>%</sup>';
        const slotsEl = document.getElementById('detail-slots');
        slotsEl.innerHTML = '';
        selectedSlot = null;
        SLOTS.forEach((s, i) => {
            const el = document.createElement('div');
            el.className = 'slot';
            el.innerHTML = `<div><div class="slot-info">${s.day} · ${s.time}</div><div class="slot-sub">${s.sub}</div></div><div class="slot-chk">✓</div>`;
            el.onclick = () => {
                document.querySelectorAll('.slot').forEach(x => x.classList.remove('sel'));
                el.classList.add('sel');
                selectedSlot = i;
            };
            slotsEl.appendChild(el);
        });
        const detail = document.getElementById('match-detail');
        detail.style.display = 'flex';
        setTimeout(() => detail.classList.add('open'), 10);
        detail.dataset.matchId = match.id;
    }
    function closeDetail() {
        const d = document.getElementById('match-detail');
        d.classList.remove('open');
        setTimeout(() => d.style.display = 'none', 350);
    }
    async function acceptDate() {
        if (selectedSlot === null) {
            showToast('Choisis un créneau');
            return;
        }
        const matchId = document.getElementById('match-detail').dataset.matchId;
        const slot = SLOTS[selectedSlot];
        await sb.from('matches').update({
            statut: 'accepte',
            slot_jour: slot.day,
            slot_heure: slot.time
        }).eq('id', matchId);
        showToast('🎉 Date confirmé !');
        closeDetail();
        setTimeout(() => loadMatchs(), 400);
    }

    /* ══ LOGOUT ══ */
    async function logout() {
        await sb.auth.signOut();
        Object.assign(st, {
            authUser: null,
            userId: null,
            prenom: '',
            email: '',
            reponses: [],
            genre: null,
            recherche: null
        });
        document.getElementById('bottom-nav').classList.remove('visible');
        document.querySelectorAll('.tab-screen').forEach(s => s.classList.remove('active'));
        goTo('s-home');
    }

    /* ══ ADMIN ══ */
    function adminLogin() {
        if (document.getElementById('admin-pw').value === ADMIN_PASSWORD) {
            goTo('s-admin');
            loadAdmin();
        }
        else
            showToast('Mot de passe incorrect');
    }
    async function loadAdmin() {
        document.getElementById('admin-users').innerHTML = '<div class="spinner"></div>';
        try {
            const {data: users} = await sb.from('users').select('*').order('created_at', {
                ascending: false
            }).limit(50);
            const {data: matches} = await sb.from('matches').select('id,statut');
            document.getElementById('stat-users').textContent = users ? users.length : 0;
            document.getElementById('stat-matches').textContent = matches ? matches.length : 0;
            document.getElementById('stat-waiting').textContent = users ? users.filter(u => u.statut_match === 'en_attente').length : 0;
            document.getElementById('stat-accepted').textContent = matches ? matches.filter(m => m.statut === 'accepte').length : 0;
            if (!users || users.length === 0) {
                document.getElementById('admin-users').innerHTML = '<p style="font-size:13px;font-style:italic;color:#9A9080">Aucun utilisateur.</p>';
                return;
            }
            document.getElementById('admin-users').innerHTML = users.slice(0, 15).map(u => `
                        <div class="user-row">
                            <div class="user-av">${u.prenom ? u.prenom.charAt(0).toUpperCase() : '?'}</div>
                            <div style="flex:1;min-width:0">
                                <div class="user-name">${u.prenom || '–'}, ${u.age || '–'} ans</div>
                                <div class="user-info">${u.genre || '–'} · cherche ${u.recherche_genre || '–'}</div>
                                <div class="user-info">${u.email || ''}</div>
                            </div>
                            <span class="user-badge ${u.statut_match === 'en_attente' ? 'badge-wait' : 'badge-match'}">${u.statut_match === 'en_attente' ? 'Attente' : 'Matché'}</span>
                        </div>`).join('');
        } catch (e) {
            document.getElementById('admin-users').innerHTML = '<p style="font-size:13px;color:#C0392B">Erreur Supabase.</p>';
        }
    }

    function compatibilityScore(repA, repB) {
        if (!repA || !repB || repA.length === 0)
            return 0;
        const common = repA.filter(a => {
            const b = repB.find(r => r.card_index === a.card_index);
            return b && b.vote === a.vote;
        });
        return Math.round((common.length / repA.length) * 100);
    }

    function hardFiltersPass(userA, userB) {
        // -- Genre --
        const genresA = userA.pref_genres || ['tous'];
        const genresB = userB.pref_genres || ['tous'];
        const genreOK = (genres, genre) => genres.includes('tous') || genres.includes(genre);
        if (!genreOK(genresA, userB.genre))
            return false;
        if (!genreOK(genresB, userA.genre))
            return false;

        // -- Âge --
        const minA = userA.pref_age_min || 18,
            maxA = userA.pref_age_max || 99;
        const minB = userB.pref_age_min || 18,
            maxB = userB.pref_age_max || 99;
        if (userB.age < minA || userB.age > maxA)
            return false;
        if (userA.age < minB || userA.age > maxB)
            return false;

        // -- Rôle (compatibilité) --
        const rolesA = userA.pref_roles || ['peu importe'];
        const rolesB = userB.pref_roles || ['peu importe'];
        const roleCompat = (rolesA, rolesB) => {
            if (rolesA.includes('peu importe') || rolesB.includes('peu importe'))
                return true;
            // Actif + Passif = compatible, Versatile + tout = compatible
            if (rolesA.includes('versatile') || rolesB.includes('versatile'))
                return true;
            if (rolesA.includes('actif') && rolesB.includes('passif'))
                return true;
            if (rolesA.includes('passif') && rolesB.includes('actif'))
                return true;
            return false;
        };
        if (!roleCompat(rolesA, rolesB))
            return false;

        return true;
    }

    async function runMatching() {
        showToast('Analyse en cours…', 5000);
        try {
            const {data: users} = await sb.from('users').select('*').eq('statut_match', 'en_attente').order('created_at');
            if (!users || users.length < 2) {
                showToast('Pas assez de profils');
                return;
            }
            let matched = 0;
            const used = new Set();
            for (let i = 0; i < users.length; i++) {
                if (used.has(users[i].id))
                    continue;
                const {data: exA} = await sb.from('matches').select('id').or(`user_a.eq.${users[i].id},user_b.eq.${users[i].id}`).in('statut', ['pending', 'accepte']).limit(1);
                if (exA && exA.length > 0) {
                    used.add(users[i].id);
                    continue;
                }
                for (let j = i + 1; j < users.length; j++) {
                    if (used.has(users[j].id))
                        continue;
                    const {data: exB} = await sb.from('matches').select('id').or(`user_a.eq.${users[j].id},user_b.eq.${users[j].id}`).in('statut', ['pending', 'accepte']).limit(1);
                    if (exB && exB.length > 0) {
                        used.add(users[j].id);
                        continue;
                    }
                    // Filtres durs obligatoires
                    if (!hardFiltersPass(users[i], users[j]))
                        continue;
                    const score = compatibilityScore(users[i].reponses, users[j].reponses);
                    if (score >= 70) {
                        await sb.from('matches').insert({
                            user_a: users[i].id,
                            user_b: users[j].id,
                            score,
                            statut: 'pending',
                            created_at: new Date().toISOString()
                        });
                        await sb.from('users').update({
                            statut_match: 'matche'
                        }).eq('id', users[i].id);
                        await sb.from('users').update({
                            statut_match: 'matche'
                        }).eq('id', users[j].id);
                        used.add(users[i].id);
                        used.add(users[j].id);
                        matched++;
                        break;
                    }
                }
            }
            showToast('✓ ' + matched + ' match(s) créé(s)');
            loadAdmin();
        } catch (e) {
            showToast('Erreur matching');
            console.error(e);
        }
    }

    /* ══ PREFERENCES ══ */
    let selectedGenres = [];
    let selectedRoles = [];

    function toggleGenreChip(el, val) {
        if (val === 'tous') {
            // Si on sélectionne "tous", déselectionner les autres
            selectedGenres = ['tous'];
            document.querySelectorAll('#genre-chips .pref-chip').forEach(c => {
                c.classList.toggle('active', c.textContent.toLowerCase() === 'tous');
            });
            return;
        }
        // Déselectionner "tous" si on choisit autre chose
        selectedGenres = selectedGenres.filter(g => g !== 'tous');
        document.querySelector('#genre-chips .pref-chip:last-child').classList.remove('active');

        if (selectedGenres.includes(val)) {
            selectedGenres = selectedGenres.filter(g => g !== val);
            el.classList.remove('active');
        } else {
            selectedGenres.push(val);
            el.classList.add('active');
        }
    }

    function toggleRoleChip(el, val) {
        // Un seul rôle à la fois
        selectedRoles = [val];
        document.querySelectorAll('#role-chips .pref-chip').forEach(c => c.classList.remove('active'));
        el.classList.add('active');
    }

    function updateAgeRange() {
        let min = parseInt(document.getElementById('age-min').value);
        let max = parseInt(document.getElementById('age-max').value);
        if (min > max) {
            // Swap si min dépasse max
            if (event.target.id === 'age-min')
                min = max;
            else
                max = min;
            document.getElementById('age-min').value = min;
            document.getElementById('age-max').value = max;
        }
        document.getElementById('age-range-label').textContent = min + ' – ' + max + ' ans';
    }

    async function savePreferences() {
        if (!st.userId) {
            showToast('Connecte-toi dabord');
            return;
        }
        const min = parseInt(document.getElementById('age-min').value);
        const max = parseInt(document.getElementById('age-max').value);
        const prefs = {
            pref_genres: selectedGenres.length > 0 ? selectedGenres : ['tous'],
            pref_age_min: min,
            pref_age_max: max,
            pref_roles: selectedRoles.length > 0 ? selectedRoles : ['peu importe'],
        };
        const {error} = await sb.from('users').update(prefs).eq('id', st.userId);
        if (error) {
            showToast('Erreur — réessaie');
            return;
        }
        showToast('✓ Préférences sauvegardées !');
    }

    async function loadPreferences() {
        if (!st.userId)
            return;
        let data;
        try {
            const res = await sb.from('users').select('pref_genres,pref_age_min,pref_age_max,pref_roles').eq('id', st.userId).single();
            data = res.data;
        } catch (e) {
            return;
        }
        if (!data)
            return;

        // Genres
        if (data.pref_genres && data.pref_genres.length > 0) {
            selectedGenres = data.pref_genres;
            document.querySelectorAll('#genre-chips .pref-chip').forEach(c => {
                if (selectedGenres.includes(c.textContent.toLowerCase()))
                    c.classList.add('active');
            });
        }
        // Age
        if (data.pref_age_min) {
            document.getElementById('age-min').value = data.pref_age_min;
            document.getElementById('age-max').value = data.pref_age_max || 45;
            updateAgeRange();
        }
        // Roles
        if (data.pref_roles && data.pref_roles.length > 0) {
            selectedRoles = data.pref_roles;
            document.querySelectorAll('#role-chips .pref-chip').forEach(c => {
                if (selectedRoles.includes(c.textContent.toLowerCase()))
                    c.classList.add('active');
            });
        }
    }

    /* ══ MATCHS ══ */
    function generateSlots() {
        const slots = [];
        const days = ['Lundi', 'Mardi', 'Mercredi', 'Jeudi', 'Vendredi', 'Samedi', 'Dimanche'];
        const months = ['jan.', 'fév.', 'mar.', 'avr.', 'mai', 'juin', 'juil.', 'août', 'sep.', 'oct.', 'nov.', 'déc.'];
        const hours = [20, 21];
        let d = new Date();
        d.setDate(d.getDate() + 1);
        let count = 0;
        while (count < 6) {
            const dow = d.getDay();
            const dayName = days[dow === 0 ? 6 : dow - 1];
            for (const h of hours) {
                if (count >= 6)
                    break;
                slots.push({
                    label: `${dayName} ${d.getDate()} ${months[d.getMonth()]} à ${h}h00`,
                    key: `${d.toISOString().slice(0, 10)}-${h}`,
                    date: d.toISOString().slice(0, 10),
                    hour: h
                });
                count++;
            }
            d = new Date(d);
            d.setDate(d.getDate() + 2);
        }
        return slots;
    }

    let currentMatch = null;
    let mySelectedSlots = [];

    async function loadMatchs() {
        const el = document.getElementById('matchs-content');
        if (!st.userId || st.userId === 'undefined') {
            renderNoMatch(el);
            return;
        }

        // Toujours afficher Kino Assistant en premier
        el.innerHTML = '';
        const assistantDone = localStorage.getItem('kino_assistant_done_' + st.userId);
        const assistantCard = document.createElement('div');
        assistantCard.className = 'match-card';
        assistantCard.style.cursor = 'pointer';
        assistantCard.style.marginBottom = '10px';
        if (assistantDone) {
            assistantCard.innerHTML = `
                        <div class="match-card-top">
                            <div class="match-av" style="background:#1E3A2F;color:#F4F0E6;font-size:.75rem;letter-spacing:.04em;">K</div>
                            <div style="flex:1"><div class="match-name">Kino Assistant</div><div style="font-family:'Newsreader',serif;font-size:12px;font-style:italic;color:#9A9080;margin-top:2px;">Onboarding complété</div></div>
                            <div style="font-family:'DM Mono',monospace;font-size:10px;color:#4A9B6F;">✓</div>
                        </div>
                        <div style="font-family:'Newsreader',serif;font-size:13px;font-style:italic;color:#5A4E3A;margin-top:8px;">Tu es prêt. On cherche quelqu’un pour toi.</div>`;
        } else {
            assistantCard.innerHTML = `
                        <div class="match-card-top">
                            <div class="match-av" style="background:#1E3A2F;color:#F4F0E6;font-size:.75rem;letter-spacing:.04em;">K</div>
                            <div style="flex:1"><div class="match-name">Kino Assistant</div><div style="font-family:'Newsreader',serif;font-size:12px;font-style:italic;color:#9A9080;margin-top:2px;">Comprendre le concept</div></div>
                            <div style="font-family:'DM Mono',monospace;font-size:10px;letter-spacing:.06em;text-transform:uppercase;color:#1E3A2F;padding:4px 8px;border:1px solid #C8BEA8;border-radius:2px;">Nouveau</div>
                        </div>
                        <div class="match-bar"><div class="match-bar-fill" style="width:100%;background:#1C1410;"></div></div>
                        <div style="font-family:'Newsreader',serif;font-size:13px;font-style:italic;color:#5A4E3A;line-height:1.5;margin:8px 0 0;">Bienvenue sur Kino. Comprends comment fonctionne ta prochaine rencontre.</div>
                        <div style="padding-top:10px;border-top:1px solid #D8D0BC;margin-top:10px;"><div style="font-family:'DM Mono',monospace;font-size:10px;letter-spacing:.06em;text-transform:uppercase;color:#9A9080;">Appuie pour commencer →</div></div>`;
        }
        assistantCard.onclick = () => openKinoAssistant();
        el.appendChild(assistantCard);

        const {data: matches} = await sb.from('matches')
        .select('id,user_a,user_b,score,statut,reponse_a,reponse_b,slots_a,slots_b,confirmed_slot,chat_state,created_at')
        .or(`user_a.eq.${st.userId},user_b.eq.${st.userId}`)
        .in('statut', ['pending', 'accepte', 'slots_pending', 'confirmed'])
        .order('created_at', {
            ascending: false
        })
        .limit(1);
        if (!matches || matches.length === 0) {
            return;
        } // Kino Assistant already shown above
        for (const m of matches) {
            const isUserA = m.user_a === st.userId;
            const otherId = isUserA ? m.user_b : m.user_a;
            const myReponse = isUserA ? m.reponse_a : m.reponse_b;
            const {data: other} = await sb.from('users').select('prenom,age').eq('id', otherId).single();
            const name = other ? other.prenom : '?';
            const score = m.score || 0;

            // Countdown 24h
            let countdownHTML = '';
            if (m.statut === 'pending' && m.created_at) {
                const created = new Date(m.created_at);
                const expires = new Date(created.getTime() + 24 * 60 * 60 * 1000);
                const remaining = expires - new Date();
                if (remaining > 0) {
                    const h = Math.floor(remaining / 3600000);
                    const min = Math.floor((remaining % 3600000) / 60000);
                    countdownHTML = `<div style="display:flex;align-items:center;gap:8px;padding:8px 10px;background:#F4F0E6;border:1px solid #C8BEA8;border-radius:2px;margin-bottom:10px;">
                                        <div style="width:6px;height:6px;border-radius:50%;background:#1E3A2F;animation:pulse 2s infinite;flex-shrink:0;"></div>
                                        <span style="font-family:'DM Mono',monospace;font-size:10px;letter-spacing:.06em;text-transform:uppercase;color:#1E3A2F;">⏱ ${h}h${String(min).padStart(2, '0')} pour répondre</span>
                                    </div>`;
                }
            }

            let actionHTML = '';
            if (m.statut === 'confirmed') {
                actionHTML = `<div style="display:flex;align-items:center;gap:8px;padding:10px 0 0;border-top:1px solid #D8D0BC;margin-top:10px;">
                                <div style="width:8px;height:8px;border-radius:50%;background:#4A9B6F;flex-shrink:0;"></div>
                                <span style="font-family:'DM Mono',monospace;font-size:10px;letter-spacing:.07em;text-transform:uppercase;color:#4A9B6F;">Rendez-vous confirmé ✓</span>
                            </div>`;
            } else if (m.statut === 'accepte' || m.statut === 'slots_pending') {
                actionHTML = `<div style="padding-top:12px;border-top:1px solid #D8D0BC;margin-top:10px;">
                                <button class="open-chat-btn" data-id="${m.id}" data-name="${name}" data-isusera="${isUserA}" style="width:100%;padding:10px;background:#1E3A2F;border:none;border-radius:50px;font-family:'DM Mono',monospace;font-size:10px;letter-spacing:.06em;text-transform:uppercase;color:#FDF8F4;cursor:pointer;">Organiser la rencontre →</button>
                            </div>`;
            } else if (myReponse === 'accepte') {
                actionHTML = `<div style="padding:10px 0 0;border-top:1px solid #D8D0BC;margin-top:10px;">
                                <span style="font-family:'DM Mono',monospace;font-size:10px;letter-spacing:.07em;text-transform:uppercase;color:#9A9080;">En attente de sa réponse…</span>
                            </div>`;
            } else if (myReponse === 'refuse') {
                actionHTML = `<div style="padding:10px 0 0;border-top:1px solid #D8D0BC;margin-top:10px;">
                                <span style="font-family:'DM Mono',monospace;font-size:10px;letter-spacing:.07em;text-transform:uppercase;color:#C0392B;">Match refusé</span>
                            </div>`;
            } else {
                actionHTML = `<div style="display:flex;flex-direction:column;gap:8px;padding-top:12px;border-top:1px solid #D8D0BC;margin-top:10px;">
                                ${countdownHTML}
                                <div style="display:flex;gap:8px;">
                                    <button class="refuse-btn" data-id="${m.id}" data-isusera="${isUserA}" style="flex:1;padding:10px;background:transparent;border:1px solid #C8BEA8;border-radius:50px;font-family:'DM Mono',monospace;font-size:10px;letter-spacing:.06em;text-transform:uppercase;color:#9A9080;cursor:pointer;">Refuser</button>
                                    <button class="accept-btn" data-id="${m.id}" data-isusera="${isUserA}" style="flex:2;padding:10px;background:#1E3A2F;border:none;border-radius:50px;font-family:'DM Mono',monospace;font-size:10px;letter-spacing:.06em;text-transform:uppercase;color:#FDF8F4;cursor:pointer;">Accepter le date !</button>
                                </div>
                            </div>`;
            }

            const card = document.createElement('div');
            card.className = 'match-card';
            card.style.cursor = 'default';
            card.innerHTML = `
                        <div class="match-card-top">
                            <div class="match-av">${name.charAt(0).toUpperCase()}</div>
                            <div style="flex:1">
                                <div class="match-name">${name}</div>
                                <div style="font-family:'Newsreader',serif;font-size:12px;font-style:italic;color:#9A9080;margin-top:2px;">${other ? other.age + ' ans' : ''}</div>
                            </div>
                            <div class="match-score">${score}<span>%</span></div>
                        </div>
                        <div class="match-bar"><div class="match-bar-fill" style="width:${score}%"></div></div>
                        <div style="font-family:'Newsreader',serif;font-size:13px;font-style:italic;color:#5A4E3A;line-height:1.5;margin:8px 0 0;">
                            Vos réponses sont alignées à <strong style="color:#1A1208;">${score}%</strong>.
                        </div>
                        ${actionHTML}`;
            el.appendChild(card);
        }

        // Event delegation
        el.onclick = function(e) {
            const openBtn = e.target.closest('.open-chat-btn');
            const refuseBtn = e.target.closest('.refuse-btn');
            const acceptBtn = e.target.closest('.accept-btn');
            if (openBtn) {
                openChat(openBtn.dataset.id, openBtn.dataset.name, openBtn.dataset.isusera === 'true');
            }
            if (refuseBtn) {
                respondMatch(refuseBtn.dataset.id, 'refuse', refuseBtn.dataset.isusera === 'true');
            }
            if (acceptBtn) {
                respondMatch(acceptBtn.dataset.id, 'accepte', acceptBtn.dataset.isusera === 'true');
            }
        };
    }

    /* ══ CHAT / SLOTS ══ */
    async function openChat(matchId, matchName, isUserA) {
        currentMatch = {
            id: matchId,
            name: matchName,
            isUserA
        };

        // Update header
        document.getElementById('chat-title').textContent = 'Assistant de ' + matchName;
        document.getElementById('chat-av').textContent = matchName.charAt(0).toUpperCase();

        // Show chat screen
        const chatScreen = document.getElementById('chat-screen');
        chatScreen.style.display = 'flex';

        // Toujours charger depuis Supabase pour avoir l'état le plus récent
        const {data: m} = await sb.from('matches').select('slots_a,slots_b,statut,confirmed_slot').eq('id', matchId).single();

        // Restaurer la sélection précédente depuis la DB
        const mySlots = isUserA ? m.slots_a : m.slots_b;
        mySelectedSlots = (mySlots && mySlots.length > 0) ? [...mySlots] : [];

        renderChat(m, matchName, isUserA);
    }

    function renderChat(matchData, matchName, isUserA) {
        const msgs = document.getElementById('chat-messages');
        msgs.innerHTML = '';
        const slots = generateSlots();
        const state = matchData.chat_state || {};
        const myConfirmed = isUserA ? state.confirmed_a : state.confirmed_b;

        // Bot intro — toujours affiché
        addBubble(msgs, 'bot', `Bonjour ! Je suis l’assistant de ${matchName}. Vous avez tous les deux accepté de vous rencontrer — c’est une bonne nouvelle !`);
        addBubble(msgs, 'bot', `Voici 6 créneaux disponibles dans les deux prochaines semaines. Sélectionne ceux où tu es disponible. Dès qu’un créneau correspond pour vous deux, je vous confirme le rendez-vous.`);

        // Render slots — toujours visibles
        const slotsWrap = document.createElement('div');
        slotsWrap.style.cssText = 'width:100%;margin:8px 0;';
        const otherSlots = isUserA ? matchData.slots_b : matchData.slots_a;

        slots.forEach(slot => {
            const isMine = mySelectedSlots.includes(slot.key);
            const isOther = otherSlots && otherSlots.includes(slot.key);
            const isCommon = isMine && isOther;
            const div = document.createElement('div');
            div.className = 'chat-slot' + (isMine ? ' selected' : '') + (isCommon ? ' matched' : '');
            div.dataset.key = slot.key;
            div.innerHTML = `<span class="slot-label">${slot.label}${isCommon ? ' ✓ Créneau commun !' : isOther ? ' ← Lui aussi' : ''}</span><div class="slot-check">✓</div>`;
            if (matchData.statut !== 'confirmed') {
                div.onclick = () => toggleSlot(div, slot.key, matchData, matchName, isUserA, slots);
            }
            slotsWrap.appendChild(div);
        });
        msgs.appendChild(slotsWrap);

        // Message après confirmation des dispo
        if (myConfirmed) {
            addBubble(msgs, 'bot', 'Tes disponibilités sont enregistrées. Je préviendrai dès que vous avez un créneau en commun.');
            document.getElementById('chat-foot').style.display = 'none';
        } else {
            addBubble(msgs, 'bot', 'Confirme tes disponibilités une fois ta sélection faite.');
            document.getElementById('chat-foot').style.display = 'block';
        }

        // Message de confirmation finale — si rendez-vous trouvé
        if (matchData.statut === 'confirmed' && matchData.confirmed_slot) {
            addBubble(msgs, 'system', `🎉 Bravo ! Vous avez rendez-vous le ${matchData.confirmed_slot}. Vous recevrez l’adresse du rendez-vous 24h avant la rencontre.`);
            document.getElementById('chat-foot').style.display = 'none';
        }

        msgs.scrollTop = msgs.scrollHeight;
    }

    function addBubble(container, type, text) {
        const div = document.createElement('div');
        if (type === 'system') {
            div.className = 'chat-bubble chat-system';
        } else {
            div.className = 'chat-bubble chat-bot';
        }
        div.textContent = text;
        container.appendChild(div);
    }

    async function toggleSlot(el, key, matchData, matchName, isUserA, slots) {
        if (mySelectedSlots.includes(key)) {
            mySelectedSlots = mySelectedSlots.filter(k => k !== key);
            el.classList.remove('selected', 'matched');
        } else {
            mySelectedSlots.push(key);
            el.classList.add('selected');
            const otherSlots = isUserA ? matchData.slots_b : matchData.slots_a;
            if (otherSlots && otherSlots.includes(key)) {
                el.classList.add('matched');
            }
        }
        // Sauvegarder immédiatement en DB à chaque clic
        const matchId = matchData.id || currentMatch.id;
        if (!matchId) {
            console.error('No matchId');
            return;
        }
        const col = isUserA ? 'slots_a' : 'slots_b';
        await sb.from('matches').update({
            [col]: mySelectedSlots
        }).eq('id', matchId);
    }

    async function confirmSlots() {
        if (!currentMatch || mySelectedSlots.length === 0) {
            showToast('Sélectionne au moins un créneau');
            return;
        }
        const col = currentMatch.isUserA ? 'slots_a' : 'slots_b';
        const stateCol = currentMatch.isUserA ? 'confirmed_a' : 'confirmed_b';

        // Récupérer l'état actuel
        const {data: current, error: fetchErr} = await sb.from('matches').select('chat_state,slots_a,slots_b').eq('id', currentMatch.id).single();
        if (fetchErr) {
            showToast('Erreur de connexion');
            console.error(fetchErr);
            return;
        }
        const newState = Object.assign({}, current.chat_state || {}, {
            [stateCol]: true
        });

        await sb.from('matches').update({
            [col]: mySelectedSlots,
            statut: 'slots_pending',
            chat_state: newState
        }).eq('id', currentMatch.id);

        // Vérifier créneau commun
        const slotsA = currentMatch.isUserA ? mySelectedSlots : (current.slots_a || []);
        const slotsB = currentMatch.isUserA ? (current.slots_b || []) : mySelectedSlots;
        const common = slotsA.filter(s => slotsB.includes(s));

        if (common.length > 0) {
            const winner = common[0];
            const slots = generateSlots();
            const slotObj = slots.find(s => s.key === winner);
            const label = slotObj ? slotObj.label : winner;
            await sb.from('matches').update({
                statut: 'confirmed',
                confirmed_slot: label
            }).eq('id', currentMatch.id);
            haptic('success');
            showToast('Rendez-vous confirmé !');
        } else {
            showToast('Disponibilités enregistrées !');
        }

        // Recharger depuis DB pour afficher l'état complet
        const {data: updated} = await sb.from('matches').select('*').eq('id', currentMatch.id).single();
        const mySlots = currentMatch.isUserA ? updated.slots_a : updated.slots_b;
        mySelectedSlots = mySlots || [];
        renderChat(updated, currentMatch.name, currentMatch.isUserA);
        loadMatchs();
    }

    function closeChat() {
        document.getElementById('chat-screen').style.display = 'none';
        loadMatchs();
    }

    async function respondMatch(matchId, reponse, isUserA) {
        const col = isUserA ? 'reponse_a' : 'reponse_b';
        const update = {
            [col]: reponse
        };
        if (reponse === 'refuse')
            update.statut = 'refuse';
        const {data: match} = await sb.from('matches').update(update).eq('id', matchId).select().single();
        if (reponse === 'accepte' && match) {
            const autreReponse = isUserA ? match.reponse_b : match.reponse_a;
            if (autreReponse === 'accepte') {
                await sb.from('matches').update({
                    statut: 'accepte'
                }).eq('id', matchId);
                haptic('success');
                showToast('Match accepté des deux côtés !');
                setTimeout(() => loadMatchs(), 500);
                return;
            }
        }
        if (reponse === 'refuse') {
            const {data: m} = await sb.from('matches').select('user_a,user_b').eq('id', matchId).single();
            if (m) {
                await sb.from('users').update({
                    statut_match: 'en_attente'
                }).eq('id', m.user_a);
                await sb.from('users').update({
                    statut_match: 'en_attente'
                }).eq('id', m.user_b);
            }
            showToast('Match refusé — tu seras remis en matching.');
        } else {
            showToast('Super ! On attend sa réponse.');
        }
        setTimeout(() => loadMatchs(), 500);
    }

    function renderNoMatch(el) {
        // Toujours afficher Kino Assistant comme premier "match"
        el.innerHTML = '';
        const card = document.createElement('div');
        card.className = 'match-card';
        card.style.cursor = 'pointer';
        card.innerHTML = `
                <div class="match-card-top">
                    <div class="match-av" style="background:#1E3A2F;color:#F4F0E6;font-size:.75rem;letter-spacing:.04em;">K</div>
                    <div style="flex:1">
                        <div class="match-name">Kino Assistant</div>
                        <div style="font-family:'Newsreader',serif;font-size:12px;font-style:italic;color:#9A9080;margin-top:2px;">Comprendre le concept</div>
                    </div>
                    <div style="font-family:'DM Mono',monospace;font-size:10px;letter-spacing:.06em;text-transform:uppercase;color:#1E3A2F;padding:4px 8px;border:1px solid #C8BEA8;border-radius:2px;">Nouveau</div>
                </div>
                <div class="match-bar"><div class="match-bar-fill" style="width:100%;background:#1C1410;"></div></div>
                <div style="font-family:'Newsreader',serif;font-size:13px;font-style:italic;color:#5A4E3A;line-height:1.5;margin:8px 0 0;">
                    Bienvenue sur Kino. Comprends comment fonctionne ta prochaine rencontre.
                </div>
                <div style="padding-top:12px;border-top:1px solid #D8D0BC;margin-top:10px;">
                    <div style="font-family:'DM Mono',monospace;font-size:10px;letter-spacing:.06em;text-transform:uppercase;color:#9A9080;">Appuie pour commencer →</div>
                </div>`;
        card.onclick = () => openKinoAssistant();
        el.appendChild(card);
    }

    function compatibilityScore(repA, repB) {
        if (!repA || !repB || repA.length === 0)
            return 0;
        const common = repA.filter(a => {
            const b = repB.find(r => r.card_index === a.card_index);
            return b && b.vote === a.vote;
        });
        return Math.round((common.length / repA.length) * 100);
    }

    function hardFiltersPass(userA, userB) {
        const genresA = userA.pref_genres || ['tous'];
        const genresB = userB.pref_genres || ['tous'];
        const genreOK = (genres, genre) => !genres || genres.includes('tous') || genres.includes(genre);
        if (!genreOK(genresA, userB.genre))
            return false;
        if (!genreOK(genresB, userA.genre))
            return false;
        const minA = userA.pref_age_min || 18,
            maxA = userA.pref_age_max || 99;
        const minB = userB.pref_age_min || 18,
            maxB = userB.pref_age_max || 99;
        if (userB.age < minA || userB.age > maxA)
            return false;
        if (userA.age < minB || userA.age > maxB)
            return false;
        const rolesA = userA.pref_roles || ['peu importe'];
        const rolesB = userB.pref_roles || ['peu importe'];
        if (rolesA.includes('peu importe') || rolesB.includes('peu importe'))
            return true;
        if (rolesA.includes('versatile') || rolesB.includes('versatile'))
            return true;
        if (rolesA.includes('actif') && rolesB.includes('passif'))
            return true;
        if (rolesA.includes('passif') && rolesB.includes('actif'))
            return true;
        return false;
    }

    async function runMatching() {
        showToast('Analyse en cours…', 5000);
        try {
            const {data: users} = await sb.from('users').select('*').eq('statut_match', 'en_attente').order('created_at');
            if (!users || users.length < 2) {
                showToast('Pas assez de profils');
                return;
            }
            let matched = 0;
            const used = new Set();
            for (let i = 0; i < users.length; i++) {
                if (used.has(users[i].id))
                    continue;
                const {data: exA} = await sb.from('matches').select('id').or(`user_a.eq.${users[i].id},user_b.eq.${users[i].id}`).in('statut', ['pending', 'accepte']).limit(1);
                if (exA && exA.length > 0) {
                    used.add(users[i].id);
                    continue;
                }
                for (let j = i + 1; j < users.length; j++) {
                    if (used.has(users[j].id))
                        continue;
                    const {data: exB} = await sb.from('matches').select('id').or(`user_a.eq.${users[j].id},user_b.eq.${users[j].id}`).in('statut', ['pending', 'accepte']).limit(1);
                    if (exB && exB.length > 0) {
                        used.add(users[j].id);
                        continue;
                    }
                    if (!hardFiltersPass(users[i], users[j]))
                        continue;
                    const score = compatibilityScore(users[i].reponses, users[j].reponses);
                    if (score >= 70) {
                        await sb.from('matches').insert({
                            user_a: users[i].id,
                            user_b: users[j].id,
                            score,
                            statut: 'pending',
                            created_at: new Date().toISOString()
                        });
                        await sb.from('users').update({
                            statut_match: 'matche'
                        }).eq('id', users[i].id);
                        await sb.from('users').update({
                            statut_match: 'matche'
                        }).eq('id', users[j].id);
                        used.add(users[i].id);
                        used.add(users[j].id);
                        matched++;
                        break;
                    }
                }
            }
            showToast('✓ ' + matched + ' match(s) créé(s)');
            loadAdmin();
        } catch (e) {
            showToast('Erreur matching');
            console.error(e);
        }
    }

    /* ══ KINO ASSISTANT ══ */
    const KINO_SCRIPT = [
    {
        type: 'bot',
        text: `Bonjour et bienvenue sur Kino. Je suis ton assistant personnel. Je vais t’expliquer comment fonctionne l’app en quelques minutes.`
    },
    {
        type: 'bot',
        text: `Kino, c’est simple : tu réponds à des flash cards de personnalité. On trouve quelqu’un compatible à au moins 70%. Et on vous propose un rendez-vous dans un bar ou un café à Paris.`
    },
    {
        type: 'question',
        text: `Tu comprends que le rendez-vous se passe en vrai, dans un lieu que Kino choisit pour vous — un café ou un bar à Paris ?`,
        answers: ['Oui, j’ai compris', 'Dis-m’en plus'],
        next: [3, 2]
    },
    {
        type: 'bot',
        text: `Le lieu est choisi selon vos réponses communes. Tu reçois l’adresse exacte 24h avant le rendez-vous. Pas de surprise désagréable — juste un endroit qui vous correspond.`
    },
    {
        type: 'bot',
        text: `Importante précision : il n’y a aucune photo avant le match. Aucune. Tu découvres la personne au rendez-vous. C’est ça, le concept Kino.`
    },
    {
        type: 'question',
        text: `Tu t’engages à te présenter au rendez-vous si tu acceptes un match ?`,
        answers: ['Oui, je m’engage', 'Et si je peux pas venir ?'],
        next: [6, 5]
    },
    {
        type: 'bot',
        text: `Pas de souci — si tu ne peux plus venir, tu peux annuler jusqu’à 24h avant. Au-delà, ton profil sera suspendu temporairement par respect pour l’autre personne.`
    },
    {
        type: 'bot',
        text: `Notre méthodologie : on compare tes réponses aux flash cards avec celles des autres membres. Si vous avez répondu pareil à au moins 70% des questions, c’est un match potentiel.`
    },
    {
        type: 'bot',
        text: `Et si personne ne correspond à tes critères ? On ne te propose rien. On préfère ne pas matcher plutôt que de forcer une rencontre qui ne tient pas la route.`
    },
    {
        type: 'question',
        text: `Des questions sur le fonctionnement ?`,
        answers: ['Non, je suis prêt !', 'Comment sont choisis les lieux ?'],
        next: [10, 9]
    },
    {
        type: 'bot',
        text: `Les lieux sont sélectionnés par l’équipe Kino — bars et cafés parisiens chaleureux, ni trop formels ni trop bruyants. Des endroits où on peut vraiment se parler.`
    },
    {
        type: 'done',
        text: `Parfait. Tu es prêt. On analyse tes réponses aux flash cards et on cherche quelqu’un pour toi. Bonne rencontre. 🌿`
    }
    ];

    let kinoStep = 0;
    let kinoAnswered = [];

    function openKinoAssistant() {
        currentMatch = null;
        kinoStep = 0;
        kinoAnswered = [];

        document.getElementById('chat-title').textContent = 'Kino Assistant';
        document.getElementById('chat-av').textContent = 'K';
        document.getElementById('chat-av').style.background = '#1C1410';
        document.getElementById('chat-foot').style.display = 'none';

        const chatScreen = document.getElementById('chat-screen');
        chatScreen.style.display = 'flex';

        const msgs = document.getElementById('chat-messages');
        msgs.innerHTML = '';

        playKinoStep(0);
    }

    async function playKinoStep(stepIdx) {
        if (stepIdx >= KINO_SCRIPT.length)
            return;
        const step = KINO_SCRIPT[stepIdx];
        const msgs = document.getElementById('chat-messages');

        if (step.type === 'bot') {
            // Petit délai pour effet naturel
            await new Promise(r => setTimeout(r, stepIdx === 0 ? 300 : 600));
            addBubble(msgs, 'bot', step.text);
            msgs.scrollTop = msgs.scrollHeight;
            // Passer automatiquement au suivant
            setTimeout(() => playKinoStep(stepIdx + 1), 800);

        } else if (step.type === 'question') {
            await new Promise(r => setTimeout(r, 700));
            addBubble(msgs, 'bot', step.text);

            // Afficher les boutons de réponse
            const btnWrap = document.createElement('div');
            btnWrap.style.cssText = 'display:flex;flex-direction:column;gap:6px;margin:8px 0 4px;';
            step.answers.forEach((ans, i) => {
                const btn = document.createElement('button');
                btn.style.cssText = `padding:10px 14px;background:${i === 0 ? '#E8622A' : 'transparent'};border:1px solid ${i === 0 ? '#E8622A' : '#C8BEA8'};border-radius:4px;font-family:'Newsreader',serif;font-size:13px;font-style:italic;color:${i === 0 ? '#FDF8F4' : '#7A5A48'};cursor:pointer;text-align:left;transition:all .2s;`;
                btn.textContent = ans;
                btn.onclick = () => {
                    // Montrer la réponse choisie
                    btnWrap.innerHTML = `<div style="font-family:'Newsreader',serif;font-size:13px;font-style:italic;color:#9A9080;padding:4px 0;">→ ${ans}</div>`;
                    setTimeout(() => playKinoStep(step.next[i]), 400);
                };
                btnWrap.appendChild(btn);
            });
            msgs.appendChild(btnWrap);
            msgs.scrollTop = msgs.scrollHeight;

        } else if (step.type === 'done') {
            await new Promise(r => setTimeout(r, 600));
            addBubble(msgs, 'bot', step.text);
            // Marquer comme complété
            if (st.userId)
                localStorage.setItem('kino_assistant_done_' + st.userId, '1');
            msgs.scrollTop = msgs.scrollHeight;
            // Bouton fermer
            setTimeout(() => {
                const foot = document.getElementById('chat-foot');
                foot.innerHTML = `<button onclick="closeChat()" style="width:100%;padding:14px;background:#1E3A2F;border:none;border-radius:50px;font-family:'Syne',sans-serif;font-weight:700;font-size:12px;letter-spacing:.06em;text-transform:uppercase;color:#FDF8F4;cursor:pointer;">C’est parti ✓</button>`;
                foot.style.display = 'block';
            }, 600);
        }
    }

    /* ══ HAPTIC FEEDBACK ══ */
    function haptic(type) {
        // Vibration API (Android + WebView)
        if (navigator.vibrate) {
            if (type === 'light')
                navigator.vibrate(10);
            else if (type === 'medium')
                navigator.vibrate(20);
            else if (type === 'success')
                navigator.vibrate([10, 30, 10]);
        }
        // iOS Taptic Engine via Median/GoNative bridge
        if (window.webkit && window.webkit.messageHandlers && window.webkit.messageHandlers.haptic) {
            window.webkit.messageHandlers.haptic.postMessage(type);
        }
    }

    /* ══ INIT ══ */
    function hideLoading() {}

    (async function init() {
        // La home est déjà active par défaut
        // On essaie de récupérer la session en arrière-plan
        try {
            const {data: {session}} = await Promise.race([
            sb.auth.getSession(),
            new Promise((_, reject) => setTimeout(() => reject(new Error('timeout')), 4000))
            ]);

            if (session && session.user) {
                st.authUser = session.user;
                st.email = session.user.email;
                try {
                    await loadExistingProfile();
                } catch (e) {
                    console.error('Profile load error:', e);
                }
            } else {
                try {
                    const {data} = await sb.from('users').select('id');
                    if (data && data.length > 0)
                        document.getElementById('user-count').textContent = 'Kino · ' + data.length + ' inscrits';
                } catch (e) {}
            }
        } catch (e) {
            console.error('Session error:', e);

        }
        // La home est déjà visible, rien à faire

        // Écouter les retours OTP
        sb.auth.onAuthStateChange(async (event, session) => {
            if (event === 'SIGNED_IN' && session && !st.authUser) {
                st.authUser = session.user;
                st.email = session.user.email;
                try {
                    await loadExistingProfile();
                } catch (e) {
                    console.error(e);
                }
            }
        });
    })();
    </script>
</body>
</html>
