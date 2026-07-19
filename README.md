<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Sorry Mai ❤️</title>
<style>
*{margin:0;padding:0;box-sizing:border-box;font-family:'Segoe UI',sans-serif}
body{
background:linear-gradient(135deg,#ff9ec4,#ffc3d9,#ffe8f1);
display:flex;justify-content:center;align-items:center;
min-height:100vh;padding:20px;overflow-x:hidden;
}
.container{
width:100%;max-width:700px;
background:rgba(255,255,255,.2);
backdrop-filter:blur(18px);
border-radius:25px;padding:40px;text-align:center;color:#fff;
box-shadow:0 15px 40px rgba(0,0,0,.2);animation:fade 2s;
}
h1{font-size:48px;margin-bottom:15px}
h2{margin-bottom:25px}
p{font-size:20px;line-height:1.9}
button{
margin-top:35px;padding:15px 35px;border:none;border-radius:40px;
font-size:18px;cursor:pointer;background:#fff;color:#ff3f86;
transition:.3s;font-weight:bold}
button:hover{transform:scale(1.05);background:#ff3f86;color:#fff}
#hidden{display:none;margin-top:25px;font-size:22px}
@keyframes fade{from{opacity:0;transform:translateY(20px)}to{opacity:1;transform:translateY(0)}}
.heart{position:fixed;color:#ff2d75;animation:float linear infinite;opacity:.8;pointer-events:none}
@keyframes float{from{transform:translateY(110vh) scale(.5)}to{transform:translateY(-10vh) scale(1.5)}}
@media(max-width:768px){
.container{padding:24px 18px}
h1{font-size:34px}
h2{font-size:24px}
p{font-size:17px}
button{width:100%}
#hidden{font-size:18px}
}
</style>
</head>
<body>
<div class="container">
<h1>❤️ Dear Mai ❤️</h1>
<h2>I'm Truly Sorry...</h2>
<p>
Mai...<br><br>
Sometimes words come too late, but feelings never do.<br><br>
If I hurt your heart, even a little, I sincerely apologize.<br><br>
You are someone very special, and seeing you upset because of me is something I never wanted.<br><br>
I can't change what happened, but I promise I can be better.<br>
I hope you can forgive me and let your beautiful smile return again.<br><br>
Thank you for being you. ❤️
</p>
<button onclick="showMessage()">Click Here ❤️</button>
<div id="hidden">💖 Mai...<br><br>I hope this little surprise brings a smile to your face. 🌹❤️</div>
</div>
<script>
function showMessage(){document.getElementById('hidden').style.display='block';}
function createHeart(){
const h=document.createElement('div');
h.className='heart';
h.innerHTML='❤';
h.style.left=Math.random()*100+'vw';
h.style.fontSize=(20+Math.random()*30)+'px';
h.style.animationDuration=(4+Math.random()*6)+'s';
document.body.appendChild(h);
setTimeout(()=>h.remove(),10000);
}
setInterval(createHeart,250);
</script>
</body>
</html>
