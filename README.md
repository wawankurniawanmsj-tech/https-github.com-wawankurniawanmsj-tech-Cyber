<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ardian - Website Pribadi Profesional</title>

    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;700&display=swap" rel="stylesheet">

    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: "Poppins", sans-serif;
        }

        body {
            background: #0f0f17;
            color: #fff;
            overflow-x: hidden;
        }

        /* ---- Background Partikel ---- */
        #particles-js {
            position: fixed;
            width: 100%;
            height: 100%;
            z-index: -10;
            top: 0;
            left: 0;
        }

        /* ---- Header ---- */
        header {
            text-align: center;
            padding: 110px 20px 80px;
            animation: fadeIn 1.4s ease;
        }

        header h1 {
            font-size: 58px;
            font-weight: 700;
            background: linear-gradient(45deg, #8a2be2, #00eaff, #ff00ff);
            -webkit-background-clip: text;
            color: transparent;
            animation: glow 3s infinite;
        }

        @keyframes glow {
            0% { text-shadow: 0 0 15px #8a2be2; }
            50% { text-shadow: 0 0 40px #00eaff; }
            100% { text-shadow: 0 0 15px #ff00ff; }
        }

        header p {
            font-size: 20px;
            opacity: 0.8;
            margin-top: 10px;
        }

        /* ---- Navbar ---- */
        nav {
            backdrop-filter: blur(10px);
            background: rgba(255,255,255,0.05);
            padding: 12px;
            display: flex;
            justify-content: center;
            gap: 40px;
            position: sticky;
            top: 0;
            z-index: 50;
            border-bottom: 1px solid rgba(255,255,255,0.08);
        }

        nav a {
            color: #fff;
            text-decoration: none;
            font-weight: 600;
            letter-spacing: 1px;
            transition: 0.3s;
        }

        nav a:hover {
            color: #00eaff;
        }

        /* ---- Sections ---- */
        section {
            padding: 70px 20px;
            max-width: 950px;
            margin: auto;
            animation: fadeUp 1s ease;
        }

        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(30px); }
            to { opacity: 1; transform: translateY(0); }
        }

        @keyframes fadeUp {
            from { opacity: 0; transform: translateY(40px); }
            to { opacity: 1; transform: translateY(0); }
        }

        .card {
            background: rgba(255,255,255,0.05);
            padding: 30px;
            border-radius: 16px;
            backdrop-filter: blur(12px);
            border: 1px solid rgba(255,255,255,0.1);
            box-shadow: 0 0 20px rgba(0,255,255,0.1);
            transition: 0.4s;
        }

        .card:hover {
            transform: translateY(-10px);
            box-shadow: 0 0 35px rgba(0,255,255,0.3);
        }

        h2 {
            font-size: 32px;
            margin-bottom: 15px;
            background: linear-gradient(45deg,#00eaff,#a020f0);
            -webkit-background-clip: text;
            color: transparent;
            font-weight: 700;
        }

        ul li {
            margin-bottom: 8px;
            opacity: 0.9;
        }

        /* --- Button --- */
        .btn {
            display: inline-block;
            padding: 14px 22px;
            background: #00eaff;
            color: #000;
            text-decoration: none;
            margin-top: 20px;
            border-radius: 10px;
            font-weight: 700;
            transition: 0.3s;
        }

        .btn:hover {
            background: #00bcd4;
            transform: translateY(-3px);
        }

        /* ---- Footer ---- */
        footer {
            text-align: center;
            padding: 30px;
            background: rgba(255,255,255,0.05);
            border-top: 1px solid rgba(255,255,255,0.1);
            backdrop-filter: blur(5px);
            margin-top: 40px;
            font-size: 15px;
            color: #ccc;
        }
    </style>
</head>

<body>

<!-- Background Partikel -->
<div id="particles-js"></div>

<header>
    <h1>Ardian</h1>
    <p>Siswa SMA Negeri 2 Punduh Pedada • Portfolio Pribadi</p>
</header>

<nav>
    <a href="#tentang">Tentang</a>
    <a href="#proyek">Proyek</a>
    <a href="#kontak">Kontak</a>
</nav>

<section id="tentang">
    <div class="card">
        <h2>Tentang Saya</h2>
        <p>Halo! Saya Ardian, seorang siswa dari <b>SMA Negeri 2 Punduh Pedada</b>. 
        Saya tertarik dengan teknologi, desain modern, serta pembuatan website. 
        Website ini adalah tempat saya membagikan karya, aktivitas, dan perjalanan saya.</p>
    </div>
</section>

<section id="proyek">
    <div class="card">
        <h2>Proyek Saya</h2>
        <p>Beberapa proyek kreatif yang saya kerjakan:</p>
        <ul>
            <li>Website Modern & Portfolio</li>
            <li>Desain UI/UX Glow Futuristic</li>
            <li>Mini Aplikasi Web</li>
            <li>Project Kreatif Sekolah</li>
            <li>Editing Konten Digital</li>
        </ul>
    </div>
</section>

<section id="kontak">
    <div class="card">
        <h2>Kontak</h2>
        <p>Ingin menghubungi saya? Klik tombol di bawah ini.</p>
        <a class="btn" href="https://wa.me/628xxxxxxxxxx" target="_blank">WhatsApp Saya</a>
    </div>
</section>

<footer>
    © 2025 Ardian • Portfolio Premium Glow Edition
</footer>

<!-- Particles.js -->
<script src="https://cdn.jsdelivr.net/npm/particles.js@2.0.0/particles.min.js"></script>
<script>
particlesJS("particles-js", {
  "particles": {
    "number": { "value": 85 },
    "size": { "value": 3 },
    "color": { "value": "#00eaff" },
    "line_linked": { "enable": true, "color": "#00eaff" },
    "move": { "speed": 2 }
  }
});
</script>

</body>
</html>






<!DOCTYPE html>
<html lang="id">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Cyber Security Dashboard</title>

<link href="https://fonts.googleapis.com/css2?family=Share+Tech+Mono&display=swap" rel="stylesheet">

<style>
*{margin:0;padding:0;box-sizing:border-box}
body{
  background:black;
  color:#00ff9c;
  font-family:'Share Tech Mono',monospace;
  overflow:hidden;
}

/* MATRIX */
canvas{
  position:fixed;
  top:0;left:0;
  width:100%;
  height:100%;
  z-index:-1;
}

/* LOGIN */
#login{
  width:320px;
  margin:120px auto;
  padding:25px;
  border:1px solid #00ff9c;
  box-shadow:0 0 25px #00ff9c;
  text-align:center;
  background:rgba(0,0,0,0.8);
}
#login h2{margin-bottom:15px}
#login input{
  width:100%;
  padding:10px;
  margin:8px 0;
  background:black;
  border:1px solid #00ff9c;
  color:#00ff9c;
}
#login button{
  width:100%;
  padding:10px;
  background:#00ff9c;
  border:none;
  cursor:pointer;
  font-weight:bold;
}

