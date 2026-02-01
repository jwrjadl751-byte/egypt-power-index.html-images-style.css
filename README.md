# egypt-power-index.html-images-style.css
egypt-power/   index.html   images/   style.css
<!DOCTYPE html>
<html lang="ar">
<head>
<meta charset="UTF-8">
<title>مصر أقوى | Egypt Power</title>
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<style>
* { box-sizing: border-box; }

body {
    margin: 0;
    font-family: Tahoma, Arial;
    direction: rtl;
    text-align: center;
    background: linear-gradient(135deg, #000, #b71c1c);
    color: white;
    transition: 0.5s;
}

header {
    padding: 30px;
    animation: fadeIn 2s;
}

h1 {
    font-size: 40px;
}

nav {
    background: rgba(0,0,0,0.7);
    padding: 10px;
    position: sticky;
    top: 0;
}

nav a {
    color: white;
    margin: 10px;
    text-decoration: none;
    font-weight: bold;
}

nav a:hover {
    color: gold;
}

.container {
    padding: 20px;
}

.card {
    background: rgba(255,255,255,0.1);
    padding: 20px;
    margin: 20px auto;
    max-width: 700px;
    border-radius: 15px;
    box-shadow: 0 0 20px black;
    animation: fadeInUp 1.5s;
}

img {
    width: 100%;
    border-radius: 15px;
    margin-top: 10px;
    transition: 0.5s;
}

img:hover {
    transform: scale(1.05);
}

button {
    background: gold;
    color: black;
    border: none;
    padding: 12px 20px;
    margin: 10px;
    border-radius: 10px;
    font-size: 16px;
    cursor: pointer;
}

button:hover {
    background: orange;
}

footer {
    margin-top: 30px;
    padding: 15px;
    background: rgba(0,0,0,0.8);
}

@keyframes fadeIn {
    from {opacity: 0;}
    to {opacity: 1;}
}

@keyframes fadeInUp {
    from {opacity: 0; transform: translateY(50px);}
    to {opacity: 1; transform: translateY(0);}
}
</style>
</head>
<body>

<header>
    <h1>🇪🇬 مصر أقوى</h1>
    <p>أقوى موقع وطني في الكون</p>
</header>

<nav>
    <a href="#">الرئيسية</a>
    <a href="#">حضارة</a>
    <a href="#">صور</a>
    <a href="#">تفاعل</a>
</nav>

<div class="container">

<div class="card">
    <h2>عن مصر</h2>
    <p>
        مصر أم الدنيا، تاريخ، حضارة، جيش قوي، شعب عظيم.
    </p>
</div>

<div class="card">
    <h2>صور أسطورية</h2>
    <img src="https://upload.wikimedia.org/wikipedia/commons/e/e3/Kheops-Pyramid.jpg">
    <img src="https://upload.wikimedia.org/wikipedia/commons/9/9f/Nile_River_and_Cairo_skyline.jpg">
</div>

<div class="card">
    <h2>زرار تفاعلي 🔥</h2>
    <p id="msg">اضغط وشوف السحر</p>
    <button onclick="power()">قوة مصر</button>
    <button onclick="changeBg()">غيّر الجو</button>
</div>

<div class="card">
    <h2>عدد الزوار</h2>
    <p id="visits">0</p>
</div>

<div class="card">
    <h2>نشيد وطني 🎵</h2>
    <button onclick="playSound()">شغّل الصوت</button>
    <audio id="sound">
        <source src="https://www.soundhelix.com/examples/mp3/SoundHelix-Song-1.mp3">
    </audio>
</div>

</div>

<footer>
    <p>© 2026 | Egypt Power</p>
</footer>

<script>
// زر القوة
function power() {
    document.getElementById("msg").innerHTML = "تحيا مصر 🇪🇬🔥 أقوى دولة!";
    alert("مصر فوق الجميع!");
}

// تغيير الخلفية
function changeBg() {
    document.body.style.background =
        "linear-gradient(135deg, #1a237e, #0d47a1)";
}

// عداد زوار وهمي
let count = 0;
setInterval(() => {
    count += Math.floor(Math.random() * 5);
    document.getElementById("visits").innerHTML = count + " زائر";
}, 1000);

// صوت
function playSound() {
    document.getElementById("sound").play();
}
</script>

</body>
</html>
