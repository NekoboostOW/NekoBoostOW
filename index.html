<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Overwatch Rank Boost</title>
  <style>
    @import url('https://fonts.googleapis.com/css2?family=Rajdhani:wght@500;700&family=Inter:wght@400;500&display=swap');

    :root {
      --orange: #ff9800;
      --bg: #0e0e0e;
      --surface: #1a1a1a;
      --border: #2a2a2a;
      --text: #e0e0e0;
      --muted: #777;
      --green: #4caf50;
    }

    *, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }

    body {
      font-family: 'Inter', sans-serif;
      background: var(--bg);
      color: var(--text);
      min-height: 100vh;
      display: flex;
      align-items: center;
      justify-content: center;
      padding: 24px;
    }

    .card {
      background: var(--surface);
      border: 1px solid var(--border);
      border-radius: 12px;
      padding: 32px;
      width: 100%;
      max-width: 480px;
    }

    h1 {
      font-family: 'Rajdhani', sans-serif;
      font-size: 28px;
      font-weight: 700;
      color: var(--orange);
      letter-spacing: 1px;
      margin-bottom: 24px;
    }

    .field { margin-bottom: 16px; }

    label {
      display: block;
      font-size: 12px;
      font-weight: 500;
      color: var(--muted);
      text-transform: uppercase;
      letter-spacing: 0.8px;
      margin-bottom: 6px;
    }

    select {
      width: 100%;
      padding: 10px 12px;
      background: var(--bg);
      border: 1px solid var(--border);
      border-radius: 6px;
      color: var(--text);
      font-family: inherit;
      font-size: 14px;
      cursor: pointer;
      transition: border-color 0.15s;
      appearance: none;
      background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='12' height='8' viewBox='0 0 12 8'%3E%3Cpath d='M1 1l5 5 5-5' stroke='%23777' stroke-width='1.5' fill='none' stroke-linecap='round'/%3E%3C/svg%3E");
      background-repeat: no-repeat;
      background-position: right 12px center;
    }
    select:focus { outline: none; border-color: var(--orange); }

    .checkboxes {
      display: flex;
      gap: 12px;
      margin-bottom: 12px;
    }
    .checkboxes:last-of-type { margin-bottom: 20px; }

    .check-label {
      display: flex;
      align-items: center;
      gap: 8px;
      background: var(--bg);
      border: 1px solid var(--border);
      border-radius: 6px;
      padding: 10px 14px;
      cursor: pointer;
      flex: 1;
      font-size: 13px;
      transition: border-color 0.15s, background 0.15s;
      user-select: none;
    }
    .check-label:has(input:checked) {
      border-color: var(--orange);
      background: rgba(255,152,0,0.06);
      color: var(--orange);
    }
    .check-label.free:has(input:checked) {
      border-color: var(--green);
      background: rgba(76,175,80,0.06);
      color: var(--green);
    }
    .check-label input { display: none; }

    /* Progress bar */
    .progress-wrap { margin-bottom: 20px; }

    .progress-track {
      position: relative;
      height: 8px;
      background: var(--bg);
      border: 1px solid var(--border);
      border-radius: 99px;
      margin-bottom: 8px;
      cursor: pointer;
    }
    .progress-fill {
      position: absolute;
      top: 0; left: 0; height: 100%;
      border-radius: 99px;
      pointer-events: none;
    }
    .progress-dot {
      position: absolute;
      top: 50%;
      transform: translate(-50%, -50%);
      width: 16px; height: 16px;
      border-radius: 50%;
      border: 2px solid var(--surface);
      cursor: grab;
      z-index: 2;
      transition: transform 0.1s, box-shadow 0.1s;
      touch-action: none;
    }
    .progress-dot:hover {
      transform: translate(-50%, -50%) scale(1.25);
      box-shadow: 0 0 0 4px rgba(255,152,0,0.2);
    }
    .progress-dot.dragging {
      cursor: grabbing;
      transform: translate(-50%, -50%) scale(1.35);
      box-shadow: 0 0 0 6px rgba(255,152,0,0.25);
      transition: none;
    }
    .progress-dot.from { background: #aaa; }
    .progress-dot.to   { background: var(--orange); }

    .progress-labels {
      display: flex;
      justify-content: space-between;
      font-size: 9px;
      color: var(--muted);
      text-transform: uppercase;
      letter-spacing: 0.5px;
      padding: 0 2px;
    }

    /* Tooltip */
    .dot-tooltip {
      position: absolute;
      bottom: 22px;
      left: 50%;
      transform: translateX(-50%);
      background: #333;
      color: #fff;
      font-size: 10px;
      white-space: nowrap;
      padding: 3px 6px;
      border-radius: 4px;
      pointer-events: none;
      opacity: 0;
      transition: opacity 0.15s;
    }
    .progress-dot:hover .dot-tooltip,
    .progress-dot.dragging .dot-tooltip { opacity: 1; }

    /* Price box */
    .price-box {
      background: var(--bg);
      border: 1px solid var(--border);
      border-radius: 8px;
      padding: 16px 16px 12px;
      text-align: center;
    }
    .price-label {
      font-size: 11px;
      text-transform: uppercase;
      letter-spacing: 1px;
      color: var(--muted);
      margin-bottom: 4px;
    }
    .price-original {
      font-size: 14px;
      color: var(--muted);
      text-decoration: line-through;
      min-height: 20px;
      margin-bottom: 2px;
    }
    .price-value {
      font-family: 'Rajdhani', sans-serif;
      font-size: 36px;
      font-weight: 700;
      color: var(--orange);
    }
    .price-value.error { font-size: 16px; color: #e57373; }
    .price-badge {
      display: inline-block;
      margin-top: 6px;
      background: rgba(76,175,80,0.15);
      color: var(--green);
      border-radius: 4px;
      padding: 2px 8px;
      font-size: 12px;
      font-weight: 500;
      min-height: 20px;
    }
  </style>
</head>
<body>
  <div class="card">
    <h1>Rank Boost</h1>

    <div class="field">
      <label>Current Rank</label>
      <select id="currentRank"></select>
    </div>

    <div class="field">
      <label>Desired Rank</label>
      <select id="desiredRank"></select>
    </div>

    <div class="field">
      <label>Role</label>
      <select id="role"></select>
    </div>

    <div class="checkboxes">
      <label class="check-label">
        <input type="checkbox" id="duoBoost"> Duo Boost <span style="color:var(--muted);font-size:11px">+70%</span>
      </label>
      <label class="check-label">
        <input type="checkbox" id="stream"> Stream <span style="color:var(--muted);font-size:11px">+5%</span>
      </label>
    </div>
    <div class="checkboxes">
      <label class="check-label free">
        <input type="checkbox" id="offline"> Offline Mode <span style="color:#4caf50;font-size:11px">Free</span>
      </label>
      <label class="check-label free">
        <input type="checkbox" id="vpn"> VPN <span style="color:#4caf50;font-size:11px">Free</span>
      </label>
    </div>

    <div class="progress-wrap">
      <div class="progress-track" id="progressTrack">
        <div class="progress-fill" id="progressFill"></div>
        <div class="progress-dot from" id="dotFrom">
          <div class="dot-tooltip" id="tipFrom"></div>
        </div>
        <div class="progress-dot to" id="dotTo">
          <div class="dot-tooltip" id="tipTo"></div>
        </div>
      </div>
      <div class="progress-labels" id="progressLabels"></div>
    </div>

    <div class="price-box">
      <div class="price-label">Total Price</div>
      <div class="price-original" id="priceOriginal"></div>
      <div class="price-value" id="priceOutput">—</div>
      <div class="price-badge" id="priceBadge"></div>
    </div>
  </div>

  <script>
    const TIERS = ["bronze","silver","gold","platinum","diamond","master","grandmaster"];
    const DIVS  = [5,4,3,2,1];

    const TIER_COLOR = {
      bronze:"#cd7f32", silver:"#aaa", gold:"#ffd700",
      platinum:"#4dd0e1", diamond:"#5c9bfa", master:"#c678dd", grandmaster:"#ff9800"
    };

    const STEP_PRICE = {
      bronze5:0.902,bronze4:0.902,bronze3:0.902,bronze2:0.902,bronze1:0.902,
      silver5:1.462,silver4:1.462,silver3:1.462,silver2:1.462,silver1:1.462,
      gold5:2.262,gold4:2.262,gold3:2.262,gold2:2.262,gold1:2.262,
      platinum5:3.462,platinum4:3.462,platinum3:3.462,platinum2:3.462,platinum1:3.462,
      diamond5:6.534,diamond4:6.534,diamond3:6.534,diamond2:6.534,diamond1:6.534,
      master5:13.75,master4:16.78,master3:20.47,master2:25.00,master1:25.00,
      grandmaster5:44.00,grandmaster4:61.47,grandmaster3:85.87,grandmaster2:120.00,
    };

    const ROLES = [
      ["tank",   "Tank",    1.00,1.15],
      ["dd",     "DD",      1.00,1.05],
      ["support","Support", 1.15,1.00],
      ["openq",  "Open Q",  1.00,1.00],
    ];

    const DISCOUNT = [0,0,0.05,0.10,0.15,0.15,0.15];

    const RANKS = TIERS.flatMap(tier =>
      DIVS.map(div => ({
        key: `${tier}${div}`,
        label: `${tier.charAt(0).toUpperCase()+tier.slice(1)} ${["V","IV","III","II","I"][5-div]}`,
        tier, div,
      }))
    );
    const TOTAL = RANKS.length; // 35

    const $ = id => document.getElementById(id);

    // ── Helpers ──────────────────────────────────────────────────────────────
    function stepPrice(tier, div) { return STEP_PRICE[`${tier}${div}`] ?? 0; }

    function calcBase(fromIdx, toIdx) {
      let t = 0;
      for (let i = fromIdx; i < toIdx; i++) t += stepPrice(RANKS[i].tier, RANKS[i].div);
      return t;
    }

    function applyMults(base, isDuo, isStream, roleValue) {
      let t = base;
      if (isDuo)    t *= 1.70;
      if (isStream) t *= 1.05;
      const role = ROLES.find(r => r[0] === roleValue);
      if (role) t *= isDuo ? role[3] : role[2];
      return t;
    }

    function tiersSpanned(fromIdx, toIdx) {
      return TIERS.indexOf(RANKS[toIdx].tier) - TIERS.indexOf(RANKS[fromIdx].tier);
    }

    function pct(idx) { return (idx / (TOTAL - 1)) * 100; }

    // ── Fill selects ─────────────────────────────────────────────────────────
    function fillRankSelect(el, selectedKey) {
      el.innerHTML = "";
      RANKS.forEach(({ key, label }) => {
        const opt = new Option(label, key);
        if (key === selectedKey) opt.selected = true;
        el.add(opt);
      });
    }

    function fillRoleSelect(isDuo, currentValue) {
      const el = $("role");
      el.innerHTML = "";
      ROLES.forEach(([value, label, sm, dm]) => {
        const mult = isDuo ? dm : sm;
        const sfx  = mult !== 1 ? ` (+${Math.round((mult-1)*100)}%)` : "";
        el.add(new Option(label + sfx, value));
      });
      if (currentValue) el.value = currentValue;
    }

    // ── Progress bar visuals ─────────────────────────────────────────────────
    function updateProgress(fromIdx, toIdx) {
      const fp = pct(fromIdx), tp = pct(toIdx);
      const c1 = TIER_COLOR[RANKS[fromIdx].tier];
      const c2 = TIER_COLOR[RANKS[toIdx].tier];
      $("progressFill").style.cssText =
        `left:${fp}%;width:${tp-fp}%;background:linear-gradient(90deg,${c1},${c2});`;
      $("dotFrom").style.left = fp + "%";
      $("dotTo").style.left   = tp + "%";
      $("tipFrom").textContent = RANKS[fromIdx].label;
      $("tipTo").textContent   = RANKS[toIdx].label;
    }

    function buildLabels() {
      const el = $("progressLabels");
      el.innerHTML = "";
      TIERS.forEach(t => {
        const span = document.createElement("span");
        span.textContent = t.slice(0,2).toUpperCase();
        span.style.color = TIER_COLOR[t];
        el.appendChild(span);
      });
    }

    // ── Render price ─────────────────────────────────────────────────────────
    function render() {
      const fromIdx = RANKS.findIndex(r => r.key === $("currentRank").value);
      const toIdx   = RANKS.findIndex(r => r.key === $("desiredRank").value);
      const isDuo   = $("duoBoost").checked;
      const out     = $("priceOutput");

      if (toIdx <= fromIdx) {
        out.textContent = "Choose a higher rank";
        out.className   = "price-value error";
        $("priceOriginal").textContent = "";
        $("priceBadge").textContent    = "";
        return;
      }

      updateProgress(fromIdx, toIdx);

      const base     = calcBase(fromIdx, toIdx);
      const noDisc   = applyMults(base, isDuo, $("stream").checked, $("role").value);
      const discRate = DISCOUNT[Math.min(tiersSpanned(fromIdx, toIdx), DISCOUNT.length-1)];
      const final    = noDisc * (1 - discRate);

      out.className   = "price-value";
      out.textContent = "$" + final.toFixed(2);

      if (discRate > 0) {
        $("priceOriginal").textContent = "$" + noDisc.toFixed(2);
        $("priceBadge").textContent    = `Save $${(noDisc-final).toFixed(2)} (${discRate*100}% off)`;
      } else {
        $("priceOriginal").textContent = "";
        $("priceBadge").textContent    = "";
      }
    }

    // ── Drag logic ───────────────────────────────────────────────────────────
    function makeDraggable(dotEl, isFrom) {
      let dragging = false;

      function onMove(clientX) {
        const track  = $("progressTrack");
        const rect   = track.getBoundingClientRect();
        const ratio  = Math.max(0, Math.min(1, (clientX - rect.left) / rect.width));
        const rawIdx = Math.round(ratio * (TOTAL - 1));

        const fromIdx = RANKS.findIndex(r => r.key === $("currentRank").value);
        const toIdx   = RANKS.findIndex(r => r.key === $("desiredRank").value);

        if (isFrom) {
          // from dot: if it would overtake toIdx, push toIdx forward together
          const newFrom = Math.min(rawIdx, TOTAL - 2);
          if (newFrom >= toIdx) {
            const newTo = Math.min(newFrom + 1, TOTAL - 1);
            $("desiredRank").value = RANKS[newTo].key;
          }
          $("currentRank").value = RANKS[newFrom].key;
        } else {
          // to dot: can't go before fromIdx
          const clamped = Math.max(rawIdx, fromIdx + 1);
          $("desiredRank").value = RANKS[clamped].key;
        }
        render();
      }

      // Mouse
      dotEl.addEventListener("mousedown", e => {
        dragging = true;
        dotEl.classList.add("dragging");
        e.preventDefault();
      });
      document.addEventListener("mousemove", e => {
        if (dragging) onMove(e.clientX);
      });
      document.addEventListener("mouseup", () => {
        if (dragging) { dragging = false; dotEl.classList.remove("dragging"); }
      });

      // Touch
      dotEl.addEventListener("touchstart", e => {
        dragging = true;
        dotEl.classList.add("dragging");
        e.preventDefault();
      }, { passive: false });
      document.addEventListener("touchmove", e => {
        if (dragging) onMove(e.touches[0].clientX);
      }, { passive: true });
      document.addEventListener("touchend", () => {
        if (dragging) { dragging = false; dotEl.classList.remove("dragging"); }
      });
    }

    // ── Init ─────────────────────────────────────────────────────────────────
    fillRankSelect($("currentRank"), "gold5");
    fillRankSelect($("desiredRank"), "diamond5");
    fillRoleSelect(false, "tank");
    buildLabels();
    render();

    makeDraggable($("dotFrom"), true);
    makeDraggable($("dotTo"),   false);

    $("currentRank").addEventListener("change", () => {
      const fromIdx = RANKS.findIndex(r => r.key === $("currentRank").value);
      const toIdx   = RANKS.findIndex(r => r.key === $("desiredRank").value);
      if (toIdx <= fromIdx) $("desiredRank").value = RANKS[fromIdx+1]?.key ?? RANKS[fromIdx].key;
      render();
    });
    $("desiredRank").addEventListener("change", render);
    $("role").addEventListener("change", render);
    $("stream").addEventListener("change", render);
    $("duoBoost").addEventListener("change", () => {
      fillRoleSelect($("duoBoost").checked, $("role").value);
      render();
    });
  </script>
</body>
</html>
