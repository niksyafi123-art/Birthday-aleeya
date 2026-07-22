<!DOCTYPE html>
<html>
<head>
<title>Happy Birthday 🤍</title>

<style>
*{
  box-sizing:border-box;
  font-family:'Poppins',Arial;
}

body{
  margin:0;
  height:100vh;
  display:flex;
  justify-content:center;
  align-items:center;
  background:linear-gradient(135deg,#ff758c,#ff7eb3);
  overflow:hidden;
}

.card{
  background:white;
  width:90%;
  max-width:400px;
  padding:35px;
  border-radius:30px;
  text-align:center;
  box-shadow:0 15px 40px rgba(0,0,0,.25);
  animation:pop 1s;
}

@keyframes pop{
 from{transform:scale(0)}
 to{transform:scale(1)}
}

h1{
 color:#ff477e;
 font-size:35px;
}

p{
 color:#555;
 line-height:1.6;
}

button{
 background:#ff477e;
 color:white;
 border:0;
 padding:15px 30px;
 border-radius:30px;
 font-size:16px;
 cursor:pointer;
}

#wish{
 display:none;
 margin-top:20px;
 animation:fade 1s;
}

@keyframes fade{
 from{opacity:0}
 to{opacity:1}
}

.heart{
 position:absolute;
 color:white;
 animation:fall 5s linear infinite;
}

@keyframes fall{
 from{
 transform:translateY(-100px);
 opacity:1;
 }
 to{
 transform:translateY(100vh);
 opacity:0;
 }
}
</style>

</head>

<body>

<div class="card">

<h1>🤍 Happy Birthday</h1>

<p>
Untuk seseorang yang paling saya sayang🤍
</p>

<button onclick="openWish()">
Tekan sini sayang
</button>

<div id="wish">
<h2> 🤍 HAPPY BIRTHDAY SAYANG 🤍</h2></h2>

<p>
HAPPY BIRTHDAY ALEEYA DELISHA, SYAFI SAYANG AWAK SORANG JE TAU,TADE SAPE BOLE GANTI AWAK, SEMOGA NEXT YEAR BIRTHDAY AWAK KITA MASIH BERSAMA,SAYA NAK KASI LEBIH DARI NI NNTI,BUT NOW INI JE SAYA BOLE BUAT OKAY,SAYA TAKKAN PERNAH BOSAN KATA DEKAT AWAK YANG SAYA SAYANG AWAK MUAH MUAH🤍
</p>

<p> from your fav boy(syafi)</p>
</div>

</div>


<script>

function openWish(){
document.getElementById("wish").style.display="block";
}

setInterval(()=>{
let heart=document.createElement("div");
heart.className="heart";
heart.innerHTML="🤍";
heart.style.left=Math.random()*100+"%";
heart.style.fontSize=(Math.random()*20+10)+"px";
document.body.appendChild(heart);

setTimeout(()=>{
heart.remove();
},5000);

},300);

</script>

</body>
</html>