/* DASHBOARD */
#dashboard{display:none;height:100vh}

.sidebar{
  width:220px;
  height:100vh;
  background:#020202;
  border-right:1px solid #00ff9c;
  padding:20px;
  position:fixed;
}
.sidebar h2{text-align:center;margin-bottom:20px}
.sidebar a{
  display:block;
  padding:10px;
  color:#00ff9c;
  text-decoration:none;
  border-bottom:1px solid #003322;
}
.sidebar a:hover{
  background:#00ff9c;
  color:black;
}

.main{
  margin-left:220px;
  padding:20px;
}

/* TERMINAL */
.terminal{
  background:#010101;
  padding:15px;
  height:220px;
  overflow:auto;
  border:1px solid #00ff9c;
  box-shadow:0 0 15px #00ff9c;
}
.terminal span{
  display:block;
  line-height:1.6;
}

/* CARDS */
.cards{
  display:grid;
  grid-template-columns:repeat(auto-fit,minmax(200px,1fr));
  gap:15px;
  margin-top:20px;
}
.card{
  background:#020202;
  padding:15px;
  border:1px solid #00ff9c;
  box-shadow:0 0 10px #00ff9c;
}
.card h3{margin-bottom:10px}

footer{
  text-align:center;
  margin-top:20px;
  font-size:0.8em;
  color:#00aa66;
}
</style>
</head>

