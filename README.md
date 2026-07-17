<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>SocialJump</title>

<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;700&display=swap" rel="stylesheet">

<style>
*{
margin:0;
padding:0;
box-sizing:border-box;
font-family:'Poppins',sans-serif;
}

body{
background:#0f172a;
color:#fff;
overflow:hidden;
}

.screen{
width:100%;
height:100vh;
display:flex;
justify-content:center;
align-items:center;
flex-direction:column;
position:absolute;
top:0;
left:0;
transition:.5s;
}

.logo{
font-size:45px;
font-weight:700;
color:#00e5ff;
animation:zoom 2s infinite;
}

.tagline{
margin-top:10px;
font-size:18px;
opacity:.8;
}

button{
padding:14px 35px;
border:none;
border-radius:30px;
background:#00e5ff;
color:#000;
font-size:18px;
font-weight:600;
cursor:pointer;
margin-top:30px;
}

@keyframes zoom{
0%{transform:scale(.8);}
50%{transform:scale(1);}
100%{transform:scale(.8);}
}

.hidden{
display:none;
}
</style>
</head>

<body>

<div id="splash" class="screen">
<h1 class="logo">SocialJump</h1>
<p class="tagline">Connect • Share • Grow</p>
</div>

<div id="welcome" class="screen hidden">
<h1>Welcome to SocialJump</h1>
<p>Create • Chat • Reels • Friends</p>

<button onclick="startApp()">
Get Started
</button>
</div>

<script>
setTimeout(()=>{
document.getElementById("splash").classList.add("hidden");
document.getElementById("welcome").classList.remove("hidden");
},3000);

function startApp(){
alert("Onboarding Screen Coming...");
}
</script>

</body>
</html>
