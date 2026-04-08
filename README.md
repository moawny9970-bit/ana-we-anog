<!DOCTYPE html>
<html lang="ar">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>A ❤️ E</title>

<style>

/* إعدادات عامة */
body {
margin:0;
font-family: 'Cairo', sans-serif;
background: linear-gradient(135deg,#ff9a9e,#fad0c4);
overflow-x:hidden;
color:white;
text-align:center;
}

/* قلوب الخلفية */
.heart {
position:fixed;
font-size:14px;
animation: float 10s linear infinite;
opacity:.7;
}

@keyframes float {
0% {transform: translateY(100vh);}
100% {transform: translateY(-10vh);}
}

/* الصفحات */
.page {
display:none;
min-height:100vh;
padding:20px;
justify-content:center;
align-items:center;
flex-direction:column;
}

.show {
display:flex;
}

/* الظرف */
.envelope {
background:white;
color:#ff4b5c;
padding:30px;
border-radius:20px;
box-shadow:0 0 25px rgba(0,0,0,.2);
width:90%;
max-width:320px;
}

.envelope h2 {
margin-bottom:15px;
}

input {
padding:12px;
border-radius:10px;
border:none;
font-size:16px;
width:100%;
margin-bottom:15px;
text-align:center;
}

button {
padding:12px 20px;
border:none;
border-radius:12px;
background:#ff4b5c;
color:white;
font-size:16px;
cursor:pointer;
}

/* الرسالة */
.message-box {
background: rgba(255,255,255,.2);
padding:25px;
border-radius:20px;
max-width:500px;
backdrop-filter: blur(10px);
font-size:18px;
line-height:1.8;
}

/* الصور */
.slideshow {
position:relative;
width:90%;
max-width:350px;
height:450px;
margin:auto;
}

.slideshow img {
position:absolute;
width:100%;
height:100%;
object-fit:cover;
border-radius:20px;
opacity:0;
animation: slideShow 50s infinite;
}

.slideshow img:nth-child(1){animation-delay:0s;}
.slideshow img:nth-child(2){animation-delay:5s;}
.slideshow img:nth-child(3){animation-delay:10s;}
.slideshow img:nth-child(4){animation-delay:15s;}
.slideshow img:nth-child(5){animation-delay:20s;}
.slideshow img:nth-child(6){animation-delay:25s;}
.slideshow img:nth-child(7){animation-delay:30s;}
.slideshow img:nth-child(8){animation-delay:35s;}
.slideshow img:nth-child(9){animation-delay:40s;}
.slideshow img:nth-child(10){animation-delay:45s;}

@keyframes slideShow {
0% {opacity:0; transform:scale(1);}
5% {opacity:1;}
10% {opacity:1; transform:scale(1.05);}
15% {opacity:0;}
100% {opacity:0;}
}

/* الفيديو */
.video-box {
margin-top:20px;
border-radius:20px;
overflow:hidden;
box-shadow:0 0 20px rgba(0,0,0,.4);
}

/* العداد */
.timer {
display:flex;
gap:10px;
justify-content:center;
flex-wrap:wrap;
margin-top:20px;
}

.time-box {
background:white;
color:#ff4b5c;
padding:15px;
border-radius:15px;
min-width:80px;
box-shadow:0 0 15px rgba(0,0,0,.2);
}

.time-box span {
display:block;
font-size:28px;
font-weight:bold;
}

.label {
font-size:14px;
}

</style>
</head>

<body>

<!-- قلوب -->
<script>
for(let i=0;i<25;i++){
let h=document.createElement("div");
h.className="heart";
h.innerHTML="A ❤️ E";
h.style.left=Math.random()*100+"%";
h.style.animationDuration=(6+Math.random()*6)+"s";
document.body.appendChild(h);
}
</script>

<!-- الصفحة 1 -->
<div class="page show" id="page1">

<div class="envelope">
<h2>اكتب الباسورد ✉️</h2>

<input type="password" id="pass">

<button onclick="checkPass()">فتح</button>

</div>

</div>

<!-- الصفحة 2 -->
<div class="page" id="page2">

<div class="message-box">

يا سنفورتي الجميلة ❤️  

الموقع ده معمول علشان يفضل ذكرى لينا احنا الاتنين…  
من أول يوم اتعرفنا فيه يوم **30 / 6 / 2023**  
والدنيا بقت أحلى بوجودك فيها.  

كل خروجة خرجناها…  
كل ضحكة…  
كل هزار بينا…  
كل لحظة كنتي فيها جنبي  
فضلت محفورة جوايا.  

انتي مش بس حد في حياتي…  
انتي حتة من يومي…  
من مزاجي…  
من ضحكتي.  

وأنا مبسوط إن كل الحاجات الحلوة دي كانت معاكي انتي بالذات.  

الموقع ده معمول علشان كل ما تفتحيه  
تفتكري إن في حد فرحان بوجودك في حياته  
وإن الذكريات اللي بينا  
غالية عندي جدًا.  

<button onclick="nextPage(3)">التالي</button>

</div>

</div>

<!-- الصفحة 3 -->
<div class="page" id="page3">

<audio autoplay controls loop>
<source src="song.mp3">
</audio>

<div class="slideshow">

<img src="Snapchat-568583960.jpg">
<img src="Snapchat-185811932.jpg">
<img src="Picsart_26-03-27_21-10-29-947.jpg">
<img src="IMG-20260327-WA0091.jpg">
<img src="IMG-20260326-WA0211.jpg">
<img src="IMG-20260326-WA0150.jpg">
<img src="IMG-20260326-WA0115(1).jpg">
<img src="IMG-20260326-WA0084(1).jpg">
<img src="IMG-20260326-WA0074.jpg">
<img src="Snapchat-697868569.jpg">

</div>

<div class="video-box">

<video width="100%" controls>
<source src="VID-20260327-WA0023.mp4">
</video>

</div>

<button onclick="nextPage(4)">التالي</button>

</div>

<!-- الصفحة 4 -->
<div class="page" id="page4">

<h2>الوقت اللي قضيناه مع بعض ⏳</h2>

<div class="timer">

<div class="time-box">
<span id="days">0</span>
<div class="label">يوم</div>
</div>

<div class="time-box">
<span id="hours">0</span>
<div class="label">ساعة</div>
</div>

<div class="time-box">
<span id="minutes">0</span>
<div class="label">دقيقة</div>
</div>

<div class="time-box">
<span id="seconds">0</span>
<div class="label">ثانية</div>
</div>

</div>

</div>

<script>

/* الباسورد */

function checkPass(){

let p=document.getElementById("pass").value;

if(p==="22/12"){

nextPage(2);

}else{

alert("الباسورد غلط");

}

}

/* التنقل */

function nextPage(n){

document.querySelectorAll(".page")
.forEach(p=>p.classList.remove("show"));

document.getElementById("page"+n)
.classList.add("show");

}

/* العداد */

let startDate=new Date("June 30, 2023 00:00:00");

setInterval(()=>{

let now=new Date();

let diff=now-startDate;

let days=Math.floor(diff/(1000*60*60*24));

let hours=Math.floor(
(diff%(1000*60*60*24))/(1000*60*60)
);

let minutes=Math.floor(
(diff%(1000*60*60))/(1000*60)
);

let seconds=Math.floor(
(diff%(1000*60))/1000
);

document.getElementById("days").innerText=days;
document.getElementById("hours").innerText=hours;
document.getElementById("minutes").innerText=minutes;
document.getElementById("seconds").innerText=seconds;

},1000);

</script>

</body>
</html>