<body>

<canvas id="matrix"></canvas>

<!-- LOGIN -->
<div id="login">
  <h2>MEMBER LOGIN</h2>
  <h2>Community Security Cyber</h2>
  <input type="text" id="user" placeholder="Username">
  <input type="password" id="pass" placeholder="Password">
  <button onclick="login()">ACCESS</button>
</div>

<!-- DASHBOARD -->
<div id="dashboard">
  <div class="sidebar">
    <h2>CSC PANEL</h2>
    <a href="#">Dashboard</a>
    <a href="#">Recon Tools</a>
    <a href="#">Pentest Lab</a>
    <a href="#">Crypto Module</a>
    <a href="#">System Logs</a>
    <a href="#" onclick="logout()">Logout</a>
  </div>

  <div class="main">
    <h1>WELCOME, OPERATOR</h1>
    <p>Status System: <span style="color:#0f0">SECURE</span></p>

    <div class="terminal" id="terminal"></div>

    <div class="cards">
      <div class="card">
        <h3>🛡 Firewall</h3>
        <p>Status: ACTIVE</p>
      </div>
      <div class="card">
        <h3>🌐 Network</h3>
        <p>Encrypted Tunnel</p>
      </div>
      <div class="card">
        <h3>🔍 Scanner</h3>
        <p>Idle</p>
      </div>
      <div class="card">
        <h3>📡 Monitoring</h3>
        <p>Running</p>
      </div>
    </div>

    <footer>© 2025 Cyber Security Community</footer>
  </div>
</div>

<script>
// ELEMENT
const loginBox = document.getElementById("login");
const dashboard = document.getElementById("dashboard");
const terminal = document.getElementById("terminal");
const user = document.getElementById("user");
const pass = document.getElementById("pass");

// LOGIN
function login(){
  if(user.value === "admin" && pass.value === "admin123"){
    loginBox.style.display="none";
    dashboard.style.display="block";
    startTerminal();
  }else{
    alert("ACCESS DENIED");
  }
}
function logout(){ location.reload(); }

// TERMINAL EFFECT
const logs=[
  "[+] Booting cyber modules...",
  "[+] Initializing firewall...",
  "[+] Establishing secure shell...",
  "[+] Encrypted tunnel active",
  "[✓] System fully operational"
];
let i=0;
function startTerminal(){
  const interval=setInterval(()=>{
    if(i<logs.length){
      const line=document.createElement("span");
      line.textContent=logs[i++];
      terminal.appendChild(line);
      terminal.scrollTop=terminal.scrollHeight;
    }else clearInterval(interval);
  },700);
}

// MATRIX EFFECT
const c=document.getElementById("matrix");
const ctx=c.getContext("2d");
c.width=innerWidth;
c.height=innerHeight;

const chars="01X#@$%&";
const fontSize=14;
const columns=c.width/fontSize;
const drops=Array(Math.floor(columns)).fill(1);

setInterval(()=>{
  ctx.fillStyle="rgba(0,0,0,0.05)";
  ctx.fillRect(0,0,c.width,c.height);
  ctx.fillStyle="#00ff9c";
  ctx.font=fontSize+"px monospace";

  drops.forEach((y,i)=>{
    const text=chars[Math.floor(Math.random()*chars.length)];
    ctx.fillText(text,i*fontSize,y*fontSize);
    if(y*fontSize>c.height && Math.random()>0.975) drops[i]=0;
    drops[i]++;
  });
},35);
</script>

</body>
</html>






