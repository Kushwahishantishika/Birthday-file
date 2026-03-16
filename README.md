<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Happy Birthday!</title>

<style>
body{
    margin:0;
    font-family: Arial, sans-serif;
    text-align:center;
    background: linear-gradient(135deg,#ff9a9e,#fad0c4);
    color:white;
    display:flex;
    justify-content:center;
    align-items:center;
    height:100vh;
}

.container{
    padding:20px;
}

h1{
    font-size:8vw;
    margin-bottom:10px;
}

p{
    font-size:4.5vw;
}

button{
    margin-top:20px;
    padding:12px 25px;
    font-size:4vw;
    border:none;
    border-radius:25px;
    background:#ff4b5c;
    color:white;
    cursor:pointer;
}

button:hover{
    background:#ff1f3d;
}

/* Mobile adjustments */
@media(min-width:600px){
    h1{font-size:50px;}
    p{font-size:22px;}
    button{font-size:18px;}
}
</style>
</head>

<body>

<div class="container">
    <h1>🎂 Happy Birthday! 🎉</h1>
    <p>Wishing you a day filled with happiness and a year filled with joy!</p>
    <button onclick="startConfetti()">Celebrate 🎊</button>
</div>

<!-- Confetti Library -->
<script src="https://cdn.jsdelivr.net/npm/canvas-confetti@1.6.0/dist/confetti.browser.min.js"></script>

<script>
function startConfetti(){
    confetti({
        particleCount:150,
        spread:90,
        origin:{y:0.6}
    });

    setTimeout(()=>{
        confetti({
            particleCount:200,
            spread:120,
            origin:{y:0.6}
        });
    },500);
}
</script>

</body>
</html>
