[nba-bets.html](https://github.com/user-attachments/files/26226917/nba-bets.html)
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0, viewport-fit=cover">
  <meta name="apple-mobile-web-app-capable" content="yes">
  <meta name="apple-mobile-web-app-status-bar-style" content="black-translucent">
  <meta name="apple-mobile-web-app-title" content="NBA Bets">
  <title>NBA Daily Bets</title>
  <style>
    *, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }

    :root {
      --green:  #30D158;
      --yellow: #FFD60A;
      --red:    #FF453A;
      --orange: #FF9F0A;
      --bg:     #08080F;
      --card:   rgba(255,255,255,0.04);
      --border: rgba(255,255,255,0.08);
      --text:   #ffffff;
      --dim:    rgba(255,255,255,0.35);
      --muted:  rgba(255,255,255,0.2);
    }

    html, body {
      width: 100%; height: 100%;
      overflow: hidden;
      background: #000;
      font-family: -apple-system, BlinkMacSystemFont, 'SF Pro Display', 'Helvetica Neue', sans-serif;
      color: var(--text);
      -webkit-font-smoothing: antialiased;
      -webkit-text-size-adjust: 100%;
    }

    /* ── App shell ──────────────────────────────────────────────────── */
    #app {
      position: relative;
      width: 100%;
      max-width: 393px;
      height: 100dvh;
      margin: 0 auto;
      background: var(--bg);
      display: flex;
      flex-direction: column;
      overflow: hidden;
    }

    /* ── Dynamic Island ─────────────────────────────────────────────── */
    #di {
      position: absolute;
      top: 13px;
      left: 50%;
      transform: translateX(-50%);
      width: 126px;
      height: 37px;
      background: #000;
      border-radius: 99px;
      z-index: 999;
      pointer-events: none;
      box-shadow: 0 0 0 1.5px rgba(255,255,255,0.07);
    }

    /* ── Safe-area spacer (Dynamic Island + gap) ──────────────────── */
    #safe-top {
      flex-shrink: 0;
      height: max(env(safe-area-inset-top, 59px), 59px);
    }

    /* ── Header ─────────────────────────────────────────────────────── */
    #header {
      flex-shrink: 0;
      display: flex;
      justify-content: space-between;
      align-items: flex-end;
      padding: 6px 22px 18px;
    }

    .eyebrow {
      font-size: 10px;
      font-weight: 700;
      letter-spacing: 1.8px;
      color: var(--muted);
      margin-bottom: 5px;
    }

    h1 {
      font-size: 27px;
      font-weight: 800;
      letter-spacing: -0.7px;
      line-height: 1;
    }

    .grad {
      background: linear-gradient(120deg, var(--green) 0%, var(--yellow) 100%);
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
      background-clip: text;
    }

    .date-card {
      flex-shrink: 0;
      background: rgba(255,255,255,0.05);
      border: 1px solid rgba(255,255,255,0.09);
      border-radius: 14px;
      padding: 9px 14px;
      display: flex;
      flex-direction: column;
      align-items: center;
      gap: 2px;
    }

    .date-card span { display: block; text-align: center; }
    .d-date  { font-size: 10px; font-weight: 700; letter-spacing: 1px; color: var(--muted); }
    .d-games { font-size: 12px; font-weight: 600; color: var(--text); }
    .d-upd   { font-size: 9px; color: rgba(255,255,255,0.22); }

    /* ── Scroll area ─────────────────────────────────────────────────── */
    #content {
      flex: 1;
      overflow-y: auto;
      overflow-x: hidden;
      padding: 4px 16px 12px;
      -webkit-overflow-scrolling: touch;
    }

    .sec-label {
      font-size: 10px;
      font-weight: 700;
      letter-spacing: 1.4px;
      color: var(--muted);
      text-transform: uppercase;
      margin-bottom: 12px;
      padding-left: 2px;
    }

    /* ── Bet cards ───────────────────────────────────────────────────── */
    .bet-card {
      background: var(--card);
      border: 1px solid var(--border);
      border-radius: 22px;
      padding: 20px 20px 14px;
      margin-bottom: 12px;
      cursor: pointer;
      transition: background .3s ease, border-color .3s ease;
      -webkit-tap-highlight-color: transparent;
      user-select: none;
    }

    .bc-top {
      display: flex;
      justify-content: space-between;
      align-items: center;
    }

    .bc-left {
      display: flex;
      align-items: center;
      gap: 8px;
    }

    .badge {
      border-radius: 7px;
      padding: 3px 9px;
      font-size: 10px;
      font-weight: 800;
      letter-spacing: 1.5px;
    }

    .risk-lbl { font-size: 12px; color: var(--dim); }

    .odds-pill {
      border-radius: 11px;
      padding: 5px 14px;
      font-size: 15px;
      font-weight: 800;
      letter-spacing: 0.2px;
    }

    .bc-body { margin-top: 16px; }

    .type-lbl {
      font-size: 10px;
      font-weight: 700;
      letter-spacing: 1.3px;
      color: rgba(255,255,255,0.27);
      text-transform: uppercase;
      margin-bottom: 4px;
    }

    .pick { font-size: 19px; font-weight: 700; letter-spacing: -0.3px; line-height: 1.25; }

    /* confidence bar */
    .conf-wrap { margin-top: 14px; }

    .conf-row {
      display: flex;
      justify-content: space-between;
      align-items: center;
      margin-bottom: 6px;
    }

    .conf-title { font-size: 10px; font-weight: 700; letter-spacing: 1.2px; color: rgba(255,255,255,0.27); text-transform: uppercase; }
    .conf-pct   { font-size: 10px; font-weight: 700; }

    .conf-track {
      background: rgba(255,255,255,0.06);
      border-radius: 99px;
      height: 4px;
      overflow: hidden;
    }

    .conf-fill {
      height: 100%;
      border-radius: 99px;
      width: 0;
      transition: width 1.1s cubic-bezier(.4,0,.2,1);
    }

    /* expanded */
    .bc-exp {
      display: none;
      margin-top: 16px;
      padding-top: 16px;
      border-top: 1px solid rgba(255,255,255,0.07);
    }

    .bc-exp.open { display: block; }

    .bc-reason {
      font-size: 13px;
      line-height: 1.75;
      color: rgba(255,255,255,0.55);
      margin-bottom: 14px;
    }

    .tags { display: flex; flex-wrap: wrap; gap: 7px; }

    .tag {
      background: rgba(255,255,255,0.05);
      border: 1px solid rgba(255,255,255,0.09);
      border-radius: 99px;
      padding: 3px 11px;
      font-size: 11px;
      color: rgba(255,255,255,0.4);
    }

    .toggle-hint {
      text-align: center;
      margin-top: 13px;
      font-size: 10px;
      letter-spacing: 1px;
      color: rgba(255,255,255,0.18);
    }

    /* disclaimer */
    .disclaimer {
      background: rgba(255,255,255,0.02);
      border: 1px solid rgba(255,255,255,0.05);
      border-radius: 16px;
      padding: 13px 16px;
      margin-top: 4px;
      text-align: center;
    }

    .disclaimer p {
      font-size: 10px;
      line-height: 1.65;
      color: rgba(255,255,255,0.2);
      letter-spacing: 0.3px;
    }

    /* ── Prop cards ──────────────────────────────────────────────────── */
    .prop-card {
      background: var(--card);
      border: 1px solid var(--border);
      border-radius: 20px;
      padding: 16px 18px;
      margin-bottom: 11px;
      display: flex;
      justify-content: space-between;
      align-items: center;
      gap: 14px;
    }

    .prop-left { flex: 1; min-width: 0; }

    .prop-meta {
      display: flex;
      align-items: center;
      gap: 8px;
      margin-bottom: 5px;
    }

    .prop-team { font-size: 11px; color: var(--dim); }
    .prop-player { font-size: 16px; font-weight: 700; letter-spacing: -0.2px; }
    .prop-line { font-size: 13px; font-weight: 600; margin-top: 3px; }
    .prop-note { font-size: 11px; line-height: 1.55; color: rgba(255,255,255,0.35); margin-top: 7px; }

    .prop-odds {
      flex-shrink: 0;
      border-radius: 12px;
      padding: 7px 13px;
      font-size: 15px;
      font-weight: 800;
      white-space: nowrap;
    }

    .combo-box {
      border-radius: 20px;
      padding: 16px 18px;
      margin-top: 4px;
    }

    .combo-label { font-size: 11px; font-weight: 700; letter-spacing: 1px; margin-bottom: 6px; }
    .combo-pick  { font-size: 14px; font-weight: 700; }
    .combo-note  { font-size: 12px; margin-top: 5px; line-height: 1.5; color: rgba(255,255,255,0.4); }

    /* ── Game cards ──────────────────────────────────────────────────── */
    .game-card {
      background: var(--card);
      border: 1px solid var(--border);
      border-radius: 20px;
      padding: 15px 18px;
      margin-bottom: 10px;
    }

    .gc-top {
      display: flex;
      justify-content: space-between;
      align-items: center;
      margin-bottom: 12px;
    }

    .gc-time { display: flex; align-items: center; gap: 7px; }

    .status-dot {
      width: 7px;
      height: 7px;
      border-radius: 50%;
      flex-shrink: 0;
    }

    .time-lbl { font-size: 11px; color: var(--dim); letter-spacing: 0.2px; }

    .pick-badge {
      background: rgba(48,209,88,0.11);
      border: 1px solid rgba(48,209,88,0.25);
      border-radius: 8px;
      padding: 2px 10px;
      font-size: 10px;
      font-weight: 700;
      letter-spacing: 0.4px;
      color: var(--green);
    }

    .gc-teams {
      display: flex;
      align-items: center;
      justify-content: space-between;
    }

    .team-col { flex: 1; }
    .team-col.right { text-align: right; }

    .team-abbr  { font-size: 18px; font-weight: 800; letter-spacing: -0.3px; }
    .team-rec   { font-size: 11px; color: var(--muted); margin-top: 2px; }
    .team-score { font-size: 24px; font-weight: 800; color: rgba(255,255,255,0.6); margin-top: 2px; }

    .vs-col { flex-shrink: 0; padding: 0 10px; text-align: center; }
    .vs-text { font-size: 12px; font-weight: 600; color: rgba(255,255,255,0.15); letter-spacing: 0.5px; }
    .et-time { font-size: 10px; color: rgba(255,255,255,0.18); margin-top: 4px; }

    .gc-channel { margin-top: 10px; font-size: 10px; color: rgba(255,255,255,0.2); }

    .result-gap { margin-top: 18px; margin-bottom: 12px; }

    /* ── Tab bar ─────────────────────────────────────────────────────── */
    #tab-bar {
      flex-shrink: 0;
      display: flex;
      justify-content: space-evenly;
      align-items: flex-start;
      background: rgba(10,10,20,0.96);
      border-top: 1px solid rgba(255,255,255,0.07);
      -webkit-backdrop-filter: blur(20px);
      backdrop-filter: blur(20px);
      padding-top: 10px;
      padding-bottom: calc(10px + env(safe-area-inset-bottom, 28px));
    }

    .tab-btn {
      flex: 1;
      background: none;
      border: none;
      cursor: pointer;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: flex-start;
      gap: 4px;
      padding: 4px 0;
      -webkit-tap-highlight-color: transparent;
      user-select: none;
    }

    .tab-icon { width: 24px; height: 24px; display: flex; align-items: center; justify-content: center; }
    .tab-icon svg { width: 22px; height: 22px; }

    .tab-lbl {
      font-size: 10px;
      font-weight: 500;
      letter-spacing: 0.4px;
      color: rgba(255,255,255,0.3);
      transition: color .2s, font-weight .2s;
    }

    .tab-dot {
      width: 4px; height: 4px;
      border-radius: 50%;
      background: var(--green);
      opacity: 0;
      transition: opacity .2s;
      margin-top: -2px;
    }

    .tab-btn.active .tab-lbl { color: #fff; font-weight: 700; }
    .tab-btn.active .tab-dot { opacity: 1; }

    /* ── Tab content visibility ─────────────────────────────────────── */
    .tab-pane { display: none; }
    .tab-pane.active { display: block; }
  </style>
</head>
<body>
<div id="app">

  <!-- Dynamic Island -->
  <div id="di"></div>

  <!-- Safe-area spacer -->
  <div id="safe-top"></div>

  <!-- Header -->
  <div id="header">
    <div>
      <div class="eyebrow">NBA DAILY PICKS</div>
      <h1>Today's <span class="grad">Bets</span></h1>
    </div>
    <div class="date-card">
      <span class="d-date" id="js-date"></span>
      <span class="d-games">🏀 4 Games</span>
      <span class="d-upd">↻ 06:00 CET</span>
    </div>
  </div>

  <!-- Scrollable content -->
  <div id="content">

    <!-- ══ BETS TAB ══════════════════════════════════════════════════ -->
    <div id="pane-bets" class="tab-pane active">
      <div class="sec-label">Tap card for full analysis</div>

      <!-- LOW -->
      <div class="bet-card" id="bc-low" onclick="toggle('low')">
        <div class="bc-top">
          <div class="bc-left">
            <div class="badge" style="background:rgba(48,209,88,.13);border:1px solid rgba(48,209,88,.32);color:#30D158">LOW</div>
            <span class="risk-lbl">Safe Play</span>
          </div>
          <div class="odds-pill" style="background:rgba(48,209,88,.12);border:1px solid rgba(48,209,88,.28);color:#30D158">-115</div>
        </div>
        <div class="bc-body">
          <div class="type-lbl">Point Spread · CHA vs SAC</div>
          <div class="pick">Charlotte Hornets -17</div>
        </div>
        <div class="conf-wrap">
          <div class="conf-row">
            <span class="conf-title">Confidence</span>
            <span class="conf-pct" style="color:#30D158">88%</span>
          </div>
          <div class="conf-track"><div class="conf-fill" id="fill-low" style="background:#30D158"></div></div>
        </div>
        <div class="bc-exp" id="exp-low">
          <p class="bc-reason">Sacramento missing 3 starters (Sabonis, LaVine, Hunter — all season-ending). Charlotte averaging +24 margin over last 3 wins. Kings bottom-3 defence in the league. Total structural mismatch tonight.</p>
          <div class="tags">
            <span class="tag">Injury Edge</span>
            <span class="tag">Home Favourite</span>
            <span class="tag">Form</span>
          </div>
        </div>
        <div class="toggle-hint" id="hint-low">▼ &nbsp;ANALYSIS</div>
      </div>

      <!-- MID -->
      <div class="bet-card" id="bc-mid" onclick="toggle('mid')">
        <div class="bc-top">
          <div class="bc-left">
            <div class="badge" style="background:rgba(255,214,10,.13);border:1px solid rgba(255,214,10,.32);color:#FFD60A">MID</div>
            <span class="risk-lbl">Value Pick</span>
          </div>
          <div class="odds-pill" style="background:rgba(255,214,10,.12);border:1px solid rgba(255,214,10,.28);color:#FFD60A">-110</div>
        </div>
        <div class="bc-body">
          <div class="type-lbl">ATS Underdog · NOP vs NYK</div>
          <div class="pick">New Orleans Pelicans +8.5</div>
        </div>
        <div class="conf-wrap">
          <div class="conf-row">
            <span class="conf-title">Confidence</span>
            <span class="conf-pct" style="color:#FFD60A">73%</span>
          </div>
          <div class="conf-track"><div class="conf-fill" id="fill-mid" style="background:#FFD60A"></div></div>
        </div>
        <div class="bc-exp" id="exp-mid">
          <p class="bc-reason">Pelicans are 13-7 ATS as 9+ pt underdogs. No 2026 draft pick to protect — they play hard every night. Top-10 net rating over last 10 games. Knicks only 11-7-1 ATS as heavy favourites.</p>
          <div class="tags">
            <span class="tag">ATS Value</span>
            <span class="tag">Motivated Side</span>
            <span class="tag">Sharp Lean</span>
          </div>
        </div>
        <div class="toggle-hint" id="hint-mid">▼ &nbsp;ANALYSIS</div>
      </div>

      <!-- HIGH -->
      <div class="bet-card" id="bc-high" onclick="toggle('high')">
        <div class="bc-top">
          <div class="bc-left">
            <div class="badge" style="background:rgba(255,69,58,.13);border:1px solid rgba(255,69,58,.32);color:#FF453A">HIGH</div>
            <span class="risk-lbl">3-Leg Parlay</span>
          </div>
          <div class="odds-pill" style="background:rgba(255,69,58,.12);border:1px solid rgba(255,69,58,.28);color:#FF453A">+480</div>
        </div>
        <div class="bc-body">
          <div class="type-lbl">Parlay · 3 Games</div>
          <div class="pick">Hornets -17 + Cavs ML + Nuggets -5.5</div>
        </div>
        <div class="conf-wrap">
          <div class="conf-row">
            <span class="conf-title">Confidence</span>
            <span class="conf-pct" style="color:#FF453A">51%</span>
          </div>
          <div class="conf-track"><div class="conf-fill" id="fill-high" style="background:#FF453A"></div></div>
        </div>
        <div class="bc-exp" id="exp-high">
          <p class="bc-reason">Charlotte dismantles depleted Kings. Cavs with Mitchell + Harden vs Magic on 5-game losing streak. Jamal Murray (31 pts last game, 24.1 PPG in March) leads Nuggets vs a slumping Suns side.</p>
          <div class="tags">
            <span class="tag">High Reward</span>
            <span class="tag">3 Favourites</span>
            <span class="tag">Murray Form</span>
          </div>
        </div>
        <div class="toggle-hint" id="hint-high">▼ &nbsp;ANALYSIS</div>
      </div>

      <div class="disclaimer">
        <p>For entertainment only · Bet responsibly · Max 2–5% bankroll per stake</p>
      </div>
    </div>

    <!-- ══ PROPS TAB ═════════════════════════════════════════════════ -->
    <div id="pane-props" class="tab-pane">
      <div class="sec-label">Tonight's top player props</div>

      <div class="prop-card">
        <div class="prop-left">
          <div class="prop-meta">
            <div class="badge" style="background:rgba(48,209,88,.13);border:1px solid rgba(48,209,88,.32);color:#30D158">LOW</div>
            <span class="prop-team">CHA Hornets</span>
          </div>
          <div class="prop-player">LaMelo Ball</div>
          <div class="prop-line" style="color:#30D158">Over 7.5 Assists</div>
          <div class="prop-note">Kings can't guard multiple actions. LaMelo avg 7.1 ast/g — line is undervalued vs this defence.</div>
        </div>
        <div class="prop-odds" style="background:rgba(48,209,88,.12);border:1px solid rgba(48,209,88,.28);color:#30D158">-118</div>
      </div>

      <div class="prop-card">
        <div class="prop-left">
          <div class="prop-meta">
            <div class="badge" style="background:rgba(255,214,10,.13);border:1px solid rgba(255,214,10,.32);color:#FFD60A">MID</div>
            <span class="prop-team">CLE Cavaliers</span>
          </div>
          <div class="prop-player">Evan Mobley</div>
          <div class="prop-line" style="color:#FFD60A">Over 5.5 Rebounds</div>
          <div class="prop-note">Jarrett Allen OUT (knee). Mobley is Cleveland's only big tonight — sole presence on the glass.</div>
        </div>
        <div class="prop-odds" style="background:rgba(255,214,10,.12);border:1px solid rgba(255,214,10,.28);color:#FFD60A">+114</div>
      </div>

      <div class="prop-card">
        <div class="prop-left">
          <div class="prop-meta">
            <div class="badge" style="background:rgba(255,159,10,.13);border:1px solid rgba(255,159,10,.32);color:#FF9F0A">MID</div>
            <span class="prop-team">DEN Nuggets</span>
          </div>
          <div class="prop-player">Jamal Murray</div>
          <div class="prop-line" style="color:#FF9F0A">Over Points — check line</div>
          <div class="prop-note">31 pts last game. 24.1 PPG in March. The hottest scorer in the West right now.</div>
        </div>
        <div class="prop-odds" style="background:rgba(255,159,10,.12);border:1px solid rgba(255,159,10,.28);color:#FF9F0A">~-115</div>
      </div>

      <div class="combo-box" style="background:rgba(48,209,88,.06);border:1px solid rgba(48,209,88,.18)">
        <div class="combo-label" style="color:#30D158">💡 SAFE PROP COMBO</div>
        <div class="combo-pick">LaMelo Ast 7.5+ & Mobley Reb 5.5+</div>
        <div class="combo-note">Both backed by concrete structural reasons tonight. Clean logic, clean combo.</div>
      </div>
    </div>

    <!-- ══ SCHEDULE TAB ══════════════════════════════════════════════ -->
    <div id="pane-schedule" class="tab-pane">
      <div class="sec-label">🟡 Upcoming · Mar 24</div>

      <!-- Game 1 -->
      <div class="game-card">
        <div class="gc-top">
          <div class="gc-time">
            <div class="status-dot" style="background:#FFD60A;box-shadow:0 0 6px rgba(255,214,10,.55)"></div>
            <span class="time-lbl">01:00 CET</span>
          </div>
          <div class="pick-badge">OUR PICK: CHA -17</div>
        </div>
        <div class="gc-teams">
          <div class="team-col">
            <div class="team-abbr">SAC</div>
            <div class="team-rec">19–53</div>
          </div>
          <div class="vs-col">
            <div class="vs-text">vs</div>
            <div class="et-time">7:00 PM ET</div>
          </div>
          <div class="team-col right">
            <div class="team-abbr">CHA</div>
            <div class="team-rec">37–34</div>
          </div>
        </div>
        <div class="gc-channel">📺 FDSSE</div>
      </div>

      <!-- Game 2 -->
      <div class="game-card">
        <div class="gc-top">
          <div class="gc-time">
            <div class="status-dot" style="background:#FFD60A;box-shadow:0 0 6px rgba(255,214,10,.55)"></div>
            <span class="time-lbl">01:30 CET</span>
          </div>
          <div class="pick-badge">OUR PICK: NOP +8.5</div>
        </div>
        <div class="gc-teams">
          <div class="team-col">
            <div class="team-abbr">NOP</div>
            <div class="team-rec">25–47</div>
          </div>
          <div class="vs-col">
            <div class="vs-text">vs</div>
            <div class="et-time">7:30 PM ET</div>
          </div>
          <div class="team-col right">
            <div class="team-abbr">NYK</div>
            <div class="team-rec">47–25</div>
          </div>
        </div>
        <div class="gc-channel">📺 MSG</div>
      </div>

      <!-- Game 3 -->
      <div class="game-card">
        <div class="gc-top">
          <div class="gc-time">
            <div class="status-dot" style="background:#FFD60A;box-shadow:0 0 6px rgba(255,214,10,.55)"></div>
            <span class="time-lbl">02:00 CET</span>
          </div>
          <div class="pick-badge">OUR PICK: CLE ML</div>
        </div>
        <div class="gc-teams">
          <div class="team-col">
            <div class="team-abbr">ORL</div>
            <div class="team-rec">38–33</div>
          </div>
          <div class="vs-col">
            <div class="vs-text">vs</div>
            <div class="et-time">8:00 PM ET</div>
          </div>
          <div class="team-col right">
            <div class="team-abbr">CLE</div>
            <div class="team-rec">44–27</div>
          </div>
        </div>
        <div class="gc-channel">📺 Bally Sports</div>
      </div>

      <!-- Game 4 -->
      <div class="game-card">
        <div class="gc-top">
          <div class="gc-time">
            <div class="status-dot" style="background:#FFD60A;box-shadow:0 0 6px rgba(255,214,10,.55)"></div>
            <span class="time-lbl">05:00 CET</span>
          </div>
          <div class="pick-badge">OUR PICK: DEN -5.5</div>
        </div>
        <div class="gc-teams">
          <div class="team-col">
            <div class="team-abbr">DEN</div>
            <div class="team-rec">44–28</div>
          </div>
          <div class="vs-col">
            <div class="vs-text">vs</div>
            <div class="et-time">11:00 PM ET</div>
          </div>
          <div class="team-col right">
            <div class="team-abbr">PHX</div>
            <div class="team-rec">40–32</div>
          </div>
        </div>
        <div class="gc-channel">📺 NBC / Peacock</div>
      </div>

      <!-- Recent results -->
      <div class="sec-label result-gap">🟢 Recent Results</div>

      <div class="game-card">
        <div class="gc-top">
          <div class="gc-time">
            <div class="status-dot" style="background:#30D158;box-shadow:0 0 6px rgba(48,209,88,.55)"></div>
            <span class="time-lbl">Final · Mar 20</span>
          </div>
        </div>
        <div class="gc-teams">
          <div class="team-col"><div class="team-abbr">TOR</div><div class="team-score">115</div></div>
          <div class="vs-col"><div class="vs-text">—</div></div>
          <div class="team-col right"><div class="team-abbr">DEN</div><div class="team-score">121</div></div>
        </div>
      </div>

      <div class="game-card">
        <div class="gc-top">
          <div class="gc-time">
            <div class="status-dot" style="background:#30D158;box-shadow:0 0 6px rgba(48,209,88,.55)"></div>
            <span class="time-lbl">Final · Mar 20</span>
          </div>
        </div>
        <div class="gc-teams">
          <div class="team-col"><div class="team-abbr">ATL</div><div class="team-score">95</div></div>
          <div class="vs-col"><div class="vs-text">—</div></div>
          <div class="team-col right"><div class="team-abbr">HOU</div><div class="team-score">117</div></div>
        </div>
      </div>

      <div class="game-card">
        <div class="gc-top">
          <div class="gc-time">
            <div class="status-dot" style="background:#30D158;box-shadow:0 0 6px rgba(48,209,88,.55)"></div>
            <span class="time-lbl">Final · Mar 12</span>
          </div>
        </div>
        <div class="gc-teams">
          <div class="team-col"><div class="team-abbr">CHI</div><div class="team-score">130</div></div>
          <div class="vs-col"><div class="vs-text">—</div></div>
          <div class="team-col right"><div class="team-abbr">LAL</div><div class="team-score">142</div></div>
        </div>
      </div>

    </div>
  </div><!-- /content -->

  <!-- ══ TAB BAR ════════════════════════════════════════════════════ -->
  <div id="tab-bar">

    <button class="tab-btn active" id="tb-bets" onclick="switchTab('bets')">
      <div class="tab-icon">
        <svg id="ti-bets" viewBox="0 0 24 24" fill="none" stroke="#fff" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
          <rect x="2" y="7" width="20" height="14" rx="3"/>
          <path d="M16 7V5a2 2 0 0 0-4 0v2M8 7V5a2 2 0 0 0-4 0v2"/>
          <line x1="12" y1="12" x2="12" y2="16"/><line x1="10" y1="14" x2="14" y2="14"/>
        </svg>
      </div>
      <span class="tab-lbl" id="tl-bets">Bets</span>
      <div class="tab-dot" id="td-bets" style="opacity:1"></div>
    </button>

    <button class="tab-btn" id="tb-props" onclick="switchTab('props')">
      <div class="tab-icon">
        <svg id="ti-props" viewBox="0 0 24 24" fill="none" stroke="rgba(255,255,255,.3)" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
          <circle cx="12" cy="8" r="4"/>
          <path d="M6 20v-2a6 6 0 0 1 12 0v2"/>
        </svg>
      </div>
      <span class="tab-lbl" id="tl-props">Props</span>
      <div class="tab-dot" id="td-props"></div>
    </button>

    <button class="tab-btn" id="tb-schedule" onclick="switchTab('schedule')">
      <div class="tab-icon">
        <svg id="ti-schedule" viewBox="0 0 24 24" fill="none" stroke="rgba(255,255,255,.3)" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
          <rect x="3" y="4" width="18" height="18" rx="2"/>
          <line x1="16" y1="2" x2="16" y2="6"/><line x1="8" y1="2" x2="8" y2="6"/>
          <line x1="3" y1="10" x2="21" y2="10"/>
        </svg>
      </div>
      <span class="tab-lbl" id="tl-schedule">Schedule</span>
      <div class="tab-dot" id="td-schedule"></div>
    </button>

  </div>
</div><!-- /app -->

<script>
  // ── Date ──────────────────────────────────────────────────────────
  document.getElementById('js-date').textContent =
    new Date().toLocaleDateString('en-US',{month:'short',day:'numeric'}).toUpperCase();

  // ── Tab switching ─────────────────────────────────────────────────
  const TABS = ['bets','props','schedule'];

  function switchTab(id) {
    TABS.forEach(t => {
      document.getElementById('pane-'+t).classList.remove('active');
      document.getElementById('tb-'+t).classList.remove('active');
      document.getElementById('ti-'+t).setAttribute('stroke','rgba(255,255,255,.3)');
      document.getElementById('td-'+t).style.opacity = '0';
    });
    document.getElementById('pane-'+id).classList.add('active');
    document.getElementById('tb-'+id).classList.add('active');
    document.getElementById('ti-'+id).setAttribute('stroke','#fff');
    document.getElementById('td-'+id).style.opacity = '1';
    document.getElementById('content').scrollTop = 0;
  }

  // ── Card toggle ───────────────────────────────────────────────────
  const colors = {low:'#30D158', mid:'#FFD60A', high:'#FF453A'};
  const pcts   = {low:88, mid:73, high:51};
  const state  = {low:false, mid:false, high:false};

  function toggle(id) {
    const card = document.getElementById('bc-'+id);
    const exp  = document.getElementById('exp-'+id);
    const hint = document.getElementById('hint-'+id);
    state[id] = !state[id];

    if (state[id]) {
      card.style.background   = colors[id]+'0D';
      card.style.borderColor  = colors[id]+'38';
      exp.classList.add('open');
      hint.textContent = '▲ \u00a0COLLAPSE';
    } else {
      card.style.background   = 'var(--card)';
      card.style.borderColor  = 'var(--border)';
      exp.classList.remove('open');
      hint.textContent = '▼ \u00a0ANALYSIS';
    }
  }

  // ── Animate confidence bars on load ──────────────────────────────
  window.addEventListener('load', () => {
    setTimeout(() => {
      ['low','mid','high'].forEach(id => {
        document.getElementById('fill-'+id).style.width = pcts[id]+'%';
      });
    }, 250);
  });
</script>
</body>
</html>
