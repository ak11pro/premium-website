<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Ultra Premium Demo</title>

<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;500;700&display=swap" rel="stylesheet">

<style>
*{margin:0;padding:0;box-sizing:border-box;font-family:'Poppins',sans-serif;}

body{
  background: radial-gradient(circle at top, #0f172a, #020617);
  color:white;
  overflow-x:hidden;
}

/* LOADER */
.loader{
  position:fixed;
  width:100%;
  height:100%;
  background:#020617;
  display:flex;
  justify-content:center;
  align-items:center;
  z-index:9999;
}
.loader h1{
  font-size:40px;
  animation:pulse 1s infinite;
}
@keyframes pulse{
  0%{opacity:0.3}
  50%{opacity:1}
  100%{opacity:0.3}
}

/* CURSOR */
.cursor{
  width:20px;height:20px;
  border:2px solid #38bdf8;
  border-radius:50%;
  position:fixed;
  pointer-events:none;
  transform:translate(-50%,-50%);
  transition:0.1s;
  z-index:999;
}

/* NAV */
nav{
  position:fixed;
  width:100%;
  display:flex;
  justify-content:space-between;
  padding:20px 50px;
  backdrop-filter:blur(15px);
  background:rgba(255,255,255,0.05);
}
nav ul{display:flex;gap:25px;}
nav li{list-style:none;cursor:pointer;}
nav li:hover{color:#38bdf8;}

/* HERO */
.hero{
  height:100vh;
  display:flex;
  flex-direction:column;
  justify-content:center;
  align-items:center;
  text-align:center;
  position:relative;
}

.hero h1{
  font-size:65px;
  background:linear-gradient(90deg,#38bdf8,#6366f1);
  -webkit-background-clip:text;
  color:transparent;
}

.hero p{
  margin-top:20px;
  opacity:0.7;
}

.hero button{
  margin-top:30px;
  padding:12px 30px;
  border:none;
  border-radius:30px;
  background:linear-gradient(45deg,#38bdf8,#6366f1);
  cursor:pointer;
  transition:0.4s;
}
.hero button:hover{
  transform:scale(1.1) rotate(-2deg);
}

/* FLOATING BLOBS */
.blob{
  position:absolute;
  width:300px;height:300px;
  background:linear-gradient(#38bdf8,#6366f1);
  border-radius:50%;
  filter:blur(120px);
  animation:move 10s infinite alternate;
}
.blob:nth-child(1){top:10%;left:10%;}
.blob:nth-child(2){bottom:10%;right:10%;}

@keyframes move{
  to{transform:translateY(50px) translateX(50px);}
}

/* SECTION */
.section{
  padding:120px 50px;
  text-align:center;
}

.cards{
  display:flex;
  gap:20px;
  flex-wrap:wrap;
  justify-content:center;
  margin-top:50px;
}

.card{
  width:260px;
  padding:30px;
  border-radius:20px;
  background:rgba(255,255,255,0.05);
  backdrop-filter:blur(20px);
  transition:0.4s;
  transform:translateY(60px);
  opacity:0;
}

.card:hover{
  transform:translateY(-10px) scale(1.05);
  background:rgba(255,255,255,0.1);
}

/* SHOW ANIMATION */
.show{
  transform:translateY(0);
  opacity:1;
}

/* FOOTER */
footer{
  text-align:center;
  padding:40px;
  background:#020617;
}
</style>
</head>

<body>

<div class="loader"><h1>Loading...</h1></div>
<div class="cursor"></div>

<nav>
  <h2>AK Dev</h2>
  <ul>
    <li>Home</li>
    <li>Work</li>
    <li>Contact</li>
  </ul>
</nav>

<section class="hero">
  <div class="blob"></div>
  <div class="blob"></div>

  <h1>Next-Level Websites</h1>
  <p>Animations • UI/UX • Premium Designs</p>
  <button>Hire Me</button>
</section>

<section class="section">
  <h2>What I Offer</h2>

  <div class="cards">
    <div class="card">
      <h3>Modern UI</h3>
      <p>Clean & futuristic designs</p>
    </div>

    <div class="card">
      <h3>Animations</h3>
      <p>Smooth scroll & effects</p>
    </div>

    <div class="card">
      <h3>Performance</h3>
      <p>Fast & optimized code</p>
    </div>
  </div>
</section>

<footer>
  <p>© 2026 AK Dev | Fiverr Portfolio</p>
</footer>

<script>
// LOADER
window.addEventListener("load", ()=>{
  document.querySelector(".loader").style.display="none";
});

// CURSOR
const cursor = document.querySelector(".cursor");
document.addEventListener("mousemove", e=>{
  cursor.style.top = e.clientY+"px";
  cursor.style.left = e.clientX+"px";
});

// SCROLL ANIMATION
const cards = document.querySelectorAll(".card");
window.addEventListener("scroll", ()=>{
  cards.forEach(card=>{
    const top = card.getBoundingClientRect().top;
    if(top < window.innerHeight*0.85){
      card.classList.add("show");
    }
  });
});
</script>

</body>
</html>
