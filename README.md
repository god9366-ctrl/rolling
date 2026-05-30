<!DOCTYPE html>
<html lang="ko">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>김상윤 실장님 퇴임 기념</title>
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Noto+Sans+KR:wght@300;400;500;700&family=Noto+Serif+KR:wght@400;600&display=swap" rel="stylesheet">
  <style>
    *, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }
    :root {
      --warm-100: #FDF6EE;
      --warm-200: #FAF0E8;
      --warm-300: #F5E4D0;
      --warm-400: #D4A070;
      --warm-500: #B8825A;
      --warm-600: #7A4F2C;
      --text-primary: #2C2018;
      --text-secondary: #7A6555;
      --text-muted: #A89585;
      --border: rgba(180,140,100,0.2);
      --border-hover: rgba(180,140,100,0.4);
      --white: #FFFFFF;
      --shadow: 0 2px 16px rgba(120,80,40,0.08);
      --shadow-hover: 0 4px 24px rgba(120,80,40,0.14);
    }
    body {
      font-family: 'Noto Sans KR', sans-serif;
      background: var(--warm-100);
      color: var(--text-primary);
      min-height: 100vh;
    }
    .hero {
      text-align: center;
      padding: 4rem 2rem 3rem;
      position: relative;
      overflow: hidden;
    }
    .hero::before {
      content: '';
      position: absolute;
      top: -60px; left: 50%;
      transform: translateX(-50%);
      width: 500px; height: 300px;
      background: radial-gradient(ellipse, rgba(212,160,112,0.12) 0%, transparent 70%);
      pointer-events: none;
    }
    .hero-petal {
      font-size: 2.2rem;
      display: block;
      margin-bottom: 1rem;
      animation: float 3s ease-in-out infinite;
    }
    @keyframes float {
      0%, 100% { transform: translateY(0); }
      50% { transform: translateY(-6px); }
    }
    .hero-badge {
      display: inline-block;
      background: var(--warm-300);
      color: var(--warm-600);
      font-size: 11px;
      font-weight: 500;
      padding: 5px 16px;
      border-radius: 20px;
      letter-spacing: 0.08em;
      margin-bottom: 1.2rem;
    }
    .hero h1 {
      font-family: 'Noto Serif KR', serif;
      font-size: clamp(24px, 5vw, 34px);
      font-weight: 600;
      color: var(--text-primary);
      margin-bottom: 0.8rem;
      line-height: 1.3;
    }
    .hero .subtitle {
      font-size: 14px;
      color: var(--text-secondary);
      line-height: 1.8;
      max-width: 480px;
      margin: 0 auto;
    }
    .hero-divider {
      width: 48px; height: 1.5px;
      background: var(--warm-400);
      margin: 1.8rem auto 0;
      border-radius: 2px;
      opacity: 0.6;
    }
    .toolbar {
      display: flex;
      align-items: center;
      justify-content: space-between;
      padding: 1rem 2rem;
      background: rgba(255,255,255,0.7);
      backdrop-filter: blur(8px);
      border-top: 1px solid var(--border);
      border-bottom: 1px solid var(--border);
      flex-wrap: wrap;
      gap: 0.75rem;
      position: sticky;
      top: 0;
      z-index: 50;
    }
    .tabs { display: flex; align-items: center; gap: 6px; flex-wrap: wrap; }
    .tab {
      font-size: 12px;
      font-weight: 400;
      padding: 5px 14px;
      border-radius: 20px;
      border: 1px solid var(--border-hover);
      background: transparent;
      color: var(--text-secondary);
      cursor: pointer;
      transition: all 0.18s;
      font-family: 'Noto Sans KR', sans-serif;
    }
    .tab:hover { background: var(--warm-200); color: var(--warm-600); }
    .tab.active { background: var(--warm-400); color: #fff; border-color: var(--warm-400); font-weight: 500; }
    .count-badge { font-size: 12px; color: var(--text-muted); margin-left: 4px; }
    .cards-grid {
      display: grid;
      grid-template-columns: repeat(auto-fill, minmax(200px, 1fr));
      gap: 16px;
      padding: 2rem;
      max-width: 1100px;
      margin: 0 auto;
    }
    .msg-card {
      background: var(--white);
      border: 1px solid var(--border);
      border-radius: 16px;
      padding
