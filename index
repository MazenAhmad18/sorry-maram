<!DOCTYPE html>
<html lang="ar">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>اعتذار لمرام</title>

<style>
body{
    margin:0;
    background:black;
    overflow:hidden;
    display:flex;
    justify-content:center;
    align-items:center;
    height:100vh;
    color:white;
    font-family:Arial;
    text-align:center;
}

button{
    padding:15px 30px;
    font-size:22px;
    background:#ff2e63;
    color:white;
    border:none;
    border-radius:30px;
    cursor:pointer;
    transition:.3s;
}

button:hover{
    transform:scale(1.1);
}

#message{
    margin-top:25px;
    font-size:24px;
    max-width:500px;
    line-height:1.8;
}

/* قلوب */
.heart{
    position:absolute;
    font-size:20px;
    animation:float 6s linear infinite;
}

@keyframes float{
    0%{transform:translateY(100vh);opacity:0;}
    50%{opacity:1;}
    100%{transform:translateY(-10vh);opacity:0;}
}
</style>
</head>

<body>

<div>
<button onclick="start()">اضغط هنا يا مرام ❤️</button>
<div id="message"></div>
</div>

<script>
let text = "مرام… أنا آسف لو زعلتك 💔 وجودك مهم عندي وبتمنى تسامحيني ❤️";
let i = 0;

function start(){
    typeWriter();
    document.querySelector("button").style.display="none";
}

function typeWriter(){
    if(i < text.length){
        document.getElementById("message").innerHTML += text.charAt(i);
        i++;
        setTimeout(typeWriter, 70);
    }
}

/* قلوب متحركة */
setInterval(()=>{
    let heart = document.createElement("div");
    heart.classList.add("heart");
    heart.innerHTML="❤️";
    heart.style.left=Math.random()*100+"vw";
    heart.style.fontSize=(Math.random()*20+10)+"px";
    document.body.appendChild(heart);
    setTimeout(()=>{heart.remove()},6000);
},400);
</script>

</body>
</html>
