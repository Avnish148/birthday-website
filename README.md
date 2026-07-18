<!DOCTYPE html>
<html><head><meta charset="UTF-8"><meta name="viewport" content="width=device-width,initial-scale=1">
<title>Birthday Surprise</title>
<style>
body{margin:0;font-family:Arial;background:linear-gradient(135deg,#6a11cb,#2575fc);color:#fff;overflow:hidden}
.page{display:none;height:100vh;justify-content:center;align-items:center;flex-direction:column;text-align:center}
#p1{display:flex}
.card{background:rgba(255,255,255,.15);padding:30px;border-radius:20px;backdrop-filter:blur(8px)}
button{padding:12px 28px;border:none;border-radius:30px;font-size:18px;cursor:pointer}
h1{font-size:48px}
#timer{font-size:32px;margin:20px}
</style></head>
<body>
<div id="p1" class="page">
<div class="card">
<h1>Welcome To My Website</h1>
<h2>Made by Avnish ❤️</h2>
<button onclick="showPage()">Next ➜</button>
</div></div>
<div id="p2" class="page">
<div class="card">
<h1>🎉 Happy Birthday Aman 🎂</h1>
<div id="timer"></div>
<p>Advance Happy Birthday Bro! 🥳❤️</p>
</div></div>
<script>
function showPage(){document.getElementById('p1').style.display='none';document.getElementById('p2').style.display='flex';}
const target=new Date("2026-08-06T00:00:00").getTime();
setInterval(()=>{
let d=target-Date.now();
if(d<=0){timer.innerHTML="🎉 Happy Birthday Aman!";return;}
let days=Math.floor(d/86400000);
let hrs=Math.floor(d%86400000/3600000);
let mins=Math.floor(d%3600000/60000);
let secs=Math.floor(d%60000/1000);
timer.innerHTML=`${days} Days ${hrs} Hours ${mins} Minutes ${secs} Seconds`;
},1000);
</script>
</body></html>
