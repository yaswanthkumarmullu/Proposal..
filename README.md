<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Will You Marry Me? ❤️</title>

<style>
body{
    margin:0;
    font-family:Arial,sans-serif;
    background:linear-gradient(135deg,#ff758c,#ff7eb3);
    display:flex;
    justify-content:center;
    align-items:center;
    height:100vh;
    overflow:hidden;
}

.box{
    text-align:center;
    background:white;
    padding:30px;
    border-radius:20px;
    box-shadow:0 0 20px rgba(0,0,0,.2);
}

h1{
    color:#ff3366;
}

button{
    padding:12px 30px;
    font-size:18px;
    border:none;
    border-radius:10px;
    cursor:pointer;
    margin:10px;
}

#yes{
    background:#28a745;
    color:white;
}

#no{
    background:#dc3545;
    color:white;
    position:absolute;
}
</style>
</head>

<body>

<div class="box">
<h1>Will You Marry Me? ❤️</h1>
<button id="yes">Yes ❤️</button>
<button id="no">No 💔</button>
</div>

<script>
const no=document.getElementById("no");

function moveButton(){
const x=Math.random()*(window.innerWidth-120);
const y=Math.random()*(window.innerHeight-60);

no.style.left=x+"px";
no.style.top=y+"px";
}

no.addEventListener("mouseover",moveButton);
no.addEventListener("touchstart",function(e){
e.preventDefault();
moveButton();
});

document.getElementById("yes").onclick=function(){
document.body.innerHTML="<h1 style='color:white;text-align:center;margin-top:40vh;font-size:45px;'>Yay! ❤️🎉</h1>";
}
</script>

</body>
</html>
