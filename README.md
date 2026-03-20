<!DOCTYPE html>
<html lang="ar">
<head>
<meta charset="UTF-8">
<title>شهودتي ❤️</title>

<style>
body {
    margin: 0;
    font-family: Arial;
    text-align: center;
    color: white;
    overflow-x: hidden;
    background: url("https://images.unsplash.com/photo-1518895949257-7621c3c786d7") no-repeat center center/cover;
}

.overlay {
    background: rgba(0,0,0,0.7);
    min-height: 100vh;
    padding: 40px;
}

.page { display: none; }
.active { display: block; }

.card {
    background: rgba(255,255,255,0.1);
    padding: 30px;
    border-radius: 20px;
    backdrop-filter: blur(10px);
    display: inline-block;
    max-width: 600px;
}

h1 { font-size: 40px; }
p { font-size: 22px; line-height: 1.9; }

button {
    margin-top: 20px;
    padding: 10px 20px;
    border: none;
    border-radius: 10px;
    background: #ff4d6d;
    color: white;
    font-size: 18px;
    cursor: pointer;
}

.images img {
    width: 110px;
    height: 110px;
    border-radius: 50%;
    margin: 5px;
    object-fit: cover;
}

.heart {
    position: fixed;
    bottom: -10px;
    color: red;
    animation: floatUp 5s linear infinite;
}

@keyframes floatUp {
    0% { transform: translateY(0); opacity: 1; }
    100% { transform: translateY(-800px); opacity: 0; }
}
</style>

<script>
function showPage(pageId) {
    document.querySelectorAll('.page').forEach(p => p.classList.remove('active'));
    document.getElementById(pageId).classList.add('active');
}

function createHeart() {
    const heart = document.createElement("div");
    heart.classList.add("heart");
    heart.innerHTML = "❤️";
    heart.style.left = Math.random() * 100 + "vw";
    heart.style.fontSize = (Math.random() * 20 + 20) + "px";
    document.body.appendChild(heart);
    setTimeout(() => { heart.remove(); }, 5000);
}
setInterval(createHeart, 500);

function showLove() {
    document.getElementById("loveText").style.display = "block";
}
</script>

</head>

<body>

<!-- موسيقى YouTube تلقائي -->
<iframe id="ytMusic" 
    src="https://www.youtube.com/embed/fGFB29lQ-Vs?autoplay=1&loop=1&playlist=fGFB29lQ-Vs"
    allow="autoplay"
    style="display:none;">
</iframe>

<div class="overlay">

<!-- الصفحة 1 -->
<div id="page1" class="page active">
<div class="card">
<h1>عيدك مبارك يا شهودتي ❤️</h1>

<p>
كل عام وانتي أقرب إنسانة لقلبي😔<br>
وكل عام وضحكتك تفرحني وتكون سبب راحتي ❤️<br><br>

يا شهودي … انتي وجودك في حياتي نعمة كبيره بكل<br>
وان شاءلله ربي يخليك ليا وما يحرمنيش منك ي اغلى شي صارلي ف حياتي كلها 💫<br><br>

انتي مش بس حبيبتي…<br>
انتي فرحتي… وراحة بالي… وكل دنيتي 🥺❤️
</p>

<div class="images">
<!-- صور قلوب وورد كرابط مباشر -->
<img src="https://cdn.pixabay.com/photo/2017/08/06/09/36/heart-2590996_1280.png">
<img src="https://cdn.pixabay.com/photo/2016/04/01/11/03/heart-1301790_1280.png">
<img src="https://cdn.pixabay.com/photo/2016/03/31/19/21/heart-1293856_1280.png">
<img src="https://cdn.pixabay.com/photo/2017/01/31/21/21/heart-2025974_1280.png"> <!-- قلب إضافي -->
</div>

<button onclick="showPage('page2')">اضغطي هنا 💌</button>
</div>
</div>

<!-- الصفحة 2 -->
<div id="page2" class="page">
<div class="card">
<h1>لشهودتي ❤️</h1>

<p>
من أول ما عرفتك… حسّيت إن حياتي بدت تتغير للاحسن 💫<br><br>

نحبك على كل شي فيك…<br>
على ضحكتك … على طيبتك … على قلبك الحلو ❤️<br><br>

معاك نحس روحي متريح…<br>
ونبي نحكيلك كل شي بدون خوف 🤍<br><br>

انتي الشي اللي كان ناقصني<br>
وانتي أجمل حاجة صارتلي 🥺❤️
</p>

<button onclick="showPage('page3')">كملي 💕</button>
</div>
</div>

<!-- الصفحة 3 -->
<div id="page3" class="page">
<div class="card">
<h1>اعتراف ❤️</h1>

<p>
تبي الصراحة؟<br><br>

انا ما نقدرش نتخيل يومي بدونك…<br>
ولا نبي نعيش لحظة وانتي مش معايا 😔❤️<br><br>

نبيك تبقي جنبي ديما…<br>
في كل يوم… في كل ظرف… في كل شي 💕<br><br>

نحبك حب كبير يا شهودتي<br>
حب طالع من اعماق قلبي  ❤️<br><br>

ومهما نقول…<br>
عمري ما نوصل نص اللي نحسه اتجاهك 🥺❤️
</p>

<button onclick="showLove()">اضغطي هنا ❤️</button>

<p id="loveText" style="display:none; font-size:28px; margin-top:20px; color:#ffccd5;">
نحبك ي شهودتي ودنيتي وروحي وكلشي ليا  ❤️
</p>

<br>
<button onclick="showPage('page1')">ارجعي للبداية ❤️</button>

</div>
</div>

</div>

</body>
</html>
