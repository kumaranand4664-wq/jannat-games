<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=yes" />
    <title>🎰 Jannat Games – Premium Casino</title>

    <!-- ============================================================ -->
    <!-- STYLES – Premium UI with Smooth Animations                    -->
    <!-- ============================================================ -->
    <style>
        /* ---------- RESET & BASE ---------- */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        :root {
            --gold: #f7e05e;
            --gold-dim: #c9a84c;
            --gold-glow: rgba(201, 168, 76, 0.35);
            --dark-bg: #0d0505;
            --card-bg: rgba(20, 12, 12, 0.72);
            --glass-border: rgba(255, 255, 255, 0.06);
            --text-primary: #f0e6d3;
            --text-muted: rgba(255, 255, 255, 0.35);
            --radius-lg: 28px;
            --radius-md: 16px;
            --radius-sm: 40px;
            --shadow-heavy: 0 20px 60px rgba(0, 0, 0, 0.8);
            --transition-smooth: all 0.35s cubic-bezier(0.25, 0.46, 0.45, 0.94);
        }

        html {
            scroll-behavior: smooth;
            -webkit-tap-highlight-color: transparent;
        }

        body {
            font-family: 'Segoe UI', system-ui, -apple-system, BlinkMacSystemFont, sans-serif;
            background: var(--dark-bg);
            min-height: 100vh;
            color: var(--text-primary);
            padding: 16px;
            display: flex;
            flex-direction: column;
            align-items: center;
            background-image:
                radial-gradient(ellipse at 20% 50%, rgba(201, 168, 76, 0.06) 0%, transparent 60%),
                radial-gradient(ellipse at 80% 20%, rgba(201, 168, 76, 0.04) 0%, transparent 50%),
                radial-gradient(ellipse at 50% 100%, rgba(201, 168, 76, 0.03) 0%, transparent 40%);
            background-attachment: fixed;
            position: relative;
            overflow-x: hidden;
        }

        /* Animated background particles */
        body::before {
            content: '';
            position: fixed;
            inset: 0;
            z-index: 0;
            pointer-events: none;
            background-image:
                radial-gradient(2px 2px at 20% 30%, rgba(255, 215, 0, 0.15), transparent),
                radial-gradient(2px 2px at 40% 70%, rgba(255, 215, 0, 0.10), transparent),
                radial-gradient(2px 2px at 60% 20%, rgba(255, 215, 0, 0.12), transparent),
                radial-gradient(2px 2px at 80% 80%, rgba(255, 215, 0, 0.08), transparent),
                radial-gradient(1px 1px at 10% 90%, rgba(255, 215, 0, 0.20), transparent),
                radial-gradient(1px 1px at 90% 10%, rgba(255, 215, 0, 0.18), transparent),
                radial-gradient(1px 1px at 50% 50%, rgba(255, 215, 0, 0.06), transparent);
            background-size: 200px 200px;
            animation: particleDrift 60s linear infinite;
        }

        @keyframes particleDrift {
            0% {
                transform: translate(0, 0) scale(1);
            }
            33% {
                transform: translate(30px, -20px) scale(1.02);
            }
            66% {
                transform: translate(-20px, 30px) scale(0.98);
            }
            100% {
                transform: translate(0, 0) scale(1);
            }
        }

        /* Floating orbs */
        .orb {
            position: fixed;
            border-radius: 50%;
            filter: blur(80px);
            pointer-events: none;
            z-index: 0;
            opacity: 0.3;
            animation: orbFloat 18s ease-in-out infinite alternate;
        }
        .orb-1 {
            width: 400px;
            height: 400px;
            background: radial-gradient(circle, rgba(201, 168, 76, 0.15), transparent 70%);
            top: -100px;
            right: -100px;
            animation-duration: 22s;
        }
        .orb-2 {
            width: 350px;
            height: 350px;
            background: radial-gradient(circle, rgba(180, 80, 200, 0.08), transparent 70%);
            bottom: -80px;
            left: -80px;
            animation-duration: 26s;
            animation-delay: -8s;
        }
        .orb-3 {
            width: 200px;
            height: 200px;
            background: radial-gradient(circle, rgba(255, 215, 0, 0.10), transparent 70%);
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            animation-duration: 30s;
            animation-delay: -4s;
        }

        @keyframes orbFloat {
            0% {
                transform: translate(0, 0) scale(1);
            }
            33% {
                transform: translate(40px, -30px) scale(1.1);
            }
            66% {
                transform: translate(-30px, 40px) scale(0.9);
            }
            100% {
                transform: translate(20px, -10px) scale(1.05);
            }
        }

        /* ---------- SCROLLBAR ---------- */
        ::-webkit-scrollbar {
            width: 5px;
            height: 5px;
        }
        ::-webkit-scrollbar-track {
            background: rgba(0, 0, 0, 0.3);
            border-radius: 10px;
        }
        ::-webkit-scrollbar-thumb {
            background: var(--gold-dim);
            border-radius: 10px;
            box-shadow: 0 0 20px var(--gold-glow);
        }

        /* ---------- MAIN CONTAINER ---------- */
        .container {
            max-width: 1140px;
            width: 100%;
            background: var(--card-bg);
            backdrop-filter: blur(20px) saturate(1.2);
            -webkit-backdrop-filter: blur(20px) saturate(1.2);
            border: 1px solid var(--glass-border);
            border-radius: var(--radius-lg);
            padding: 24px 28px 20px;
            box-shadow: var(--shadow-heavy), inset 0 1px 0 rgba(255, 255, 255, 0.03);
            position: relative;
            z-index: 1;
            transition: var(--transition-smooth);
        }

        .container::after {
            content: '';
            position: absolute;
            inset: -1px;
            border-radius: var(--radius-lg);
            padding: 1px;
            background: linear-gradient(135deg, rgba(201, 168, 76, 0.15), transparent 40%, transparent 60%, rgba(201, 168, 76, 0.08));
            -webkit-mask: linear-gradient(#fff 0 0) content-box, linear-gradient(#fff 0 0);
            mask: linear-gradient(#fff 0 0) content-box, linear-gradient(#fff 0 0);
            -webkit-mask-composite: xor;
            mask-composite: exclude;
            pointer-events: none;
        }

        /* ---------- HEADER ---------- */
        .header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            flex-wrap: wrap;
            gap: 12px 18px;
            margin-bottom: 20px;
            position: relative;
            z-index: 2;
        }

        .logo {
            display: flex;
            align-items: center;
            gap: 10px;
            font-size: clamp(22px, 4vw, 32px);
            font-weight: 800;
            letter-spacing: 0.5px;
            background: linear-gradient(135deg, #f7e05e, #c9a84c, #f7e05e);
            background-size: 200% 200%;
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            animation: shimmerLogo 4s ease-in-out infinite;
            text-shadow: 0 0 60px rgba(201, 168, 76, 0.15);
            transition: var(--transition-smooth);
        }
        .logo span {
            font-size: clamp(28px, 4.5vw, 38px);
            -webkit-text-fill-color: initial;
            animation: none;
        }
        @keyframes shimmerLogo {
            0%,
            100% {
                background-position: 0% 50%;
            }
            50% {
                background-position: 100% 50%;
            }
        }

        .header-actions {
            display: flex;
            align-items: center;
            gap: 10px;
            flex-wrap: wrap;
        }

        .balance-wrap {
            display: flex;
            align-items: center;
            gap: 14px;
            background: rgba(0, 0, 0, 0.45);
            padding: 6px 16px 6px 20px;
            border-radius: 60px;
            border: 1px solid rgba(201, 168, 76, 0.15);
            backdrop-filter: blur(8px);
            transition: var(--transition-smooth);
        }
        .balance-wrap:hover {
            border-color: rgba(201, 168, 76, 0.3);
            box-shadow: 0 0 30px rgba(201, 168, 76, 0.04);
        }
        .balance-label {
            font-size: 11px;
            text-transform: uppercase;
            letter-spacing: 2px;
            opacity: 0.5;
            font-weight: 600;
        }
        .balance-amount {
            font-size: clamp(18px, 2.8vw, 26px);
            font-weight: 700;
            color: var(--gold);
            min-width: 70px;
            text-align: right;
            transition: var(--transition-smooth);
        }
        .balance-amount.pulse {
            animation: balancePulse 0.4s ease;
        }
        @keyframes balancePulse {
            0%,
            100% {
                transform: scale(1);
            }
            50% {
                transform: scale(1.12);
                color: #fff;
            }
        }

        .btn-outline {
            background: rgba(201, 168, 76, 0.06);
            border: 1px solid rgba(201, 168, 76, 0.18);
            color: var(--gold-dim);
            padding: 6px 16px;
            border-radius: 60px;
            cursor: pointer;
            font-weight: 600;
            font-size: 13px;
            transition: var(--transition-smooth);
            display: flex;
            align-items: center;
            gap: 6px;
            white-space: nowrap;
            backdrop-filter: blur(4px);
        }
        .btn-outline:hover {
            background: rgba(201, 168, 76, 0.14);
            border-color: var(--gold-dim);
            transform: translateY(-1px) scale(1.03);
            box-shadow: 0 8px 30px rgba(201, 168, 76, 0.08);
        }
        .btn-outline:active {
            transform: scale(0.96);
        }
        .btn-outline.wallet {
            border-color: rgba(76, 175, 80, 0.3);
            color: #8bc34a;
        }
        .btn-outline.wallet:hover {
            background: rgba(76, 175, 80, 0.12);
            border-color: #8bc34a;
            box-shadow: 0 8px 30px rgba(76, 175, 80, 0.08);
        }
        .btn-reset {
            background: rgba(255, 255, 255, 0.04);
            border: 1px solid rgba(255, 255, 255, 0.06);
            color: rgba(255, 255, 255, 0.35);
            padding: 6px 14px;
            border-radius: 60px;
            cursor: pointer;
            font-weight: 600;
            font-size: 12px;
            transition: var(--transition-smooth);
        }
        .btn-reset:hover {
            background: rgba(255, 255, 255, 0.08);
            color: var(--text-primary);
            transform: rotate(-8deg) scale(1.04);
        }

        /* ---------- TABS ---------- */
        .tabs {
            display: flex;
            gap: 4px;
            margin-bottom: 22px;
            position: relative;
            z-index: 2;
            flex-wrap: wrap;
            background: rgba(0, 0, 0, 0.2);
            border-radius: 60px;
            padding: 4px;
            border: 1px solid rgba(255, 255, 255, 0.03);
        }
        .tab-btn {
            background: transparent;
            border: none;
            color: rgba(255, 255, 255, 0.4);
            padding: 8px 20px;
            font-size: clamp(13px, 1.4vw, 16px);
            font-weight: 600;
            cursor: pointer;
            border-radius: 40px;
            transition: var(--transition-smooth);
            position: relative;
            letter-spacing: 0.3px;
            flex: 1 0 auto;
            text-align: center;
            min-width: 60px;
        }
        .tab-btn:hover {
            color: rgba(255, 255, 255, 0.7);
            background: rgba(255, 255, 255, 0.04);
        }
        .tab-btn.active {
            color: #1a0a0a;
            background: linear-gradient(135deg, var(--gold), var(--gold-dim));
            box-shadow: 0 4px 20px rgba(201, 168, 76, 0.25);
            transform: scale(1.02);
        }
        .tab-btn.active:hover {
            transform: scale(1.04);
        }

        /* ---------- GAME PANELS ---------- */
        .game-panel {
            display: none;
            animation: panelSlide 0.45s cubic-bezier(0.25, 0.46, 0.45, 0.94) forwards;
            position: relative;
            z-index: 2;
        }
        .game-panel.active {
            display: block;
        }

        @keyframes panelSlide {
            0% {
                opacity: 0;
                transform: translateY(18px) scale(0.98);
            }
            100% {
                opacity: 1;
                transform: translateY(0) scale(1);
            }
        }

        /* ---------- GAME CARDS (for arcade) ---------- */
        .arcade-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(140px, 1fr));
            gap: 14px;
            margin: 8px 0 4px;
        }

        .game-card {
            background: rgba(255, 255, 255, 0.03);
            border: 1px solid rgba(255, 255, 255, 0.05);
            border-radius: var(--radius-md);
            padding: 18px 10px 14px;
            text-align: center;
            cursor: pointer;
            transition: var(--transition-smooth);
            display: flex;
            flex-direction: column;
            align-items: center;
            gap: 4px;
            backdrop-filter: blur(4px);
            position: relative;
            overflow: hidden;
        }
        .game-card::before {
            content: '';
            position: absolute;
            inset: 0;
            background: radial-gradient(circle at 50% 0%, rgba(201, 168, 76, 0.06), transparent 70%);
            opacity: 0;
            transition: var(--transition-smooth);
        }
        .game-card:hover {
            transform: translateY(-6px) scale(1.02);
            border-color: rgba(201, 168, 76, 0.2);
            box-shadow: 0 12px 40px rgba(0, 0, 0, 0.4);
            background: rgba(255, 255, 255, 0.06);
        }
        .game-card:hover::before {
            opacity: 1;
        }
        .game-card:active {
            transform: scale(0.95);
        }
        .game-card .icon {
            font-size: clamp(32px, 5vw, 44px);
            transition: var(--transition-smooth);
        }
        .game-card:hover .icon {
            transform: scale(1.12) rotate(-4deg);
        }
        .game-card .name {
            font-weight: 700;
            font-size: clamp(12px, 1.2vw, 15px);
            color: var(--text-primary);
            margin-top: 2px;
        }
        .game-card .desc {
            font-size: 10px;
            opacity: 0.35;
            letter-spacing: 0.3px;
        }

        /* ---------- GAME VIEW (arcade) ---------- */
        .game-view {
            display: none;
            flex-direction: column;
            align-items: center;
            gap: 14px;
            padding: 6px 0 10px;
            animation: panelSlide 0.4s ease;
        }
        .game-view.active {
            display: flex;
        }

        .game-view .back-btn {
            align-self: flex-start;
            background: rgba(255, 255, 255, 0.04);
            border: 1px solid rgba(255, 255, 255, 0.06);
            color: var(--gold-dim);
            padding: 5px 16px;
            border-radius: 60px;
            cursor: pointer;
            font-size: 13px;
            font-weight: 600;
            transition: var(--transition-smooth);
            display: flex;
            align-items: center;
            gap: 6px;
        }
        .game-view .back-btn:hover {
            background: rgba(201, 168, 76, 0.10);
            transform: translateX(-4px);
        }
        .game-view .game-title {
            font-size: clamp(22px, 3vw, 30px);
            font-weight: 800;
            color: var(--gold);
            text-shadow: 0 0 40px rgba(201, 168, 76, 0.08);
        }
        .game-view .game-area {
            display: flex;
            flex-direction: column;
            align-items: center;
            gap: 14px;
            width: 100%;
            max-width: 420px;
        }
        .game-view .bet-ctrl {
            display: flex;
            align-items: center;
            gap: 12px;
            flex-wrap: wrap;
            justify-content: center;
            width: 100%;
        }
        .game-view .bet-ctrl label {
            font-size: 13px;
            opacity: 0.6;
            font-weight: 600;
        }
        .game-view .bet-ctrl input {
            background: rgba(0, 0, 0, 0.4);
            border: 1px solid rgba(255, 255, 255, 0.08);
            border-radius: 60px;
            padding: 8px 16px;
            color: var(--gold);
            font-size: 18px;
            font-weight: 700;
            width: 100px;
            text-align: center;
            outline: none;
            transition: var(--transition-smooth);
        }
        .game-view .bet-ctrl input:focus {
            border-color: var(--gold-dim);
            box-shadow: 0 0 30px rgba(201, 168, 76, 0.05);
        }
        .game-view .options {
            display: flex;
            gap: 8px;
            flex-wrap: wrap;
            justify-content: center;
            width: 100%;
        }
        .game-view .options button {
            background: rgba(255, 255, 255, 0.04);
            border: 1px solid rgba(255, 255, 255, 0.06);
            color: var(--text-primary);
            padding: 7px 16px;
            border-radius: 60px;
            cursor: pointer;
            font-weight: 600;
            transition: var(--transition-smooth);
            font-size: 14px;
            flex: 0 1 auto;
            min-width: 44px;
        }
        .game-view .options button:hover:not(.selected) {
            background: rgba(255, 255, 255, 0.08);
            border-color: rgba(255, 255, 255, 0.12);
            transform: translateY(-1px);
        }
        .game-view .options button.selected {
            background: rgba(201, 168, 76, 0.18);
            border-color: var(--gold-dim);
            color: var(--gold);
            box-shadow: 0 0 30px rgba(201, 168, 76, 0.06);
            transform: scale(1.04);
        }
        .game-view .options button:active {
            transform: scale(0.94);
        }

        .game-view .play-btn {
            background: linear-gradient(135deg, var(--gold), var(--gold-dim));
            border: none;
            color: #1a0a0a;
            font-weight: 800;
            font-size: clamp(18px, 2vw, 22px);
            padding: 10px 44px;
            border-radius: 60px;
            cursor: pointer;
            transition: var(--transition-smooth);
            box-shadow: 0 4px 30px rgba(201, 168, 76, 0.2);
            position: relative;
            overflow: hidden;
        }
        .game-view .play-btn::after {
            content: '';
            position: absolute;
            inset: 0;
            background: linear-gradient(135deg, transparent 30%, rgba(255, 255, 255, 0.15) 50%, transparent 70%);
            transform: translateX(-100%);
            transition: transform 0.6s ease;
        }
        .game-view .play-btn:hover:not(:disabled)::after {
            transform: translateX(100%);
        }
        .game-view .play-btn:hover:not(:disabled) {
            transform: scale(1.04);
            box-shadow: 0 8px 40px rgba(201, 168, 76, 0.35);
        }
        .game-view .play-btn:active:not(:disabled) {
            transform: scale(0.96);
        }
        .game-view .play-btn:disabled {
            opacity: 0.35;
            cursor: not-allowed;
            transform: none;
        }

        .game-view .result {
            font-size: clamp(16px, 1.6vw, 20px);
            font-weight: 600;
            min-height: 34px;
            color: var(--gold);
            text-align: center;
            padding: 4px 12px;
            border-radius: 40px;
            background: rgba(0, 0, 0, 0.2);
            backdrop-filter: blur(4px);
            width: 100%;
            transition: var(--transition-smooth);
        }
        .game-view .result .highlight {
            font-size: clamp(26px, 3vw, 34px);
            display: inline-block;
            animation: resultPop 0.5s cubic-bezier(0.34, 1.56, 0.64, 1);
        }
        @keyframes resultPop {
            0% {
                transform: scale(0.5);
                opacity: 0;
            }
            100% {
                transform: scale(1);
                opacity: 1;
            }
        }

        .game-view .history {
            font-size: 13px;
            opacity: 0.4;
            max-height: 52px;
            overflow-y: auto;
            width: 100%;
            text-align: center;
            padding: 4px 8px;
            background: rgba(0, 0, 0, 0.15);
            border-radius: 40px;
            letter-spacing: 0.3px;
        }

        /* ---------- SLOTS ---------- */
        .slots-container {
            text-align: center;
        }
        .reels {
            display: flex;
            justify-content: center;
            gap: clamp(10px, 2vw, 22px);
            margin: 14px 0 20px;
            perspective: 900px;
        }
        .reel {
            width: clamp(70px, 12vw, 120px);
            height: clamp(88px, 14vw, 140px);
            background: radial-gradient(ellipse at center, #2a1a1a, #0f0707);
            border: 2px solid rgba(201, 168, 76, 0.25);
            border-radius: var(--radius-md);
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            font-size: clamp(38px, 7vw, 64px);
            box-shadow: inset 0 0 60px rgba(0, 0, 0, 0.6), 0 8px 40px rgba(0, 0, 0, 0.5);
            transition: border-color 0.3s, box-shadow 0.3s;
            position: relative;
            overflow: hidden;
            user-select: none;
        }
        .reel::after {
            content: '';
            position: absolute;
            inset: 0;
            background: linear-gradient(180deg, rgba(0, 0, 0, 0.5) 0%, transparent 30%, transparent 70%, rgba(0, 0, 0, 0.5) 100%);
            pointer-events: none;
        }
        .reel .symbol {
            transition: transform 0.1s;
            font-size: clamp(42px, 7vw, 68px);
            line-height: 1;
            z-index: 1;
        }
        .reel.spinning {
            border-color: var(--gold);
            box-shadow: 0 0 50px rgba(201, 168, 76, 0.15), inset 0 0 60px rgba(0, 0, 0, 0.6);
            animation: reelShake 0.08s steps(1) infinite;
        }
        @keyframes reelShake {
            0% {
                transform: translateY(0) rotate(0deg);
            }
            25% {
                transform: translateY(-4px) rotate(0.5deg);
            }
            50% {
                transform: translateY(2px) rotate(-0.5deg);
            }
            75% {
                transform: translateY(-2px) rotate(0.3deg);
            }
            100% {
                transform: translateY(0) rotate(0deg);
            }
        }

        .slots-controls {
            display: flex;
            justify-content: center;
            align-items: center;
            gap: 16px;
            flex-wrap: wrap;
            margin-top: 4px;
        }
        .bet-input-wrap {
            display: flex;
            align-items: center;
            gap: 8px;
            background: rgba(0, 0, 0, 0.35);
            padding: 4px 14px 4px 18px;
            border-radius: 60px;
            border: 1px solid rgba(201, 168, 76, 0.08);
            backdrop-filter: blur(4px);
            transition: var(--transition-smooth);
        }
        .bet-input-wrap:hover {
            border-color: rgba(201, 168, 76, 0.15);
        }
        .bet-input-wrap label {
            font-size: 13px;
            opacity: 0.5;
            font-weight: 600;
        }
        .bet-input-wrap input {
            background: transparent;
            border: none;
            color: var(--gold);
            font-size: clamp(17px, 2vw, 22px);
            font-weight: 700;
            width: 70px;
            text-align: center;
            outline: none;
            padding: 6px 0;
        }
        .bet-input-wrap input::-webkit-inner-spin-button {
            -webkit-appearance: none;
        }

        .btn-spin {
            background: linear-gradient(135deg, var(--gold), var(--gold-dim));
            border: none;
            color: #1a0a0a;
            font-weight: 800;
            font-size: clamp(16px, 1.8vw, 22px);
            padding: 10px 34px;
            border-radius: 60px;
            cursor: pointer;
            transition: var(--transition-smooth);
            box-shadow: 0 4px 30px rgba(201, 168, 76, 0.15);
            position: relative;
            overflow: hidden;
        }
        .btn-spin::after {
            content: '';
            position: absolute;
            inset: 0;
            background: linear-gradient(135deg, transparent 30%, rgba(255, 255, 255, 0.12) 50%, transparent 70%);
            transform: translateX(-100%);
            transition: transform 0.5s ease;
        }
        .btn-spin:hover:not(:disabled)::after {
            transform: translateX(100%);
        }
        .btn-spin:hover:not(:disabled) {
            transform: scale(1.04);
            box-shadow: 0 8px 40px rgba(201, 168, 76, 0.25);
        }
        .btn-spin:active:not(:disabled) {
            transform: scale(0.96);
        }
        .btn-spin:disabled {
            opacity: 0.35;
            cursor: not-allowed;
            transform: none;
        }

        .slot-result {
            margin-top: 12px;
            font-size: clamp(15px, 1.4vw, 19px);
            min-height: 30px;
            font-weight: 600;
            color: var(--gold);
            background: rgba(0, 0, 0, 0.2);
            padding: 4px 16px;
            border-radius: 40px;
            display: inline-block;
            backdrop-filter: blur(4px);
            transition: var(--transition-smooth);
        }

        /* ---------- ROULETTE ---------- */
        .roulette-container {
            text-align: center;
        }
        .roulette-wheel-wrap {
            display: flex;
            flex-direction: column;
            align-items: center;
            margin: 8px 0 16px;
        }
        .wheel {
            width: clamp(200px, 35vw, 300px);
            height: clamp(200px, 35vw, 300px);
            border-radius: 50%;
            background: conic-gradient(#e74c3c 0deg 9.73deg, #2c3e50 9.73deg 19.46deg,
                    #e74c3c 19.46deg 29.19deg, #2c3e50 29.19deg 38.92deg,
                    #e74c3c 38.92deg 48.65deg, #2c3e50 48.65deg 58.38deg,
                    #e74c3c 58.38deg 68.11deg, #2c3e50 68.11deg 77.84deg,
                    #e74c3c 77.84deg 87.57deg, #2c3e50 87.57deg 97.30deg,
                    #e74c3c 97.30deg 107.03deg, #2c3e50 107.03deg 116.76deg,
                    #e74c3c 116.76deg 126.49deg, #2c3e50 126.49deg 136.22deg,
                    #e74c3c 136.22deg 145.95deg, #2c3e50 145.95deg 155.68deg,
                    #e74c3c 155.68deg 165.41deg, #2c3e50 165.41deg 175.14deg,
                    #e74c3c 175.14deg 184.86deg, #2c3e50 184.86deg 194.59deg,
                    #e74c3c 194.59deg 204.32deg, #2c3e50 204.32deg 214.05deg,
                    #e74c3c 214.05deg 223.78deg, #2c3e50 223.78deg 233.51deg,
                    #e74c3c 233.51deg 243.24deg, #2c3e50 243.24deg 252.97deg,
                    #e74c3c 252.97deg 262.70deg, #2c3e50 262.70deg 272.43deg,
                    #e74c3c 272.43deg 282.16deg, #2c3e50 282.16deg 291.89deg,
                    #e74c3c 291.89deg 301.62deg, #2c3e50 301.62deg 311.35deg,
                    #e74c3c 311.35deg 321.08deg, #2c3e50 321.08deg 330.81deg,
                    #e74c3c 330.81deg 340.54deg, #2c3e50 340.54deg 350.27deg,
                    #e74c3c 350.27deg 360deg);
            border: 5px solid var(--gold-dim);
            box-shadow: 0 0 0 3px rgba(0, 0, 0, 0.6), 0 0 60px rgba(201, 168, 76, 0.08);
            position: relative;
            transition: transform 4s cubic-bezier(0.17, 0.67, 0.12, 0.99);
        }
        .wheel.spinning {
            transition: transform 4.8s cubic-bezier(0.13, 0.71, 0.09, 0.99);
        }
        .wheel-center {
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            width: clamp(34px, 5vw, 48px);
            height: clamp(34px, 5vw, 48px);
            background: radial-gradient(circle, var(--gold), var(--gold-dim));
            border-radius: 50%;
            border: 3px solid #1a0a0a;
            box-shadow: 0 0 30px rgba(201, 168, 76, 0.3);
            z-index: 3;
        }
        .wheel-pointer {
            position: absolute;
            top: -12px;
            left: 50%;
            transform: translateX(-50%);
            width: 0;
            height: 0;
            border-left: 16px solid transparent;
            border-right: 16px solid transparent;
            border-top: 26px solid var(--gold);
            filter: drop-shadow(0 4px 12px rgba(0, 0, 0, 0.5));
            z-index: 4;
        }

        .roulette-numbers {
            display: grid;
            grid-template-columns: repeat(10, 1fr);
            gap: 4px;
            max-width: 480px;
            margin: 12px auto 10px;
        }
        .roulette-number {
            padding: 5px 3px;
            border-radius: 8px;
            font-size: clamp(11px, 1vw, 14px);
            font-weight: 700;
            text-align: center;
            cursor: pointer;
            transition: var(--transition-smooth);
            background: rgba(255, 255, 255, 0.03);
            border: 1px solid rgba(255, 255, 255, 0.04);
            color: rgba(255, 255, 255, 0.6);
        }
        .roulette-number:hover {
            background: rgba(201, 168, 76, 0.10);
            transform: scale(1.06);
            border-color: rgba(201, 168, 76, 0.15);
        }
        .roulette-number.selected {
            background: rgba(201, 168, 76, 0.18);
            border-color: var(--gold-dim);
            color: var(--gold);
            box-shadow: 0 0 30px rgba(201, 168, 76, 0.06);
            transform: scale(1.08);
        }
        .roulette-number.red {
            color: #e74c3c;
        }
        .roulette-number.black {
            color: #b0b0b0;
        }
        .roulette-number.green {
            color: #2ecc71;
        }

        .roulette-controls {
            display: flex;
            justify-content: center;
            align-items: center;
            gap: 16px;
            flex-wrap: wrap;
            margin-top: 6px;
        }
        .roulette-result {
            margin-top: 12px;
            font-size: clamp(16px, 1.6vw, 22px);
            font-weight: 600;
            min-height: 34px;
            color: var(--gold);
            background: rgba(0, 0, 0, 0.2);
            padding: 4px 18px;
            border-radius: 40px;
            display: inline-block;
            backdrop-filter: blur(4px);
        }

        /* ---------- BLACKJACK ---------- */
        .bj-container {
            text-align: center;
        }
        .bj-table {
            background: radial-gradient(ellipse at center, #1a5a2a, #0d2a15);
            border-radius: 32px;
            padding: 18px 16px 16px;
            border: 1px solid rgba(201, 168, 76, 0.10);
            box-shadow: inset 0 0 80px rgba(0, 0, 0, 0.3), 0 8px 40px rgba(0, 0, 0, 0.4);
            margin: 6px 0 14px;
            min-height: 220px;
        }
        .bj-hand {
            display: flex;
            flex-direction: column;
            align-items: center;
            margin: 6px 0;
        }
        .bj-hand-label {
            font-size: 12px;
            text-transform: uppercase;
            letter-spacing: 2px;
            opacity: 0.4;
            font-weight: 600;
        }
        .bj-hand-value {
            font-size: clamp(16px, 1.4vw, 20px);
            font-weight: 700;
            color: var(--gold);
            margin-top: 2px;
        }
        .bj-cards {
            display: flex;
            justify-content: center;
            gap: 8px;
            flex-wrap: wrap;
            margin: 4px 0 2px;
        }
        .bj-card {
            width: clamp(50px, 8vw, 76px);
            height: clamp(72px, 11vw, 106px);
            background: #fcf9f2;
            border-radius: 10px;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            font-size: clamp(18px, 2.5vw, 28px);
            font-weight: 800;
            color: #1a0a0a;
            box-shadow: 0 4px 20px rgba(0, 0, 0, 0.3);
            transition: var(--transition-smooth);
            border: 1px solid rgba(0, 0, 0, 0.08);
            line-height: 1;
        }
        .bj-card .suit {
            font-size: clamp(20px, 2.8vw, 30px);
        }
        .bj-card.red {
            color: #c0392b;
        }
        .bj-card.black {
            color: #1a1a1a;
        }
        .bj-card.face-down {
            background: linear-gradient(135deg, #2a1a8a, #1a0a5a);
            color: transparent;
            border: 2px solid var(--gold-dim);
            box-shadow: 0 4px 20px rgba(0, 0, 0, 0.5);
        }
        .bj-card.face-down .suit,
        .bj-card.face-down .rank {
            display: none;
        }
        .bj-card:hover:not(.face-down) {
            transform: translateY(-2px);
        }

        .bj-controls {
            display: flex;
            justify-content: center;
            gap: 8px;
            flex-wrap: wrap;
            margin-top: 8px;
        }
        .bj-btn {
            background: rgba(255, 255, 255, 0.04);
            border: 1px solid rgba(255, 255, 255, 0.06);
            color: var(--text-primary);
            padding: 8px 20px;
            border-radius: 60px;
            font-weight: 700;
            font-size: clamp(13px, 1.2vw, 16px);
            cursor: pointer;
            transition: var(--transition-smooth);
            min-width: 68px;
        }
        .bj-btn:hover:not(:disabled) {
            background: rgba(201, 168, 76, 0.10);
            border-color: rgba(201, 168, 76, 0.15);
            transform: translateY(-2px);
        }
        .bj-btn:active:not(:disabled) {
            transform: scale(0.94);
        }
        .bj-btn:disabled {
            opacity: 0.25;
            cursor: not-allowed;
            transform: none;
        }
        .bj-btn.primary {
            background: linear-gradient(135deg, var(--gold), var(--gold-dim));
            border-color: var(--gold-dim);
            color: #1a0a0a;
        }
        .bj-btn.primary:hover:not(:disabled) {
            transform: scale(1.04);
            box-shadow: 0 8px 30px rgba(201, 168, 76, 0.15);
        }
        .bj-btn.danger {
            border-color: rgba(231, 76, 60, 0.3);
            color: #e74c3c;
        }
        .bj-btn.danger:hover:not(:disabled) {
            background: rgba(231, 76, 60, 0.08);
            border-color: #e74c3c;
        }

        .bj-result {
            margin-top: 10px;
            font-size: clamp(18px, 1.8vw, 24px);
            font-weight: 700;
            min-height: 34px;
            color: var(--gold);
            background: rgba(0, 0, 0, 0.2);
            padding: 4px 16px;
            border-radius: 40px;
            display: inline-block;
            backdrop-filter: blur(4px);
        }

        /* ---------- WALLET MODAL ---------- */
        .modal-overlay {
            position: fixed;
            inset: 0;
            background: rgba(0, 0, 0, 0.7);
            backdrop-filter: blur(12px) saturate(1.2);
            -webkit-backdrop-filter: blur(12px) saturate(1.2);
            display: none;
            align-items: center;
            justify-content: center;
            z-index: 999;
            animation: modalFade 0.3s ease;
            padding: 16px;
        }
        .modal-overlay.open {
            display: flex;
        }
        @keyframes modalFade {
            0% {
                opacity: 0;
                transform: scale(0.94);
            }
            100% {
                opacity: 1;
                transform: scale(1);
            }
        }

        .modal {
            background: #1a0e0e;
            border: 1px solid rgba(201, 168, 76, 0.12);
            border-radius: var(--radius-lg);
            max-width: 500px;
            width: 100%;
            padding: 24px 22px 22px;
            box-shadow: 0 40px 100px rgba(0, 0, 0, 0.8);
            position: relative;
            max-height: 90vh;
            overflow-y: auto;
        }
        .modal-close {
            position: absolute;
            top: 12px;
            right: 16px;
            background: none;
            border: none;
            color: rgba(255, 255, 255, 0.25);
            font-size: 28px;
            cursor: pointer;
            transition: var(--transition-smooth);
        }
        .modal-close:hover {
            color: var(--text-primary);
            transform: rotate(90deg);
        }
        .modal-title {
            font-size: clamp(22px, 3vw, 28px);
            font-weight: 700;
            margin-bottom: 14px;
            color: var(--gold);
            display: flex;
            align-items: center;
            gap: 10px;
        }
        .modal-balance {
            background: rgba(0, 0, 0, 0.3);
            border-radius: 60px;
            padding: 8px 16px;
            text-align: center;
            font-size: 17px;
            border: 1px solid rgba(201, 168, 76, 0.06);
            margin-bottom: 12px;
        }
        .modal-balance span {
            color: var(--gold);
            font-weight: 700;
        }

        .modal-tabs {
            display: flex;
            gap: 4px;
            margin-bottom: 16px;
            border-bottom: 1px solid rgba(255, 255, 255, 0.04);
        }
        .modal-tab {
            background: transparent;
            border: none;
            color: rgba(255, 255, 255, 0.3);
            padding: 8px 18px;
            font-weight: 600;
            font-size: 15px;
            cursor: pointer;
            border-bottom: 3px solid transparent;
            transition: var(--transition-smooth);
        }
        .modal-tab.active {
            color: var(--gold);
            border-bottom-color: var(--gold-dim);
        }
        .modal-tab:hover {
            color: var(--text-primary);
        }

        .modal-body {
            padding: 4px 0;
        }
        .modal-form {
            display: none;
            flex-direction: column;
            gap: 14px;
        }
        .modal-form.active {
            display: flex;
        }
        .modal-form label {
            font-size: 13px;
            font-weight: 600;
            opacity: 0.5;
            letter-spacing: 0.3px;
        }
        .modal-form input,
        .modal-form select {
            background: rgba(0, 0, 0, 0.3);
            border: 1px solid rgba(255, 255, 255, 0.06);
            border-radius: 60px;
            padding: 10px 18px;
            color: var(--text-primary);
            font-size: 16px;
            outline: none;
            width: 100%;
            transition: var(--transition-smooth);
        }
        .modal-form input:focus,
        .modal-form select:focus {
            border-color: rgba(201, 168, 76, 0.2);
            box-shadow: 0 0 30px rgba(201, 168, 76, 0.03);
        }
        .modal-form input::placeholder {
            color: rgba(255, 255, 255, 0.15);
        }

        .modal-form .btn-primary {
            background: linear-gradient(135deg, var(--gold), var(--gold-dim));
            border: none;
            color: #1a0a0a;
            font-weight: 800;
            font-size: 18px;
            padding: 12px;
            border-radius: 60px;
            cursor: pointer;
            transition: var(--transition-smooth);
            margin-top: 2px;
            box-shadow: 0 4px 30px rgba(201, 168, 76, 0.10);
        }
        .modal-form .btn-primary:hover:not(:disabled) {
            transform: scale(1.02);
            box-shadow: 0 8px 40px rgba(201, 168, 76, 0.20);
        }
        .modal-form .btn-primary:disabled {
            opacity: 0.35;
            cursor: not-allowed;
        }

        .modal-message {
            margin-top: 8px;
            font-size: 14px;
            text-align: center;
            min-height: 26px;
            font-weight: 600;
            color: var(--gold);
        }
        .modal-message.error {
            color: #e74c3c;
        }
        .modal-message.success {
            color: #2ecc71;
        }

        .tx-history {
            margin-top: 16px;
            border-top: 1px solid rgba(255, 255, 255, 0.04);
            padding-top: 12px;
        }
        .tx-history h4 {
            font-size: 13px;
            text-transform: uppercase;
            letter-spacing: 1px;
            opacity: 0.3;
            margin-bottom: 8px;
        }
        .tx-list {
            max-height: 130px;
            overflow-y: auto;
            display: flex;
            flex-direction: column;
            gap: 5px;
            padding-right: 4px;
        }
        .tx-item {
            display: flex;
            justify-content: space-between;
            font-size: 13px;
            padding: 5px 12px;
            background: rgba(255, 255, 255, 0.02);
            border-radius: 30px;
            border-left: 3px solid var(--gold-dim);
            transition: var(--transition-smooth);
        }
        .tx-item.deposit {
            border-left-color: #2ecc71;
        }
        .tx-item.withdraw {
            border-left-color: #e74c3c;
        }
        .tx-item .tx-left {
            display: flex;
            gap: 10px;
            align-items: center;
            flex-wrap: wrap;
        }
        .tx-item .tx-method {
            opacity: 0.4;
            font-size: 11px;
        }
        .tx-item .tx-time {
            font-size: 10px;
            opacity: 0.25;
        }
        .tx-item .tx-right {
            font-weight: 600;
        }
        .tx-item .tx-right.positive {
            color: #2ecc71;
        }
        .tx-item .tx-right.negative {
            color: #e74c3c;
        }

        /* ---------- SOCIAL FOOTER ---------- */
        .social-footer {
            margin-top: 24px;
            padding: 14px 0 6px;
            border-top: 1px solid rgba(255, 255, 255, 0.04);
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            align-items: center;
            gap: 16px 28px;
            position: relative;
            z-index: 2;
        }
        .social-footer a {
            display: flex;
            align-items: center;
            gap: 8px;
            color: rgba(255, 255, 255, 0.3);
            text-decoration: none;
            font-size: 14px;
            font-weight: 500;
            transition: var(--transition-smooth);
            letter-spacing: 0.3px;
        }
        .social-footer a:hover {
            color: var(--gold);
            transform: translateY(-2px);
        }
        .social-footer a .icon {
            font-size: 22px;
            transition: var(--transition-smooth);
        }
        .social-footer a:hover .icon {
            transform: scale(1.15);
        }
        .social-footer .handle {
            opacity: 0.6;
        }
        .social-footer .handle:hover {
            opacity: 1;
        }

        /* ---------- DISCLAIMER ---------- */
        .disclaimer {
            margin-top: 8px;
            padding: 10px 16px 4px;
            text-align: center;
            font-size: 12px;
            color: rgba(255, 255, 255, 0.10);
            letter-spacing: 0.3px;
            position: relative;
            z-index: 2;
        }
        .disclaimer strong {
            color: rgba(255, 255, 255, 0.20);
        }

        /* ---------- RESPONSIVE ---------- */
        @media (max-width: 768px) {
            .container {
                padding: 16px 14px 14px;
                border-radius: 20px;
            }
            .header {
                gap: 10px;
            }
            .tabs {
                gap: 2px;
                padding: 3px;
                border-radius: 40px;
                overflow-x: auto;
                flex-wrap: nowrap;
                -webkit-overflow-scrolling: touch;
            }
            .tab-btn {
                padding: 6px 14px;
                font-size: 13px;
                min-width: 50px;
                flex: 0 0 auto;
            }
            .arcade-grid {
                grid-template-columns: repeat(auto-fill, minmax(110px, 1fr));
                gap: 10px;
            }
            .game-card {
                padding: 14px 6px 10px;
            }
            .game-card .icon {
                font-size: 30px;
            }
            .roulette-numbers {
                grid-template-columns: repeat(7, 1fr);
                gap: 3px;
            }
            .bj-table {
                padding: 14px 10px;
                min-height: 180px;
            }
            .bj-card {
                width: 46px;
                height: 66px;
                font-size: 16px;
            }
            .bj-card .suit {
                font-size: 18px;
            }
            .bj-btn {
                padding: 6px 14px;
                font-size: 13px;
                min-width: 56px;
            }
            .balance-wrap {
                padding: 4px 12px 4px 16px;
                gap: 8px;
            }
            .balance-amount {
                font-size: 17px;
                min-width: 50px;
            }
            .btn-outline {
                font-size: 12px;
                padding: 4px 12px;
            }
            .btn-reset {
                font-size: 11px;
                padding: 4px 10px;
            }
            .modal {
                padding: 18px 16px;
            }
            .game-view .options button {
                padding: 5px 12px;
                font-size: 13px;
            }
            .game-view .bet-ctrl input {
                width: 80px;
                font-size: 16px;
                padding: 6px 12px;
            }
            .slots-controls {
                gap: 10px;
            }
            .btn-spin {
                padding: 8px 24px;
                font-size: 16px;
            }
            .bet-input-wrap {
                padding: 2px 10px 2px 14px;
            }
            .bet-input-wrap input {
                width: 60px;
                font-size: 16px;
            }
            .reel {
                width: 60px;
                height: 76px;
            }
            .reel .symbol {
                font-size: 34px;
            }
            .social-footer {
                gap: 12px 20px;
            }
            .social-footer a {
                font-size: 13px;
            }
        }

        @media (max-width: 480px) {
            body {
                padding: 10px;
            }
            .container {
                padding: 12px 10px 12px;
                border-radius: 16px;
            }
            .arcade-grid {
                grid-template-columns: repeat(auto-fill, minmax(90px, 1fr));
                gap: 8px;
            }
            .game-card {
                padding: 10px 4px 8px;
                border-radius: 12px;
            }
            .game-card .icon {
                font-size: 26px;
            }
            .game-card .name {
                font-size: 11px;
            }
            .game-card .desc {
                font-size: 9px;
            }
            .roulette-numbers {
                grid-template-columns: repeat(5, 1fr);
                gap: 3px;
            }
            .roulette-number {
                font-size: 10px;
                padding: 4px 2px;
            }
            .wheel {
                width: 160px;
                height: 160px;
            }
            .wheel-center {
                width: 28px;
                height: 28px;
            }
            .wheel-pointer {
                border-left-width: 12px;
                border-right-width: 12px;
                border-top-width: 20px;
                top: -10px;
            }
            .bj-card {
                width: 38px;
                height: 54px;
                font-size: 13px;
            }
            .bj-card .suit {
                font-size: 15px;
            }
            .bj-btn {
                padding: 4px 10px;
                font-size: 12px;
                min-width: 48px;
            }
            .tab-btn {
                font-size: 11px;
                padding: 4px 10px;
                min-width: 40px;
            }
            .game-view .game-title {
                font-size: 20px;
            }
            .game-view .options button {
                font-size: 12px;
                padding: 4px 10px;
            }
            .game-view .play-btn {
                font-size: 16px;
                padding: 8px 28px;
            }
            .modal {
                padding: 14px 12px;
                border-radius: 20px;
            }
            .modal-title {
                font-size: 20px;
            }
            .balance-amount {
                font-size: 15px;
                min-width: 44px;
            }
            .btn-outline {
                font-size: 11px;
                padding: 3px 10px;
            }
            .btn-reset {
                font-size: 10px;
                padding: 3px 8px;
            }
            .reel {
                width: 48px;
                height: 62px;
            }
            .reel .symbol {
                font-size: 28px;
            }
            .btn-spin {
                padding: 6px 18px;
                font-size: 14px;
            }
            .bet-input-wrap input {
                width: 50px;
                font-size: 14px;
            }
            .slot-result,
            .roulette-result,
            .bj-result {
                font-size: 14px;
                padding: 3px 12px;
            }
            .social-footer {
                gap: 10px 16px;
            }
            .social-footer a {
                font-size: 12px;
            }
            .social-footer a .icon {
                font-size: 18px;
            }
        }

        /* ---------- UTILITY ---------- */
        .text-gold {
            color: var(--gold);
        }
        .text-muted {
            opacity: 0.4;
        }
        .mt-1 {
            margin-top: 6px;
        }
        .mb-1 {
            margin-bottom: 6px;
        }
        .flex-center {
            display: flex;
            align-items: center;
            justify-content: center;
        }
        .gap-1 {
            gap: 8px;
        }
        .w-full {
            width: 100%;
        }
    </style>
</head>
<body>

    <!-- Floating orbs -->
    <div class="orb orb-1"></div>
    <div class="orb orb-2"></div>
    <div class="orb orb-3"></div>

    <div class="container">

        <!-- ===== HEADER ===== -->
        <header class="header">
            <div class="logo"><span>🎰</span> Jannat Games</div>
            <div class="header-actions">
                <div class="balance-wrap">
                    <span class="balance-label">💰 Bankroll</span>
                    <span class="balance-amount" id="balanceDisplay">1,000</span>
                </div>
                <button class="btn-outline wallet" id="walletBtn">💳 Wallet</button>
                <button class="btn-reset" id="resetBtn">↺</button>
            </div>
        </header>

        <!-- ===== TABS ===== -->
        <nav class="tabs">
            <button class="tab-btn active" data-tab="slots">🎰 Slots</button>
            <button class="tab-btn" data-tab="roulette">🎡 Roulette</button>
            <button class="tab-btn" data-tab="blackjack">🃏 BJ</button>
            <button class="tab-btn" data-tab="arcade">🎮 Arcade</button>
        </nav>

        <!-- ============================================================ -->
        <!-- SLOTS -->
        <!-- ============================================================ -->
        <section class="game-panel active" id="panel-slots">
            <div class="slots-container">
                <div class="reels">
                    <div class="reel" id="reel1"><span class="symbol">🍒</span></div>
                    <div class="reel" id="reel2"><span class="symbol">🍒</span></div>
                    <div class="reel" id="reel3"><span class="symbol">🍒</span></div>
                </div>
                <div class="slots-controls">
                    <div class="bet-input-wrap">
                        <label>Bet</label>
                        <input type="number" id="slotBet" value="10" min="1" step="1" />
                    </div>
                    <button class="btn-spin" id="spinBtn">▶ SPIN</button>
                </div>
                <div class="slot-result" id="slotResult">Place your bet & spin!</div>
            </div>
        </section>

        <!-- ============================================================ -->
        <!-- ROULETTE -->
        <!-- ============================================================ -->
        <section class="game-panel" id="panel-roulette">
            <div class="roulette-container">
                <div class="roulette-wheel-wrap">
                    <div class="wheel" id="rouletteWheel">
                        <div class="wheel-center"></div>
                        <div class="wheel-pointer"></div>
                    </div>
                </div>
                <div class="roulette-numbers" id="rouletteNumbers"></div>
                <div class="roulette-controls">
                    <div class="bet-input-wrap">
                        <label>Bet</label>
                        <input type="number" id="rouletteBet" value="10" min="1" step="1" />
                    </div>
                    <button class="btn-spin" id="rouletteSpinBtn">🎡 SPIN</button>
                </div>
                <div class="roulette-result" id="rouletteResult">Pick a number and spin!</div>
            </div>
        </section>

        <!-- ============================================================ -->
        <!-- BLACKJACK -->
        <!-- ============================================================ -->
        <section class="game-panel" id="panel-blackjack">
            <div class="bj-container">
                <div class="bj-table">
                    <div class="bj-hand">
                        <span class="bj-hand-label">Dealer</span>
                        <div class="bj-cards" id="dealerCards"></div>
                        <div class="bj-hand-value" id="dealerValue">?</div>
                    </div>
                    <div class="bj-hand" style="margin-top:10px;">
                        <span class="bj-hand-label">You</span>
                        <div class="bj-cards" id="playerCards"></div>
                        <div class="bj-hand-value" id="playerValue">0</div>
                    </div>
                </div>
                <div class="bj-controls">
                    <div class="bet-input-wrap">
                        <label>Bet</label>
                        <input type="number" id="bjBet" value="10" min="1" step="1" />
                    </div>
                    <button class="bj-btn primary" id="bjDealBtn">🔄 Deal</button>
                    <button class="bj-btn" id="bjHitBtn" disabled>Hit</button>
                    <button class="bj-btn" id="bjStandBtn" disabled>Stand</button>
                    <button class="bj-btn danger" id="bjDoubleBtn" disabled>Double</button>
                </div>
                <div class="bj-result" id="bjResult">Press Deal to start</div>
            </div>
        </section>

        <!-- ============================================================ -->
        <!-- ARCADE -->
        <!-- ============================================================ -->
        <section class="game-panel" id="panel-arcade">
            <div id="arcadeGrid" class="arcade-grid"></div>
            <div id="arcadeGameView" class="game-view">
                <button class="back-btn" id="arcadeBackBtn">← Back</button>
                <div class="game-title" id="arcadeGameTitle">Game</div>
                <div class="game-area" id="arcadeGameArea"></div>
                <div class="result" id="arcadeResult"></div>
                <div class="history" id="arcadeHistory"></div>
            </div>
        </section>

        <!-- ============================================================ -->
        <!-- WALLET MODAL -->
        <!-- ============================================================ -->
        <div class="modal-overlay" id="walletModal">
            <div class="modal">
                <button class="modal-close" id="modalClose">✕</button>
                <div class="modal-title">💳 Wallet</div>
                <div class="modal-balance">Balance: <span id="modalBalance">1,000</span></div>
                <div class="modal-tabs">
                    <button class="modal-tab active" data-wtab="deposit">Deposit</button>
                    <button class="modal-tab" data-wtab="withdraw">Withdraw</button>
                </div>
                <div class="modal-body">
                    <div class="modal-form active" id="depositForm">
                        <label for="depositAmount">Amount (₹)</label>
                        <input type="number" id="depositAmount" placeholder="Enter amount" min="1" step="1" value="100" />
                        <label for="depositMethod">Payment Method</label>
                        <select id="depositMethod">
                            <option value="Paytm">Paytm</option>
                            <option value="PhonePe">PhonePe</option>
                            <option value="Google Pay">Google Pay</option>
                        </select>
                        <label for="depositUPI">UPI ID (optional)</label>
                        <input type="text" id="depositUPI" placeholder="e.g. example@upi" />
                        <button class="btn-primary" id="depositBtn">💰 Deposit Now</button>
                        <div class="modal-message" id="depositMsg"></div>
                    </div>
                    <div class="modal-form" id="withdrawForm">
                        <label for="withdrawAmount">Amount (₹)</label>
                        <input type="number" id="withdrawAmount" placeholder="Enter amount" min="1" step="1" value="50" />
                        <label for="withdrawMethod">Withdraw to</label>
                        <select id="withdrawMethod">
                            <option value="Bank Transfer">Bank Transfer</option>
                            <option value="UPI">UPI</option>
                            <option value="Paytm">Paytm</option>
                        </select>
                        <label for="withdrawUPI">UPI ID (optional)</label>
                        <input type="text" id="withdrawUPI" placeholder="e.g. example@upi" />
                        <button class="btn-primary" id="withdrawBtn">💸 Withdraw Now</button>
                        <div class="modal-message" id="withdrawMsg"></div>
                    </div>
                </div>
                <div class="tx-history">
                    <h4>📜 Transaction History</h4>
                    <div class="tx-list" id="txList"></div>
                </div>
            </div>
        </div>

        <!-- ============================================================ -->
        <!-- SOCIAL FOOTER – Instagram handles                            -->
        <!-- ============================================================ -->
        <div class="social-footer">
            <a href="https://instagram.com/_.ankittttt16" target="_blank" rel="noopener">
                <span class="icon">📸</span>
                <span class="handle">@_.ankittttt16</span>
            </a>
            <a href="https://instagram.com/trady._ankitt" target="_blank" rel="noopener">
                <span class="icon">📸</span>
                <span class="handle">@trady._ankitt</span>
            </a>
        </div>

        <!-- ===== DISCLAIMER ===== -->
        <div class="disclaimer">
            <strong>🎯 For entertainment only.</strong> No real money. Must be 18+.
        </div>
    </div>

    <!-- ============================================================ -->
    <!-- JAVASCRIPT – Full Game Logic with Premium UI                   -->
    <!-- ============================================================ -->
    <script>
        (function() {
            'use strict';

            // ---------- STATE ----------
            let balance = 1000;
            let transactions = [];

            // DOM refs
            const balanceDisplay = document.getElementById('balanceDisplay');
            const resetBtn = document.getElementById('resetBtn');
            const walletBtn = document.getElementById('walletBtn');
            const walletModal = document.getElementById('walletModal');
            const modalClose = document.getElementById('modalClose');
            const modalBalance = document.getElementById('modalBalance');
            const txList = document.getElementById('txList');

            const wTabs = document.querySelectorAll('.modal-tab');
            const depositForm = document.getElementById('depositForm');
            const withdrawForm = document.getElementById('withdrawForm');
            const depositBtn = document.getElementById('depositBtn');
            const withdrawBtn = document.getElementById('withdrawBtn');
            const depositAmount = document.getElementById('depositAmount');
            const withdrawAmount = document.getElementById('withdrawAmount');
            const depositMethod = document.getElementById('depositMethod');
            const withdrawMethod = document.getElementById('withdrawMethod');
            const depositUPI = document.getElementById('depositUPI');
            const withdrawUPI = document.getElementById('withdrawUPI');
            const depositMsg = document.getElementById('depositMsg');
            const withdrawMsg = document.getElementById('withdrawMsg');

            // ---------- HELPERS ----------
            function updateBalance() {
                balanceDisplay.textContent = balance.toLocaleString();
                if (modalBalance) modalBalance.textContent = balance.toLocaleString();
                // pulse animation
                balanceDisplay.classList.remove('pulse');
                void balanceDisplay.offsetWidth;
                balanceDisplay.classList.add('pulse');
            }

            function canBet(amount) { return amount > 0 && amount <= balance; }

            function deduct(amount) {
                if (!canBet(amount)) return false;
                balance -= amount;
                updateBalance();
                return true;
            }

            function add(amount) {
                balance += amount;
                updateBalance();
            }

            // ---------- TRANSACTIONS ----------
            function addTransaction(type, method, amount, status = 'success', details = '') {
                const now = new Date();
                const timeStr = now.toLocaleTimeString('en-IN', { hour: '2-digit', minute: '2-digit' });
                transactions.push({ type, method, amount, status, details, time: timeStr, timestamp: now.getTime() });
                renderTransactions();
            }

            function renderTransactions() {
                if (!txList) return;
                if (transactions.length === 0) {
                    txList.innerHTML =
                        `<div style="opacity:0.25; text-align:center; padding:10px; font-size:13px;">No transactions yet</div>`;
                    return;
                }
                const reversed = [...transactions].reverse();
                txList.innerHTML = reversed.map(tx => {
                    const cls = tx.type === 'deposit' ? 'deposit' : 'withdraw';
                    const sign = tx.type === 'deposit' ? '+' : '-';
                    const colorClass = tx.type === 'deposit' ? 'positive' : 'negative';
                    return `<div class="tx-item ${cls}">
                                <div class="tx-left"><span>${tx.type === 'deposit' ? '💰' : '💸'} ${tx.type}</span>
                                <span class="tx-method">${tx.method}</span><span class="tx-time">${tx.time}</span></div>
                                <div class="tx-right ${colorClass}">${sign}₹${tx.amount.toLocaleString()}</div>
                            </div>`;
                }).join('');
            }

            // ---------- RESET ----------
            resetBtn.addEventListener('click', () => {
                balance = 1000;
                updateBalance();
                resetSlots();
                resetRoulette();
                resetBlackjack();
                depositMsg.textContent = '';
                withdrawMsg.textContent = '';
                transactions = [];
                renderTransactions();
            });

            // ================================================================
            //  TABS
            // ================================================================
            const tabBtns = document.querySelectorAll('.tab-btn');
            const panels = {
                slots: document.getElementById('panel-slots'),
                roulette: document.getElementById('panel-roulette'),
                blackjack: document.getElementById('panel-blackjack'),
                arcade: document.getElementById('panel-arcade'),
            };
            tabBtns.forEach(btn => {
                btn.addEventListener('click', () => {
                    tabBtns.forEach(b => b.classList.remove('active'));
                    btn.classList.add('active');
                    const tab = btn.dataset.tab;
                    Object.keys(panels).forEach(key => {
                        panels[key].classList.toggle('active', key === tab);
                    });
                    if (tab === 'arcade') {
                        document.getElementById('arcadeGrid').style.display = 'grid';
                        document.getElementById('arcadeGameView').classList.remove('active');
                    }
                });
            });

            // ================================================================
            //  WALLET
            // ================================================================
            function openModal() {
                walletModal.classList.add('open');
                modalBalance.textContent = balance.toLocaleString();
                depositMsg.textContent = '';
                withdrawMsg.textContent = '';
                wTabs.forEach(t => t.classList.remove('active'));
                document.querySelector('.modal-tab[data-wtab="deposit"]').classList.add('active');
                depositForm.classList.add('active');
                withdrawForm.classList.remove('active');
                renderTransactions();
            }
            walletBtn.addEventListener('click', openModal);
            modalClose.addEventListener('click', () => walletModal.classList.remove('open'));
            walletModal.addEventListener('click', (e) => { if (e.target === walletModal) walletModal.classList.remove(
                    'open'); });

            wTabs.forEach(tab => {
                tab.addEventListener('click', () => {
                    wTabs.forEach(t => t.classList.remove('active'));
                    tab.classList.add('active');
                    const target = tab.dataset.wtab;
                    if (target === 'deposit') {
                        depositForm.classList.add('active');
                        withdrawForm.classList.remove('active');
                        depositMsg.textContent = '';
                    } else {
                        withdrawForm.classList.add('active');
                        depositForm.classList.remove('active');
                        withdrawMsg.textContent = '';
                    }
                });
            });

            depositBtn.addEventListener('click', () => {
                const amount = parseInt(depositAmount.value, 10);
                if (!amount || amount <= 0) { depositMsg.textContent = '⚠️ Valid amount required.';
                    depositMsg.className = 'modal-message error'; return; }
                const method = depositMethod.value;
                depositMsg.textContent = '⏳ Processing...';
                depositMsg.className = 'modal-message';
                depositBtn.disabled = true;
                setTimeout(() => {
                    add(amount);
                    modalBalance.textContent = balance.toLocaleString();
                    addTransaction('deposit', method, amount, 'success', 'UPI: ' + (depositUPI.value.trim() || 'N/A'));
                    depositMsg.textContent =
                        `✅ ₹${amount.toLocaleString()} deposited via ${method}. Balance: ₹${balance.toLocaleString()}`;
                    depositMsg.className = 'modal-message success';
                    depositBtn.disabled = false;
                    updateBalance();
                }, 1200);
            });

            withdrawBtn.addEventListener('click', () => {
                const amount = parseInt(withdrawAmount.value, 10);
                if (!amount || amount <= 0) { withdrawMsg.textContent = '⚠️ Valid amount required.';
                    withdrawMsg.className = 'modal-message error'; return; }
                if (amount > balance) { withdrawMsg.textContent = '❌ Insufficient balance.';
                    withdrawMsg.className = 'modal-message error'; return; }
                const method = withdrawMethod.value;
                withdrawMsg.textContent = '⏳ Processing...';
                withdrawMsg.className = 'modal-message';
                withdrawBtn.disabled = true;
                setTimeout(() => {
                    deduct(amount);
                    modalBalance.textContent = balance.toLocaleString();
                    addTransaction('withdraw', method, amount, 'success', 'UPI: ' + (withdrawUPI.value.trim() || 'N/A'));
                    withdrawMsg.textContent =
                        `✅ ₹${amount.toLocaleString()} withdrawn via ${method}. Balance: ₹${balance.toLocaleString()}`;
                    withdrawMsg.className = 'modal-message success';
                    withdrawBtn.disabled = false;
                    updateBalance();
                }, 1200);
            });

            // ================================================================
            //  SLOTS
            // ================================================================
            const SYMBOLS = ['🍒', '🍋', '🍊', '🍇', '🔔', '💎', '7️⃣', '⭐'];
            const SYM_PAYOUTS = { '🍒': 2, '🍋': 3, '🍊': 4, '🍇': 5, '🔔': 8, '💎': 15, '7️⃣': 25, '⭐': 50 };
            const reelEls = [
                document.getElementById('reel1'),
                document.getElementById('reel2'),
                document.getElementById('reel3')
            ];
            const spinBtn = document.getElementById('spinBtn');
            const slotBetInput = document.getElementById('slotBet');
            const slotResult = document.getElementById('slotResult');
            let isSpinning = false;

            function getRandomSymbol() { return SYMBOLS[Math.floor(Math.random() * SYMBOLS.length)]; }

            function resetSlots() {
                reelEls.forEach(reel => { reel.querySelector('.symbol').textContent = '🍒';
                    reel.classList.remove('spinning'); });
                slotResult.textContent = 'Place your bet & spin!';
                isSpinning = false;
                spinBtn.disabled = false;
            }

            function spinSlots() {
                if (isSpinning) return;
                const bet = parseInt(slotBetInput.value, 10) || 10;
                if (!canBet(bet)) { slotResult.textContent = '❌ Insufficient balance!'; return; }
                if (!deduct(bet)) return;
                isSpinning = true;
                spinBtn.disabled = true;
                slotResult.textContent = '🎰 Spinning...';
                reelEls.forEach(reel => reel.classList.add('spinning'));
                const results = [getRandomSymbol(), getRandomSymbol(), getRandomSymbol()];
                setTimeout(() => { reelEls[0].classList.remove('spinning');
                    reelEls[0].querySelector('.symbol').textContent = results[0]; }, 400);
                setTimeout(() => { reelEls[1].classList.remove('spinning');
                    reelEls[1].querySelector('.symbol').textContent = results[1]; }, 900);
                setTimeout(() => {
                    reelEls[2].classList.remove('spinning');
                    reelEls[2].querySelector('.symbol').textContent = results[2];
                    const [a, b, c] = results;
                    let win = 0,
                        msg = '';
                    if (a === b && b === c) { win = bet * (SYM_PAYOUTS[a] || 2);
                        msg = `🎉 JACKPOT! Three ${a} — win ₹${win.toLocaleString()}!`; } else if (a === b || b === c || a ===
                        c) {
                        const matched = a === b ? a : (b === c ? b : c);
                        win = Math.round(bet * (SYM_PAYOUTS[matched] || 1.5));
                        msg = `✨ Pair of ${matched} — win ₹${win.toLocaleString()}!`;
                    } else msg = `😔 No match.`;
                    if (win > 0) add(win);
                    slotResult.textContent = msg + ` (Balance: ₹${balance.toLocaleString()})`;
                    isSpinning = false;
                    spinBtn.disabled = false;
                }, 1400);
            }
            spinBtn.addEventListener('click', spinSlots);
            slotBetInput.addEventListener('keydown', (e) => { if (e.key === 'Enter') spinSlots(); });

            // ================================================================
            //  ROULETTE
            // ================================================================
            const ROULETTE_NUMBERS = [0, 32, 15, 19, 4, 21, 2, 25, 17, 34, 6, 27, 13, 36, 11, 30, 8, 23, 10, 5, 24, 16, 33, 1,
                20, 14, 31, 9, 22, 18, 29, 7, 28, 12, 35, 3, 26
            ];
            const RED_NUMBERS = new Set([1, 3, 5, 7, 9, 12, 14, 16, 18, 19, 21, 23, 25, 27, 30, 32, 34, 36]);
            const rouletteWheel = document.getElementById('rouletteWheel');
            const rouletteNumbersEl = document.getElementById('rouletteNumbers');
            const rouletteSpinBtn = document.getElementById('rouletteSpinBtn');
            const rouletteBetInput = document.getElementById('rouletteBet');
            const rouletteResult = document.getElementById('rouletteResult');
            let selectedNumber = null,
                rouletteSpinning = false;

            ROULETTE_NUMBERS.forEach(num => {
                const div = document.createElement('div');
                div.className = 'roulette-number';
                div.textContent = num;
                if (num === 0) div.classList.add('green');
                else if (RED_NUMBERS.has(num)) div.classList.add('red');
                else div.classList.add('black');
                div.dataset.num = num;
                div.addEventListener('click', () => {
                    if (rouletteSpinning) return;
                    document.querySelectorAll('.roulette-number').forEach(el => el.classList.remove('selected'));
                    div.classList.add('selected');
                    selectedNumber = num;
                    rouletteResult.textContent = `Selected ${num}. Place your bet & spin!`;
                });
                rouletteNumbersEl.appendChild(div);
            });

            function resetRoulette() {
                document.querySelectorAll('.roulette-number').forEach(el => el.classList.remove('selected'));
                selectedNumber = null;
                rouletteResult.textContent = 'Pick a number and spin!';
                rouletteWheel.style.transform = 'rotate(0deg)';
                rouletteSpinning = false;
                rouletteSpinBtn.disabled = false;
            }

            function spinRoulette() {
                if (rouletteSpinning) return;
                if (selectedNumber === null) { rouletteResult.textContent = '⚠️ Select a number first!'; return; }
                const bet = parseInt(rouletteBetInput.value, 10) || 10;
                if (!canBet(bet)) { rouletteResult.textContent = '❌ Insufficient balance!'; return; }
                if (!deduct(bet)) return;
                rouletteSpinning = true;
                rouletteSpinBtn.disabled = true;
                rouletteResult.textContent = '🎡 Spinning...';
                const resultIndex = Math.floor(Math.random() * ROULETTE_NUMBERS.length);
                const result = ROULETTE_NUMBERS[resultIndex];
                const segmentAngle = 360 / ROULETTE_NUMBERS.length;
                const targetAngle = resultIndex * segmentAngle + segmentAngle / 2;
                const spins = 5 + Math.floor(Math.random() * 4);
                const totalRotation = spins * 360 + (360 - targetAngle);
                rouletteWheel.style.transform = `rotate(${totalRotation}deg)`;
                rouletteWheel.classList.add('spinning');
                setTimeout(() => {
                    rouletteWheel.classList.remove('spinning');
                    const win = (result === selectedNumber) ? bet * 35 : 0;
                    if (win > 0) { add(win);
                        rouletteResult.textContent =
                            `🎉 Ball landed on ${result}! You win ₹${win.toLocaleString()}! (Balance: ₹${balance.toLocaleString()})`; } else
                        rouletteResult.textContent =
                        `😔 Ball landed on ${result}. (Balance: ₹${balance.toLocaleString()})`;
                    rouletteSpinning = false;
                    rouletteSpinBtn.disabled = false;
                }, 4800);
            }
            rouletteSpinBtn.addEventListener('click', spinRoulette);
            rouletteBetInput.addEventListener('keydown', (e) => { if (e.key === 'Enter') spinRoulette(); });

            // ================================================================
            //  BLACKJACK
            // ================================================================
            const SUITS = ['♠', '♥', '♦', '♣'];
            const RANKS = ['A', '2', '3', '4', '5', '6', '7', '8', '9', '10', 'J', 'Q', 'K'];
            let deck = [],
                playerHand = [],
                dealerHand = [],
                bjGameActive = false,
                bjBetAmount = 0;
            const dealerCardsEl = document.getElementById('dealerCards');
            const playerCardsEl = document.getElementById('playerCards');
            const dealerValueEl = document.getElementById('dealerValue');
            const playerValueEl = document.getElementById('playerValue');
            const bjResult = document.getElementById('bjResult');
            const bjBetInput = document.getElementById('bjBet');
            const bjDealBtn = document.getElementById('bjDealBtn');
            const bjHitBtn = document.getElementById('bjHitBtn');
            const bjStandBtn = document.getElementById('bjStandBtn');
            const bjDoubleBtn = document.getElementById('bjDoubleBtn');

            function createDeck() { const d = []; for (const suit of SUITS)
                    for (const rank of RANKS) d.push({ rank, suit }); return shuffle(d); }

            function shuffle(arr) { for (let i = arr.length - 1; i > 0; i--) { const j = Math.floor(Math.random() * (i +
                        1));
                    [arr[i], arr[j]] = [arr[j], arr[i]]; } return arr; }

            function cardValue(c) { if (c.rank === 'A') return 11; if (['J', 'Q', 'K'].includes(c.rank)) return 10; return parseInt(
                    c.rank, 10); }

            function handTotal(hand) { let total = hand.reduce((s, c) => s + cardValue(c), 0); let aces = hand.filter(c => c
                    .rank === 'A').length; while (total > 21 && aces > 0) { total -= 10;
                    aces--; } return total; }

            function cardHTML(c, faceDown = false) {
                if (faceDown) return `<div class="bj-card face-down"><span class="rank">?</span><span class="suit">?</span></div>`;
                const isRed = c.suit === '♥' || c.suit === '♦';
                return `<div class="bj-card ${isRed?'red':'black'}"><span class="rank">${c.rank}</span><span class="suit">${c.suit}</span></div>`;
            }

            function renderBJ() {
                let dealerHTML = '';
                if (bjGameActive) { dealerHTML = cardHTML(dealerHand[0], true); for (let i = 1; i < dealerHand.length; i++)
                        dealerHTML += cardHTML(dealerHand[i]);
                    dealerValueEl.textContent = '?'; } else { dealerHTML = dealerHand.map(c => cardHTML(c)).join('');
                    dealerValueEl.textContent = handTotal(dealerHand) || '0'; }
                dealerCardsEl.innerHTML = dealerHTML;
                playerCardsEl.innerHTML = playerHand.map(c => cardHTML(c)).join('');
                playerValueEl.textContent = handTotal(playerHand) || '0';
            }

            function resetBlackjack() {
                deck = createDeck();
                playerHand = [];
                dealerHand = [];
                bjGameActive = false;
                bjBetAmount = 0;
                bjDealBtn.disabled = false;
                bjHitBtn.disabled = true;
                bjStandBtn.disabled = true;
                bjDoubleBtn.disabled = true;
                bjResult.textContent = 'Press Deal to start';
                renderBJ();
                dealerValueEl.textContent = '?';
            }

            function dealBJ() {
                if (bjGameActive) return;
                const bet = parseInt(bjBetInput.value, 10) || 10;
                if (!canBet(bet)) { bjResult.textContent = '❌ Insufficient balance!'; return; }
                if (!deduct(bet)) return;
                bjBetAmount = bet;
                deck = createDeck();
                playerHand = [deck.pop(), deck.pop()];
                dealerHand = [deck.pop(), deck.pop()];
                bjGameActive = true;
                bjDealBtn.disabled = true;
                bjHitBtn.disabled = false;
                bjStandBtn.disabled = false;
                bjDoubleBtn.disabled = (playerHand.length === 2) && (handTotal(playerHand) >= 9 && handTotal(playerHand) <=
                11);
                bjResult.textContent = '';
                renderBJ();
                const pTotal = handTotal(playerHand),
                    dTotal = handTotal(dealerHand);
                if (pTotal === 21 && dTotal === 21) { bjResult.textContent = '🤝 Push.';
                    add(bet);
                    endBJHand(); return; }
                if (pTotal === 21) { bjResult.textContent = '🎉 BLACKJACK!';
                    add(bet * 2.5);
                    endBJHand(); return; }
                if (dTotal === 21) { bjResult.textContent = '😔 Dealer Blackjack.';
                    endBJHand(); return; }
                if (pTotal === 21) standBJ();
            }

            function hitBJ() {
                if (!bjGameActive) return;
                playerHand.push(deck.pop());
                renderBJ();
                if (handTotal(playerHand) > 21) { bjResult.textContent = '💥 BUST!';
                    endBJHand(); } else if (handTotal(playerHand) === 21) standBJ();
                bjDoubleBtn.disabled = true;
            }

            function standBJ() {
                if (!bjGameActive) return;
                bjHitBtn.disabled = true;
                bjStandBtn.disabled = true;
                bjDoubleBtn.disabled = true;
                let dTotal = handTotal(dealerHand);
                while (dTotal < 17) { dealerHand.push(deck.pop());
                    dTotal = handTotal(dealerHand); }
                renderBJ();
                dealerValueEl.textContent = dTotal;
                const pTotal = handTotal(playerHand);
                let msg = '',
                    win = 0;
                if (pTotal > 21) msg = '💥 You busted.';
                else if (dTotal > 21) { msg = '🎉 Dealer busts! You win!';
                    win = bjBetAmount * 2; } else if (pTotal > dTotal) { msg = '🎉 You win!';
                    win = bjBetAmount * 2; } else if (pTotal < dTotal) msg = '😔 Dealer wins.'; else { msg = '🤝 Push.';
                    win = bjBetAmount; }
                if (win > 0) add(win);
                bjResult.textContent = msg + ` (Balance: ₹${balance.toLocaleString()})`;
                endBJHand();
            }

            function doubleBJ() {
                if (!bjGameActive || playerHand.length !== 2) return;
                const bet = bjBetAmount;
                if (!canBet(bet)) { bjResult.textContent = '❌ Not enough to double!'; return; }
                deduct(bet);
                bjBetAmount += bet;
                playerHand.push(deck.pop());
                renderBJ();
                bjDoubleBtn.disabled = true;
                if (handTotal(playerHand) > 21) { bjResult.textContent = '💥 BUST after double!';
                    endBJHand(); } else standBJ();
            }

            function endBJHand() {
                bjGameActive = false;
                bjDealBtn.disabled = false;
                bjHitBtn.disabled = true;
                bjStandBtn.disabled = true;
                bjDoubleBtn.disabled = true;
                renderBJ();
                dealerValueEl.textContent = handTotal(dealerHand);
            }
            bjDealBtn.addEventListener('click', dealBJ);
            bjHitBtn.addEventListener('click', hitBJ);
            bjStandBtn.addEventListener('click', standBJ);
            bjDoubleBtn.addEventListener('click', doubleBJ);
            resetBlackjack();

            // ================================================================
            //  ARCADE – 11 games
            // ================================================================
            const arcadeGrid = document.getElementById('arcadeGrid');
            const arcadeGameView = document.getElementById('arcadeGameView');
            const arcadeBackBtn = document.getElementById('arcadeBackBtn');
            const arcadeGameTitle = document.getElementById('arcadeGameTitle');
            const arcadeGameArea = document.getElementById('arcadeGameArea');
            const arcadeResult = document.getElementById('arcadeResult');
            const arcadeHistory = document.getElementById('arcadeHistory');

            const games = [{
                id: 'coinflip',
                name: 'Coin Flip',
                icon: '🪙',
                desc: 'Heads or Tails',
                play: function(bet, option) {
                    const result = Math.random() < 0.5 ? 'Heads' : 'Tails';
                    const win = (option === result) ? bet * 2 : 0;
                    return { result, win, detail: `Coin landed ${result}` };
                },
                options: ['Heads', 'Tails']
            }, {
                id: 'dice1',
                name: 'Dice Roll',
                icon: '🎲',
                desc: 'Guess 1-6',
                play: function(bet, option) {
                    const result = Math.floor(Math.random() * 6) + 1;
                    const win = (parseInt(option) === result) ? bet * 5 : 0;
                    return { result, win, detail: `Dice shows ${result}` };
                },
                options: ['1', '2', '3', '4', '5', '6']
            }, {
                id: 'dice2',
                name: 'Double Dice',
                icon: '🎲🎲',
                desc: 'Guess sum 2-12',
                play: function(bet, option) {
                    const d1 = Math.floor(Math.random() * 6) + 1,
                        d2 = Math.floor(Math.random() * 6) + 1;
                    const sum = d1 + d2;
                    const win = (parseInt(option) === sum) ? bet * 10 : 0;
                    return { result: sum, win, detail: `Dice: ${d1}+${d2}=${sum}` };
                },
                options: ['2', '3', '4', '5', '6', '7', '8', '9', '10', '11', '12']
            }, {
                id: 'luckynum',
                name: 'Lucky Number',
                icon: '🔮',
                desc: 'Pick 1-10',
                play: function(bet, option) {
                    const result = Math.floor(Math.random() * 10) + 1;
                    const win = (parseInt(option) === result) ? bet * 8 : 0;
                    return { result, win, detail: `Lucky number ${result}` };
                },
                options: ['1', '2', '3', '4', '5', '6', '7', '8', '9', '10']
            }, {
                id: 'colorpred',
                name: 'Color Prediction',
                icon: '🎨',
                desc: 'Red / Green / Blue',
                play: function(bet, option) {
                    const colors = ['Red', 'Green', 'Blue'];
                    const result = colors[Math.floor(Math.random() * colors.length)];
                    const win = (option === result) ? bet * 3 : 0;
                    return { result, win, detail: `Color is ${result}` };
                },
                options: ['Red', 'Green', 'Blue']
            }, {
                id: 'highlow',
                name: 'High-Low',
                icon: '⬆️⬇️',
                desc: 'High / Low / Equal 50',
                play: function(bet, option) {
                    const num = Math.floor(Math.random() * 100) + 1;
                    let win = 0;
                    if (option === 'High' && num > 50) win = bet * 2;
                    else if (option === 'Low' && num < 50) win = bet * 2;
                    else if (option === 'Equal' && num === 50) win = bet * 10;
                    return { result: num, win, detail: `Number is ${num}` };
                },
                options: ['High', 'Low', 'Equal']
            }, {
                id: 'rps',
                name: 'Rock Paper Scissors',
                icon: '✊✋✌️',
                desc: 'Beat the computer',
                play: function(bet, option) {
                    const choices = ['Rock', 'Paper', 'Scissors'];
                    const comp = choices[Math.floor(Math.random() * choices.length)];
                    let win = 0;
                    if ((option === 'Rock' && comp === 'Scissors') ||
                        (option === 'Paper' && comp === 'Rock') ||
                        (option === 'Scissors' && comp === 'Paper')) win = bet * 2;
                    else if (option === comp) win = bet;
                    return { result: comp, win, detail: `Computer chose ${comp}` };
                },
                options: ['Rock', 'Paper', 'Scissors']
            }, {
                id: 'keno',
                name: 'Keno',
                icon: '🎯',
                desc: 'Pick 1-20',
                play: function(bet, option) {
                    const drawn = Math.floor(Math.random() * 20) + 1;
                    const win = (parseInt(option) === drawn) ? bet * 15 : 0;
                    return { result: drawn, win, detail: `Drawn: ${drawn}` };
                },
                options: Array.from({ length: 20 }, (_, i) => (i + 1).toString())
            }, {
                id: 'wheel',
                name: 'Mini Wheel',
                icon: '🎡',
                desc: '8 segments',
                play: function(bet, option) {
                    const segments = ['1', '2', '3', '4', '5', '6', '7', '8'];
                    const result = segments[Math.floor(Math.random() * segments.length)];
                    const win = (option === result) ? bet * 6 : 0;
                    return { result, win, detail: `Wheel landed on ${result}` };
                },
                options: ['1', '2', '3', '4', '5', '6', '7', '8']
            }, {
                id: 'bingo',
                name: 'Bingo',
                icon: '🟡',
                desc: 'Pick 1-50',
                play: function(bet, option) {
                    const drawn = Math.floor(Math.random() * 50) + 1;
                    const win = (parseInt(option) === drawn) ? bet * 5 : 0;
                    return { result: drawn, win, detail: `Bingo: ${drawn}` };
                },
                options: Array.from({ length: 50 }, (_, i) => (i + 1).toString())
            }, {
                id: 'firstshot',
                name: '⚡ First Shot',
                icon: '🎯',
                desc: 'Odd/Even/Over/Under/5',
                play: function(bet, option) {
                    const num = Math.floor(Math.random() * 10);
                    let win = 0;
                    if (option === 'Odd' && num % 2 === 1) win = bet * 2;
                    else if (option === 'Even' && num % 2 === 0) win = bet * 2;
                    else if (option === 'Over' && num > 5) win = bet * 2;
                    else if (option === 'Under' && num < 5) win = bet * 2;
                    else if (option === '5' && num === 5) win = bet * 8;
                    return { result: num, win, detail: `Number is ${num}` };
                },
                options: ['Odd', 'Even', 'Over', 'Under', '5']
            }];

            function buildArcadeGrid() {
                arcadeGrid.innerHTML = '';
                games.forEach(g => {
                    const card = document.createElement('div');
                    card.className = 'game-card';
                    card.innerHTML =
                        `<div class="icon">${g.icon}</div><div class="name">${g.name}</div><div class="desc">${g.desc}</div>`;
                    card.addEventListener('click', () => openGame(g.id));
                    arcadeGrid.appendChild(card);
                });
            }
            buildArcadeGrid();

            let currentGame = null,
                selectedOption = null,
                gameHistory = [];

            function openGame(gameId) {
                const game = games.find(g => g.id === gameId);
                if (!game) return;
                currentGame = game;
                selectedOption = null;
                gameHistory = [];
                arcadeGrid.style.display = 'none';
                arcadeGameView.classList.add('active');
                arcadeGameTitle.textContent = game.icon + ' ' + game.name;
                let html =
                    `<div class="bet-ctrl"><label>Bet</label><input type="number" id="arcadeBet" value="10" min="1" step="1" /></div>`;
                html += `<div class="options">`;
                game.options.forEach(opt => {
                    html += `<button data-opt="${opt}" class="opt-btn">${opt}</button>`;
                });
                html += `</div><button class="play-btn" id="arcadePlayBtn">▶ Play</button>`;
                arcadeGameArea.innerHTML = html;

                const optBtns = arcadeGameArea.querySelectorAll('.opt-btn');
                optBtns.forEach(btn => {
                    btn.addEventListener('click', () => {
                        optBtns.forEach(b => b.classList.remove('selected'));
                        btn.classList.add('selected');
                        selectedOption = btn.dataset.opt;
                    });
                });
                const playBtn = document.getElementById('arcadePlayBtn');
                playBtn.addEventListener('click', playArcadeGame);
                arcadeResult.textContent = '';
                arcadeHistory.textContent = '';
            }

            function playArcadeGame() {
                if (!currentGame) return;
                if (!selectedOption) { arcadeResult.textContent = '⚠️ Select an option!'; return; }
                const betInput = document.getElementById('arcadeBet');
                const bet = parseInt(betInput.value, 10) || 10;
                if (!canBet(bet)) { arcadeResult.textContent = '❌ Insufficient balance!'; return; }
                if (!deduct(bet)) return;

                const result = currentGame.play(bet, selectedOption);
                let msg = result.detail + ' — ';
                if (result.win > 0) {
                    add(result.win);
                    msg += `🎉 You win ₹${result.win.toLocaleString()}!`;
                } else {
                    msg += `😔 You lose.`;
                }
                arcadeResult.innerHTML = msg + ` (Balance: ₹${balance.toLocaleString()})`;
                gameHistory.push({ option: selectedOption, result: result.result, win: result.win });
                if (gameHistory.length > 5) gameHistory.shift();
                arcadeHistory.textContent = 'History: ' + gameHistory.map(h =>
                    `${h.option}→${h.result}${h.win>0?'✅':'❌'}`).join(' | ');
            }

            arcadeBackBtn.addEventListener('click', () => {
                arcadeGameView.classList.remove('active');
                arcadeGrid.style.display = 'grid';
                arcadeResult.textContent = '';
                arcadeHistory.textContent = '';
            });

            // ================================================================
            //  KEYBOARD SHORTCUTS
            // ================================================================
            document.querySelectorAll('input[type="number"]').forEach(inp => {
                inp.addEventListener('keydown', (e) => {
                    if (e.key === 'Enter') {
                        const panel = inp.closest('.game-panel');
                        if (panel) {
                            if (panel.id === 'panel-slots') spinSlots();
                            else if (panel.id === 'panel-roulette') spinRoulette();
                            else if (panel.id === 'panel-blackjack') dealBJ();
                            else if (panel.id === 'panel-arcade') {
                                const playBtn = document.getElementById('arcadePlayBtn');
                                if (playBtn) playBtn.click();
                            }
                        }
                    }
                });
            });

            // ================================================================
            //  INIT
            // ================================================================
            updateBalance();
            resetSlots();
            resetRoulette();
            renderTransactions();
            console.log('🎰 Jannat Games – Premium UI with social links loaded!');
        })();
    </script>

</body>
</html>
