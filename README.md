
<!DOCTYPE html>
<html lang="hi">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>For Zuveriya ❤️</title>
<style>
*{margin:0;padding:0;box-sizing:border-box}
body{
 background:radial-gradient(circle,#54204e,#160d27);
 color:white;font-family:Georgia,serif;
 min-height:100vh;overflow:hidden;
 display:flex;align-items:center;justify-content:center;
 text-align:center;
}
.scene{width:100%;padding:20px}
h1{color:#ffb6df;margin-bottom:20px}
.panda{
 font-size:110px;
 animation:bounce 2s infinite;
 filter:drop-shadow(0 10px 20px #ff7acb);
}
@keyframes bounce{
 0%,100%{transform:translateY(0) rotate(-5deg)}
 50%{transform:translateY(-22px) rotate(5deg)}
}
button{
 background:#ff70bd;color:white;border:0;
 padding:14px 25px;border-radius:30px;
 font-size:17px;margin-top:25px;
}
#message{font-size:19px;line-height:1.8;margin-top:20px}
.heart{
 position:absolute;bottom:-30px;
 animation:float 6s linear infinite;
}
@keyframes float{
 to{transform:translateY(-110vh) rotate(360deg);opacity:0}
}
</style>
</head>
<body>
<div class="scene">
<h1>For My Rasmalai ❤️</h1>
<div class="panda">🐼</div>
<div id="message">Aapke liye ek chhota sa surprise hai... ❤️</div>
<br>
<button onclick="start()">Surprise dekho ❤️</button>
</div>

<script>
function start(){
 const msg=document.getElementById("message");
 msg.innerHTML="Hiii Zuveriya! 🥰<br><br>";
 setTimeout(()=>{
 msg.innerHTML+='I love you too! ❤️<br><br>Aapke liye aapke betu ne ek pyaari si shayari likhi hai...';
 },1500);
 setTimeout(()=>{
 msg.innerHTML+=' <br><br>Aapki muskurahat meri jaan hai,<br>Aap meri har khushi ki pehchaan hai,<br>Door rehkar bhi dil ke paas ho aap,<br>Meri duniya ka sabse pyaara ehsaas ho aap. ❤️';
 },4500);
}
setInterval(()=>{
 let h=document.createElement("div");
 h.className="heart";
 h.innerHTML="❤️";
 h.style.left=Math.random()*100+"%";
 h.style.animationDuration=(4+Math.random()*4)+"s";
 document.body.appendChild(h);
 setTimeout(()=>h.remove(),8000);
},500);
</script>
</body>
</html>
