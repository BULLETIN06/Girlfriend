<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Happy Girlfriend's Day ❤️</title>

<link href="https://fonts.googleapis.com/css2?family=Cinzel:wght@600;700&family=Poppins:wght@300;500&display=swap" rel="stylesheet">

<style>
*{
margin:0;
padding:0;
box-sizing:border-box;
}

body{
overflow:hidden;
font-family:Poppins,sans-serif;
background:#000;
color:#fff;
}

video{
position:fixed;
top:0;
left:0;
width:100%;
height:100%;
object-fit:cover;
z-index:-3;
filter:brightness(.35);
}

.overlay{
position:fixed;
inset:0;
background:radial-gradient(circle,transparent,#000);
z-index:-2;
}

.stars{
position:absolute;
width:100%;
height:100%;
background:url("https://i.imgur.com/6QJjYMe.png");
animation:move 120s linear infinite;
opacity:.5;
}

@keyframes move{
from{transform:translateY(0);}
to{transform:translateY(-2000px);}
}

.intro{
position:absolute;
width:100%;
height:100%;
display:flex;
justify-content:center;
align-items:center;
flex-direction:column;
text-align:center;
animation:intro 10s forwards;
}

.intro h1{
font-family:Cinzel;
font-size:65px;
letter-spacing:6px;
text-shadow:0 0 25px gold;
}

.intro p{
margin-top:15px;
font-size:22px;
color:#ddd;
}

@keyframes intro{
0%{opacity:0;transform:scale(.6);}
20%{opacity:1;}
80%{opacity:1;}
100%{opacity:0;transform:scale(1.8);}
}

.main{
position:absolute;
width:100%;
height:100%;
display:flex;
justify-content:center;
align-items:center;
flex-direction:column;
text-align:center;
opacity:0;
animation:appear 4s forwards;
animation-delay:10s;
padding:30px;
}

@keyframes appear{
to{opacity:1;}
}

.name{
font-family:Cinzel;
font-size:60px;
color:#FFD700;
text-shadow:0 0 20px gold;
margin-bottom:20px;
}

.text{
max-width:900px;
font-size:24px;
line-height:1.8;
animation:float 4s ease-in-out infinite;
}

@keyframes float{
50%{transform:translateY(-10px);}
}

button{
margin-top:40px;
padding:18px 40px;
font-size:20px;
border:none;
border-radius:40px;
cursor:pointer;
background:#FFD700;
font-weight:bold;
transition:.4s;
}

button:hover{
transform:scale(1.08);
box-shadow:0 0 25px gold;
}

#letter{
display:none;
margin-top:40px;
max-width:900px;
font-size:22px;
line-height:2;
animation:fade 2s;
}

@keyframes fade{
from{opacity:0;transform:translateY(40px);}
to{opacity:1;transform:translateY(0);}
}

.heart{
position:absolute;
color:#ff4d6d;
animation:rise linear infinite;
}

@keyframes rise{
0%{
transform:translateY(100vh);
opacity:0;
}
20%{
opacity:1;
}
100%{
transform:translateY(-120vh);
opacity:0;
}
}
</style>
</head>

<body>

<!-- Replace movie.mp4 with your cinematic background -->
<video autoplay muted loop>
<source src="movie.mp4" type="video/mp4">
</video>

<div class="overlay"></div>
<div class="stars"></div>

<!-- Intro -->
<div class="intro">
<h1>HAPPY GIRLFRIEND'S DAY</h1>
<p>A Love Story Written By Destiny ❤️</p>
</div>

<!-- Main -->
<div class="main">

<div class="name">For My Beautiful Queen ❤️</div>

<div class="text">
Some people spend their whole lives searching for someone who makes their heart feel at home.

I never have to search...

Because I found you.

You are my peace when life becomes loud.

You are my happiness when days become dark.

You are the smile I never want to lose.

You are the most beautiful chapter of my life.
</div>

<button onclick="openLetter()">Open My Heart ❤️</button>

<div id="letter">

My Love,

If I had one wish...

I'd relive every moment with you over and over again.

Your smile heals me.

Your voice calms me.

Your love changes me.

Thank you for choosing me every single day.

On this Girlfriend's Day I just want you to know...

I promise to keep loving you.

I promise to keep making you smile.

I promise to stand beside you through every chapter life writes.

And if loving you were a movie...

I'd watch it forever without ever skipping a single scene.

❤️ Happy Girlfriend's Day ❤️

Forever Yours...
</div>

</div>

<!-- Music -->
<audio id="music" autoplay loop>
<source src="perfect.mp3" type="audio/mpeg">
</audio>

<script>
window.addEventListener("click",()=>{
document.getElementById("music").play();
},{once:true});

function openLetter(){
document.getElementById("letter").style.display="block";
}

for(let i=0;i<120;i++){
let h=document.createElement("div");
h.className="heart";
h.innerHTML="❤";
h.style.left=Math.random()*100+"vw";
h.style.fontSize=(Math.random()*25+15)+"px";
h.style.animationDuration=(Math.random()*6+6)+"s";
h.style.animationDelay=Math.random()*10+"s";
document.body.appendChild(h);
}
</script>

</body>
</html>
