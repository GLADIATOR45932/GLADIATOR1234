<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="utf-8" />
<meta name="viewport" content="width=device-width,initial-scale=1,maximum-scale=1,user-scalable=no" />
<title>Gladiator</title>
<style>
  :root{
    --bg:#0b0b0f;
    --bg-soft:#111119;
    --panel:#141420;
    --ink:#e8e8f0;
    --muted:#a6a6b3;
    --red:#ff1f3d;
    --red-2:#ff3b58;
    --accent:#ff2f4a;
    --line:#1f2030;
    --green:#34e5a6;
    --yellow:#ffd36a;
  }
  *{box-sizing:border-box}
  html,body{height:100%;background:var(--bg);color:var(--ink);font-family: ui-rounded, system-ui, -apple-system, Segoe UI, Roboto, "Helvetica Neue", Arial, "Noto Sans", "Liberation Sans", sans-serif; margin:0}
  /* Lightning corner effect */
  body::before, body::after{
    content:"";
    position:fixed; z-index:0; width:45vmin; height:45vmin;
    background:
      radial-gradient(closest-side, rgba(255,31,61,.35), transparent 60%),
      conic-gradient(from 0deg, rgba(255,80,100,.35), transparent 40%, rgba(255,31,61,.6), transparent 70%);
    filter: blur(18px) saturate(140%);
    animation: arc 8s linear infinite;
    pointer-events:none;
  }
  body::before{ top:-10vmin; left:-12vmin; }
  body::after{ bottom:-12vmin; right:-10vmin; animation-direction: reverse; }
  @keyframes arc{ to{ transform:rotate(360deg)} }

  /* Layout */
  .app{ position:relative; min-height:100%; padding:88px 16px 90px; isolation:isolate; }
  header{
    position:fixed; top:0; left:0; right:0; height:72px;
    background: linear-gradient(180deg,#12121a, #0d0d14);
    border-bottom:1px solid var(--line);
    display:flex; align-items:center; justify-content:center; gap:16px;
    z-index:10;
  }
  .brand{
    position:absolute; left:50%; transform:translateX(-50%);
    font-weight:900; letter-spacing:.22em; font-size:20px; color:#fff;
    text-shadow:0 0 18px rgba(255,47,74,.35);
  }
  .nav{
    position:absolute; inset:0; display:flex; align-items:center; justify-content:space-between; padding:0 10px;
  }
  .icon-btn{
    width:52px; height:52px; border-radius:14px; border:1px solid var(--line);
    background:linear-gradient(180deg,#161621,#11111a);
    display:grid; place-items:center; cursor:pointer; transition:.15s transform ease, .15s filter ease;
    box-shadow:inset 0 0 0 1px rgba(255,47,74,.08);
  }
  .icon-btn:active{ transform:scale(.96) }
  .icon-btn.active{ outline:2px solid rgba(255,47,74,.55); box-shadow:0 0 0 6px rgba(255,47,74,.08) inset; }
  .icon{ width:26px; height:26px; fill: none; stroke:#ff4b63; stroke-width:2.2; }

  /* Content sections */
  .grid{ display:grid; gap:18px; max-width:980px; margin:0 auto; }
  .cards{ display:grid; grid-template-columns: repeat(auto-fit,minmax(260px,1fr)); gap:18px; }
  .card{
    background:linear-gradient(180deg,#151522,#11111a); border:1px solid var(--line); border-radius:18px; overflow:hidden;
    box-shadow: 0 8px 30px rgba(0,0,0,.3), inset 0 0 0 1px rgba(255,47,74,.05);
  }
  .thumb{ background:#0d0d16; height:160px; display:grid; place-items:center; border-bottom:1px solid var(--line); }
  .card-body{ padding:14px 14px 16px }
  .title{ font-weight:800; letter-spacing:.08em; font-size:18px; }
  .muted{ color:var(--muted); font-size:13px; margin-top:6px }
  .row{ display:flex; gap:10px; align-items:center; margin-top:12px }
  .btn{
    padding:10px 14px; border-radius:12px; border:1px solid var(--line);
    background:linear-gradient(180deg,#1a1a28,#131320); color:#fff; font-weight:700; letter-spacing:.06em;
    cursor:pointer; transition: .15s transform ease, .15s background ease;
  }
  .btn.red{ background:linear-gradient(180deg,#ff2347,#e41836); border-color:#c20f29; box-shadow:0 4px 18px rgba(255,35,71,.35) }
  .btn:active{ transform: translateY(1px) }

  /* Section panels */
  section{ display:none }
  section.active{ display:block }

  /* Game modal */
  .modal{
    position:fixed; inset:0; display:none; align-items:center; justify-content:center; padding:18px; z-index:20;
    background: rgba(0,0,0,.55);
  }
  .modal.show{ display:flex }
  .sheet{ width:min(680px, 96vw); background:linear-gradient(180deg,#151521,#101018); border:1px solid var(--line); border-radius:18px; overflow:hidden }
  .sheet .hd{ display:flex; align-items:center; justify-content:space-between; padding:14px 16px; border-bottom:1px solid var(--line) }
  .sheet .bd{ padding:16px }
  .x{ background:#191927; border:1px solid var(--line); color:#fff; border-radius:10px; padding:8px 12px; cursor:pointer }
  .fld{ display:grid; gap:8px; margin:10px 0 }
  .fld label{ font-size:13px; color:var(--muted) }
  .inp, .inp-num, .txt{
    width:100%; background:#10101a; color:#fff; border:1px solid var(--line); padding:12px 12px; border-radius:12px;
  }
  .txt{ min-height:90px; resize:vertical }
  .two{ display:grid; grid-template-columns:1fr 1fr; gap:10px }
  .note{ color:var(--muted); font-size:12px }

  /* Account & Contact */
  .stack{ display:grid; gap:12px; max-width:760px; margin:0 auto }
  .bar{ display:flex; gap:8px; align-items:center }
  .chip{ padding:7px 10px; background:#171729; border:1px solid var(--line); border-radius:999px; font-size:12px; color:var(--muted) }
  .list{ display:grid; gap:10px }
  .msg{
    background:linear-gradient(180deg,#141425,#101018); border:1px solid var(--line); border-radius:14px; padding:10px 12px;
  }

  /* Footer socials */
  footer{
    position:fixed; bottom:0; left:0; right:0; height:72px; display:flex; align-items:center; justify-content:center; gap:14px;
    border-top:1px solid var(--line); background:linear-gradient(180deg,#0f0f16,#0b0b11); z-index:9;
  }
  .link{
    display:flex; gap:8px; align-items:center; padding:8px 12px; border-radius:999px; border:1px solid var(--line);
    background:#12121c; color:#fff; text-decoration:none; font-size:13px;
  }
  .dot{ width:10px; height:10px; border-radius:50%; background:var(--red); box-shadow:0 0 10px rgba(255,47,74,.9) }
  .notif{ font-size:12px; color:#ff9aa8 }

  /* Splash (Loading) */
  .splash{
    position:fixed; inset:0; display:grid; place-items:center; background:radial-gradient(1200px 700px at 50% 80%, rgba(255,47,74,.08), transparent), #0a0a0e; z-index:30;
  }
  .sp-title{ font-size:36px; font-weight:900; letter-spacing:.25em; color:#ff304b; text-shadow:0 0 20px rgba(255,50,80,.55) }
  .spinner{ margin-top:14px; width:62px; height:62px; border-radius:50%; border:3px solid rgba(255,47,74,.35); border-top-color:#ff2f4a; animation: spin 1.1s linear infinite }
  @keyframes spin{ to{ transform:rotate(360deg)} }

  /* SVG thumbs look “pixelated” */
  svg{ image-rendering: pixelated; }

  /* Small screens */
  @media (max-width:540px){
    .title{ font-size:16px }
    .thumb{ height:140px }
  }
</style>
</head>
<body>

<!-- Splash -->
<div class="splash" id="splash">
  <div style="text-align:center">
    <div class="sp-title">hello spartan</div>
    <div class="spinner"></div>
  </div>
</div>

<header>
  <div class="nav">
    <div style="display:flex; gap:10px">
      <button class="icon-btn" data-tab="home" id="btnHome" title="Home">
        <svg class="icon" viewBox="0 0 24 24"><path d="M3 10.5 12 3l9 7.5M6 9.5V21h12V9.5"/></svg>
      </button>
      <button class="icon-btn" data-tab="about" id="btnAbout" title="About">
        <svg class="icon" viewBox="0 0 24 24"><circle cx="12" cy="12" r="9"/><path d="M12 8.5h.01M11 12h1v4"/></svg>
      </button>
    </div>
    <div class="brand">GLADIATOR</div>
    <div style="display:flex; gap:10px">
      <button class="icon-btn" data-tab="contact" id="btnContact" title="Contact">
        <svg class="icon" viewBox="0 0 24 24"><path d="M4 5h16v12H6l-2 2V5z"/><path d="M9 10h6M9 13h6M9 7h6"/></svg>
      </button>
      <button class="icon-btn" data-tab="account" id="btnAccount" title="Account">
        <svg class="icon" viewBox="0 0 24 24"><circle cx="12" cy="8" r="4"/><path d="M4 21a8 8 0 0 1 16 0"/></svg>
      </button>
    </div>
  </div>
</header>

<div class="app">
  <section id="home" class="active">
    <div class="grid">
      <div class="cards">

        <!-- COD Mobile -->
        <div class="card">
          <div class="thumb">
            <!-- Simple inline SVG poster -->
            <svg width="100%" height="100%" viewBox="0 0 320 160">
              <rect x="0" y="0" width="320" height="160" fill="#0f0f16"/>
              <rect x="8" y="8" width="304" height="144" fill="#17172a" stroke="#27273b"/>
              <g stroke="#ff2f4a" stroke-width="3">
                <path d="M20 120 L70 40 L120 120 Z" fill="none"/>
                <path d="M130 120 L180 40 L230 120 Z" fill="none"/>
                <path d="M240 120 L290 40 L300 60" fill="none"/>
              </g>
              <text x="160" y="150" text-anchor="middle" fill="#ff2f4a" style="font: 900 18px sans-serif; letter-spacing:3px">CALL OF DUTY MOBILE</text>
            </svg>
          </div>
          <div class="card-body">
            <div class="title">Call of Duty Mobile</div>
            <div class="muted">Competitive FPS on mobile.</div>
            <div class="row">
              <button class="btn red" onclick="openGame('Call of Duty Mobile')">Open</button>
              <button class="btn" onclick="shareGame('Call of Duty Mobile')">Share</button>
            </div>
          </div>
        </div>

        <!-- Delta Force -->
        <div class="card">
          <div class="thumb">
            <svg width="100%" height="100%" viewBox="0 0 320 160">
              <rect width="320" height="160" fill="#0f0f16"/>
              <rect x="8" y="8" width="304" height="144" fill="#161626" stroke="#27273b"/>
              <g stroke="#ff2f4a" stroke-width="3">
                <rect x="30" y="90" width="50" height="30" fill="none"/>
                <rect x="90" y="70" width="60" height="50" fill="none"/>
                <rect x="170" y="50" width="80" height="70" fill="none"/>
                <rect x="260" y="30" width="40" height="90" fill="none"/>
              </g>
              <text x="160" y="150" text-anchor="middle" fill="#ff2f4a" style="font: 900 18px sans-serif; letter-spacing:3px">DELTA FORCE</text>
            </svg>
          </div>
          <div class="card-body">
            <div class="title">Delta Force</div>
            <div class="muted">Classic tactical action.</div>
            <div class="row">
              <button class="btn red" onclick="openGame('Delta Force')">Open</button>
              <button class="btn" onclick="shareGame('Delta Force')">Share</button>
            </div>
          </div>
        </div>

        <!-- PUBG Mobile -->
        <div class="card">
          <div class="thumb">
            <svg width="100%" height="100%" viewBox="0 0 320 160">
              <rect width="320" height="160" fill="#0f0f16"/>
              <rect x="8" y="8" width="304" height="144" fill="#151524" stroke="#27273b"/>
              <g stroke="#ff2f4a" stroke-width="3">
                <circle cx="80" cy="85" r="26" fill="none"/>
                <rect x="120" y="60" width="160" height="50" rx="8" fill="none"/>
                <path d="M140 115 h120" />
              </g>
              <text x="160" y="150" text-anchor="middle" fill="#ff2f4a" style="font: 900 18px sans-serif; letter-spacing:3px">PUBG MOBILE</text>
            </svg>
          </div>
          <div class="card-body">
            <div class="title">PUBG Mobile</div>
            <div class="muted">Battle royale, squad up.</div>
            <div class="row">
              <button class="btn red" onclick="openGame('PUBG Mobile')">Open</button>
              <button class="btn" onclick="shareGame('PUBG Mobile')">Share</button>
            </div>
          </div>
        </div>

      </div>

      <div class="row" id="videoNoticeRow" style="display:none">
        <div class="notif">Gladiator posted new videos • Choose a platform:</div>
        <a class="link" id="ytLink" href="#" target="_blank">
          <span class="dot"></span><span id="ytName">YouTube</span>
        </a>
        <a class="link" id="igLink" href="#" target="_blank">
          <span class="dot"></span><span id="igName">Instagram</span>
        </a>
      </div>
    </div>
  </section>

  <section id="about">
    <div class="grid">
      <div class="card">
        <div class="card-body">
          <div class="title">About Gladiator</div>
          <p class="muted" style="margin-top:10px">
            eSports content, daily uploads, collaborations, and squad play.  
            Only verified accounts can request matches and send messages.
          </p>
          <div class="row">
            <span class="chip">Theme: Red/Black</span>
            <span class="chip">Secure OTP (simulated)</span>
            <span class="chip">Admin-only management</span>
          </div>
        </div>
      </div>

      <!-- AI Chat -->
      <div class="card">
        <div class="card-body">
          <div class="title">AI Assistant</div>
          <p class="muted">Ask anything about the games or schedule.</p>
          <div class="fld">
            <label>Your message</label>
            <textarea id="aiIn" class="txt" placeholder="Type here..."></textarea>
          </div>
          <div class="row">
            <button class="btn red" onclick="askAI()">Send to AI</button>
            <button class="btn" onclick="clearAI()">Clear</button>
          </div>
          <div class="list" id="aiOut" style="margin-top:12px"></div>
        </div>
      </div>
    </div>
  </section>

  <section id="contact">
    <div class="stack">
      <div class="card">
        <div class="card-body">
          <div class="title">Contact Admin</div>
          <p class="muted">Send a direct message (requires sign-in).</p>
          <div class="fld">
            <label>Subject</label>
            <input class="inp" id="msgSubj" placeholder="Collab / Scrim / Question">
          </div>
          <div class="fld">
            <label>Message</label>
            <textarea class="txt" id="msgBody" placeholder="Type your message..."></textarea>
          </div>
          <div class="row">
            <button class="btn red" onclick="sendMessage()">Send</button>
            <div class="note" id="msgNote"></div>
          </div>
        </div>
      </div>

      <!-- Inbox (local preview) -->
      <div class="card">
        <div class="card-body">
          <div class="title">Inbox (local)</div>
          <div class="list" id="inbox"></div>
        </div>
      </div>
    </div>
  </section>

  <section id="account">
    <div class="stack">
      <div class="card">
        <div class="card-body">
          <div class="title">Create Account</div>
          <div class="fld">
            <label>Phone number</label>
            <input id="accPhone" class="inp" placeholder="+98..." inputmode="tel">
          </div>
          <div class="row">
            <button class="btn" onclick="sendOTP()">Send Code</button>
            <div class="note" id="otpSentNote"></div>
          </div>
          <div class="two">
            <div class="fld">
              <label>OTP code</label>
              <input id="accOTP" class="inp-num" placeholder="4-digit" maxlength="6" inputmode="numeric">
            </div>
            <div class="fld">
              <label>Display name</label>
              <input id="accName" class="inp" placeholder="Your gamer name">
            </div>
          </div>
          <div class="row">
            <button class="btn red" onclick="verifyOTP()">Create / Sign In</button>
            <div class="note" id="accNote"></div>
          </div>
        </div>
      </div>

      <!-- Admin controls -->
      <div class="card">
        <div class="card-body">
          <div class="title">Admin Mode</div>
          <div class="fld">
            <label>Enter Admin PIN</label>
            <input id="adminPIN" class="inp" placeholder="PIN">
          </div>
          <div class="row">
            <button class="btn" onclick="unlockAdmin()">Unlock</button>
            <div class="note" id="adminNote"></div>
          </div>

          <div id="adminPanel" style="display:none; margin-top:14px">
            <div class="title" style="font-size:16px">Social & Video Links</div>
            <div class="two">
              <div class="fld"><label>YouTube name</label><input id="ytNameInp" class="inp" placeholder="YouTube"/></div>
              <div class="fld"><label>YouTube link</label><input id="ytLinkInp" class="inp" placeholder="https://..."/></div>
            </div>
            <div class="two">
              <div class="fld"><label>Instagram name</label><input id="igNameInp" class="inp" placeholder="Instagram"/></div>
              <div class="fld"><label>Instagram link</label><input id="igLinkInp" class="inp" placeholder="https://..."/></div>
            </div>
            <div class="two">
              <div class="fld"><label>New video (YouTube link)</label><input id="newYT" class="inp" placeholder="https://youtube.com/..."/></div>
              <div class="fld"><label>New video (Instagram link)</label><input id="newIG" class="inp" placeholder="https://instagram.com/..."/></div>
            </div>
            <div class="row">
              <button class="btn red" onclick="postVideos()">Post videos</button>
              <div class="note">This triggers on-site notification.</div>
            </div>

            <div class="title" style="font-size:16px; margin-top:16px">Upload Music (local)</div>
            <div class="fld">
              <label>Select audio file</label>
              <input id="musicFile" type="file" accept="audio/*" />
            </div>
            <div class="row">
              <button class="btn" onclick="addMusic()">Add to player</button>
              <div class="note">Admin-only. Plays locally in browser.</div>
            </div>
            <div id="musicList" class="list" style="margin-top:12px"></div>
          </div>
        </div>
      </div>

    </div>
  </section>
</div>

<footer>
  <a class="link" id="ytLinkFoot" href="#" target="_blank">
    <span class="dot"></span><span id="ytNameFoot">YouTube</span>
  </a>
  <a class="link" id="igLinkFoot" href="#" target="_blank">
    <span class="dot"></span><span id="igNameFoot">Instagram</span>
  </a>
</footer>

<!-- Game Modal -->
<div class="modal" id="gameModal" aria-hidden="true">
  <div class="sheet">
    <div class="hd">
      <div class="title" id="gameTitle">Game</div>
      <button class="x" onclick="closeGame()">Close</button>
    </div>
    <div class="bd">
      <div class="two">
        <div>
          <div class="fld">
            <label>Admin In‑Game Name</label>
            <input class="inp" id="adminGameName" value="Gladiator" readonly>
          </div>
          <div class="fld">
            <label>Admin Numeric ID</label>
            <input class="inp" id="adminGameID" value="88442211" readonly>
          </div>
        </div>
        <div>
          <div class="fld">
            <label>Your In‑Game Name</label>
            <input class="inp" id="yourGameName" placeholder="Your nickname">
          </div>
          <div class="fld">
            <label>Your Numeric ID</label>
            <input class="inp" id="yourGameID" placeholder="12345678">
          </div>
        </div>
      </div>
      <div class="fld">
        <label>Message to Admin</label>
        <textarea class="txt" id="yourMsg" placeholder="Let’s play tonight? Mode, time, etc."></textarea>
      </div>
      <div class="row">
        <button class="btn red" onclick="requestPlay()">Send Play Request</button>
        <div class="note" id="gameNote"></div>
      </div>
    </div>
  </div>
</div>

<script>
/* =========================
   Simple state + storage
========================= */
const ADMIN_PIN = "GLAD-ADMIN-2025";
const st = {
  user: null,       // {name, phone}
  otpCode: null,    // generated code for demo
  adminUnlocked: false,
  socials: {
    ytName:"YouTube", ytLink:"#",
    igName:"Instagram", igLink:"#"
  },
  inbox: [],        // {from, phone, ts, subj, body}
  music: [],        // {name, url}
  posted: false     // whether admin posted new videos (for notification)
};
// Load from localStorage (if any)
(function load(){
  try{
    const u = localStorage.getItem("glad_user");
    if(u) st.user = JSON.parse(u);
    const s = localStorage.getItem("glad_socials");
    if(s) st.socials = JSON.parse(s);
    const i = localStorage.getItem("glad_inbox");
    if(i) st.inbox = JSON.parse(i);
    const m = localStorage.getItem("glad_music");
    if(m) st.music = JSON.parse(m);
  }catch(e){}
})();

/* =========================
   Nav (icons -> tabs)
========================= */
const tabs = ["home","about","contact","account"];
function setTab(id){
  tabs.forEach(t=>{
    document.getElementById(t).classList.remove("active");
    document.querySelector(`[data-tab="${t}"]`).classList.remove("active");
  });
  document.getElementById(id).classList.add("active");
  document.querySelector(`[data-tab="${id}"]`).classList.add("active");
}
document.querySelectorAll(".icon-btn").forEach(b=>{
  b.addEventListener("click",()=> setTab(b.dataset.tab));
});
setTab("home");

/* =========================
   Splash
========================= */
setTimeout(()=>{ document.getElementById("splash").style.display="none"; }, 1200);

/* =========================
   Home – social links + notice
========================= */
function refreshSocials(){
  const {ytName, ytLink, igName, igLink} = st.socials;
  document.getElementById("ytName").textContent = ytName;
  document.getElementById("igName").textContent = igName;
  document.getElementById("ytLink").href = ytLink || "#";
  document.getElementById("igLink").href = igLink || "#";
  document.getElementById("ytNameFoot").textContent = ytName;
  document.getElementById("igNameFoot").textContent = igName;
  document.getElementById("ytLinkFoot").href = ytLink || "#";
  document.getElementById("igLinkFoot").href = igLink || "#";
  document.getElementById("videoNoticeRow").style.display = st.posted ? "flex":"none";
}
refreshSocials();

/* =========================
   Game cards
========================= */
let currentGame = null;
function openGame(name){
  currentGame = name;
  document.getElementById("gameTitle").textContent = name;
  document.getElementById("gameModal").classList.add("show");
  document.getElementById("gameNote").textContent = "";
}
function closeGame(){
  document.getElementById("gameModal").classList.remove("show");
  currentGame = null;
}
function shareGame(name){
  alert("Share: " + name);
}
function requestPlay(){
  if(!st.user){
    document.getElementById("gameNote").textContent = "Sign in first (Account icon).";
    return;
  }
  const youN = document.getElementById("yourGameName").value.trim();
  const youI = document.getElementById("yourGameID").value.trim();
  const msg  = document.getElementById("yourMsg").value.trim();
  if(!youN || !youI){
    document.getElementById("gameNote").textContent = "Enter your name and numeric ID.";
    return;
  }
  const subj = `[${currentGame}] Play request from ${youN} (${youI})`;
  st.inbox.unshift({from: st.user.name, phone: st.user.phone, ts: Date.now(), subj, body: msg || "Let's play!"});
  localStorage.setItem("glad_inbox", JSON.stringify(st.inbox));
  renderInbox();
  document.getElementById("gameNote").textContent = "Request sent.";
}

/* =========================
   Contact (messages)
========================= */
function sendMessage(){
  const subj = document.getElementById("msgSubj").value.trim();
  const body = document.getElementById("msgBody").value.trim();
  if(!st.user){ setTab("account"); document.getElementById("msgNote").textContent = "Sign in first."; return; }
  if(!subj || !body){ document.getElementById("msgNote").textContent = "Fill subject and message."; return; }
  st.inbox.unshift({from: st.user.name, phone: st.user.phone, ts: Date.now(), subj, body});
  localStorage.setItem("glad_inbox", JSON.stringify(st.inbox));
  renderInbox();
  document.getElementById("msgSubj").value = "";
  document.getElementById("msgBody").value = "";
  document.getElementById("msgNote").textContent = "Message sent.";
}
function renderInbox(){
  const box = document.getElementById("inbox");
  box.innerHTML = "";
  st.inbox.forEach(m=>{
    const d = new Date(m.ts);
    const el = document.createElement("div");
    el.className = "msg";
    el.innerHTML = `<div style="font-weight:700">${m.subj}</div>
      <div class="muted">${d.toLocaleString()} • From: ${m.from} (${m.phone})</div>
      <div style="margin-top:6px">${m.body}</div>`;
    box.appendChild(el);
  });
}
renderInbox();

/* =========================
   Account + OTP (simulated)
========================= */
function sendOTP(){
  const ph = document.getElementById("accPhone").value.trim();
  if(!ph){ document.getElementById("otpSentNote").textContent = "Enter phone first."; return; }
  const code = Math.floor(1000 + Math.random()*9000).toString();
  st.otpCode = code;
  document.getElementById("otpSentNote").textContent = "Test OTP (for demo): " + code;
}
function verifyOTP(){
  const code = document.getElementById("accOTP").value.trim();
  const name = document.getElementById("accName").value.trim() || "Player";
  const phone = document.getElementById("accPhone").value.trim();
  if(!st.otpCode){ document.getElementById("accNote").textContent = "Send code first."; return; }
  if(code !== st.otpCode){ document.getElementById("accNote").textContent = "Invalid code."; return; }
  st.user = {name, phone};
  localStorage.setItem("glad_user", JSON.stringify(st.user));
  document.getElementById("accNote").textContent = "Signed in as " + name;
  st.otpCode = null;
}

/* =========================
   Admin
========================= */
function unlockAdmin(){
  const pin = document.getElementById("adminPIN").value.trim();
  if(pin === ADMIN_PIN){
    st.adminUnlocked = true;
    document.getElementById("adminPanel").style.display = "block";
    document.getElementById("adminNote").textContent = "Admin unlocked.";
    // preload fields
    document.getElementById("ytNameInp").value = st.socials.ytName;
    document.getElementById("ytLinkInp").value = st.socials.ytLink;
    document.getElementById("igNameInp").value = st.socials.igName;
    document.getElementById("igLinkInp").value = st.socials.igLink;
    renderMusic();
  }else{
    document.getElementById("adminNote").textContent = "Wrong PIN.";
  }
}
function postVideos(){
  if(!st.adminUnlocked) return;
  const ytName = document.getElementById("ytNameInp").value.trim() || "YouTube";
  const ytLink = document.getElementById("ytLinkInp").value.trim() || "#";
  const igName = document.getElementById("igNameInp").value.trim() || "Instagram";
  const igLink = document.getElementById("igLinkInp").value.trim() || "#";
  st.socials = {ytName, ytLink, igName, igLink};
  localStorage.setItem("glad_socials", JSON.stringify(st.socials));
  st.posted = true;
  refreshSocials();
  alert("Gladiator posted new videos. A notice is shown on Home.");
}
function addMusic(){
  if(!st.adminUnlocked) return;
  const f = document.getElementById("musicFile").files[0];
  if(!f){ alert("Choose an audio file."); return; }
  const url = URL.createObjectURL(f);
  const name = f.name;
  st.music.unshift({name, url});
  localStorage.setItem("glad_music", JSON.stringify(st.music));
  renderMusic();
}
function renderMusic(){
  const list = document.getElementById("musicList");
  list.innerHTML = "";
  st.music.forEach((m, i)=>{
    const wrap = document.createElement("div");
    wrap.className="msg";
    wrap.innerHTML = `<div style="font-weight:700">${m.name}</div>
      <audio controls style="width:100%; margin-top:6px" src="${m.url}"></audio>`;
    list.appendChild(wrap);
  });
}

/* =========================
   AI (simple offline)
========================= */
function askAI(){
  const q = document.getElementById("aiIn").value.trim();
  if(!q) return;
  const out = document.getElementById("aiOut");
  const me = document.createElement("div");
  me.className="msg";
  me.innerHTML = `<div style="font-weight:700">You</div><div style="margin-top:6px">${q}</div>`;
  out.prepend(me);
  // Simple canned logic
  let a = "I’m here. Tell me which game and your region/time.";
  const s = q.toLowerCase();
  if(s.includes("time")||s.includes("when")) a = "I’m available most evenings. Propose a time and game mode.";
  if(s.includes("cod")||s.includes("call of duty")) a = "COD Mobile: I usually play MP ranked and BR. Drop your ID.";
  if(s.includes("pubg")) a = "PUBG Mobile: squad preferred, hot drop or safe rotation?";
  if(s.includes("delta")) a = "Delta Force: classic modes; we can run tactical missions.";
  const bot = document.createElement("div");
  bot.className="msg";
  bot.innerHTML = `<div style="font-weight:700">AI</div><div style="margin-top:6px">${a}</div>`;
  out.prepend(bot);
}
function clearAI(){
  document.getElementById("aiIn").value="";
  document.getElementById("aiOut").innerHTML="";
}

/* =========================
   Utilities
========================= */
function fmtTime(ts){
  const d = new Date(ts);
  return d.toLocaleString();
}

/* =========================
   Keyboard hint (optional)
========================= */
document.addEventListener("keydown",(e)=>{
  if(e.key==="1") setTab("home");
  if(e.key==="2") setTab("about");
  if(e.key==="3") setTab("contact");
  if(e.key==="4") setTab("account");
});

</script>
</body>
</html>
