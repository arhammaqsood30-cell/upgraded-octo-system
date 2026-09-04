index.html<!DOCTYPE html><html lang="ur" dir="rtl">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>دل جان 1400</title><style>
*{
    box-sizing:border-box;
    margin:0;
    padding:0;
}

body{
    font-family:Arial,"Noto Nastaliq Urdu",sans-serif;
    background:#f4f7f6;
    color:#17352d;
    line-height:1.8;
}

header{
    background:linear-gradient(135deg,#174c3e,#28745e);
    color:white;
    text-align:center;
    padding:25px 15px;
}

.logo{
    width:75px;
    height:75px;
    margin:auto;
    border-radius:50%;
    background:#d4af37;
    color:#173f35;
    display:flex;
    align-items:center;
    justify-content:center;
    font-size:27px;
    font-weight:bold;
}

header h1{
    margin-top:10px;
    font-size:28px;
}

header p{
    font-size:15px;
}

nav{
    background:white;
    display:flex;
    justify-content:center;
    flex-wrap:wrap;
    gap:8px;
    padding:12px;
    box-shadow:0 2px 8px #ddd;
}

nav button{
    border:0;
    padding:9px 16px;
    border-radius:25px;
    background:#edf5f2;
    color:#174c3e;
    cursor:pointer;
    font-size:14px;
}

nav button:hover,
nav button.active{
    background:#246b58;
    color:white;
}

.container{
    width:94%;
    max-width:1100px;
    margin:25px auto;
}

.section{
    display:none;
}

.section.active{
    display:block;
}

.hero{
    background:white;
    padding:25px;
    border-radius:20px;
    text-align:center;
    margin-bottom:20px;
    box-shadow:0 4px 15px #ddd;
}

.hero h2{
    color:#246b58;
    margin-bottom:10px;
}

.grid{
    display:grid;
    grid-template-columns:repeat(auto-fit,minmax(220px,1fr));
    gap:16px;
}

.card{
    background:white;
    padding:22px;
    border-radius:18px;
    text-align:center;
    box-shadow:0 4px 15px #ddd;
}

.icon{
    font-size:38px;
}

.card h3{
    color:#246b58;
    margin:8px 0;
}

.card p{
    color:#555;
    font-size:14px;
}

.btn{
    margin-top:12px;
    padding:9px 18px;
    border:0;
    border-radius:20px;
    background:#246b58;
    color:white;
    cursor:pointer;
    font-family:inherit;
}

.btn:hover{
    background:#173f35;
}

.search{
    width:100%;
    padding:14px;
    border:1px solid #ccdcd6;
    border-radius:15px;
    margin-bottom:18px;
    font-size:15px;
}

.contact{
    background:#eef7f3;
    padding:20px;
    border-radius:15px;
    text-align:center;
}

.number{
    direction:ltr;
    display:inline-block;
    font-family:Arial,sans-serif;
    font-size:20px;
    margin:8px;
}

footer{
    margin-top:35px;
    padding:22px;
    text-align:center;
    background:#173f35;
    color:white;
}

@media(max-width:600px){
    header h1{
        font-size:23px;
    }

    nav button{
        font-size:13px;
        padding:7px 12px;
    }
}
</style></head><body><header>
    <div class="logo">DJ</div>
    <h1>دل جان 1400</h1>
    <p>صحت • تعلیم • روزگار • عوامی رہنمائی</p>
</header><nav>
    <button class="active" onclick="showSection('home',this)">🏠 ہوم</button>
    <button onclick="showSection('health',this)">❤️ صحت</button>
    <button onclick="showSection('education',this)">📚 تعلیم</button>
    <button onclick="showSection('jobs',this)">💼 روزگار</button>
    <button onclick="showSection('info',this)">ℹ️ معلومات</button>
    <button onclick="showSection('contact',this)">📞 رابطہ</button>
</nav><div class="container"><section id="home" class="section active"><div class="hero">
    <h2>خوش آمدید — دل جان 1400</h2>

    <p>
        یہ پلیٹ فارم عام عوام کے لیے صحت، تعلیم،
        روزگار اور مفید معلومات ایک جگہ فراہم کرنے
        کے مقصد سے بنایا گیا ہے۔
    </p>
</div>

<div class="grid">

    <div class="card">
        <div class="icon">❤️</div>
        <h3>صحت</h3>
        <p>صحت سے متعلق مفید اور عام فہم معلومات۔</p>
        <button class="btn" onclick="showSection('health')">
            مزید دیکھیں
        </button>
    </div>

    <div class="card">
        <div class="icon">📚</div>
        <h3>تعلیم</h3>
        <p>تعلیم اور سیکھنے کے مفید مواقع۔</p>
        <button class="btn" onclick="showSection('education')">
            مزید دیکھیں
        </button>
    </div>

    <div class="card">
        <div class="icon">💼</div>
        <h3>روزگار</h3>
        <p>روزگار اور ہنر سے متعلق رہنمائی۔</p>
        <button class="btn" onclick="showSection('jobs')">
            مزید دیکھیں
        </button>
    </div>

    <div class="card">
        <div class="icon">ℹ️</div>
        <h3>معلومات</h3>
        <p>عوام کے فائدے کے لیے اہم معلومات۔</p>
        <button class="btn" onclick="showSection('info')">
            مزید دیکھیں
        </button>
    </div>

</div>

</section><section id="health" class="section"><div class="hero">
    <h2>❤️ صحت</h2>
    <p>صحت سے متعلق مفید معلومات</p>
</div>

<input
    class="search"
    type="text"
    placeholder="صحت کی معلومات تلاش کریں..."
    onkeyup="searchCards(this)"
>

<div class="grid">

    <div class="card searchable">
        <div class="icon">🥗</div>
        <h3>غذائیت</h3>
        <p>متوازن غذا اور صحت مند زندگی کی بنیادی معلومات۔</p>
    </div>

    <div class="card searchable">
        <div class="icon">🏃</div>
        <h3>ورزش</h3>
        <p>روزانہ جسمانی سرگرمی کی اہمیت۔</p>
    </div>

    <div class="card searchable">
        <div class="icon">🩺</div>
        <h3>صحت کی احتیاط</h3>
        <p>صحت کے مسئلے میں بروقت ماہر سے مشورہ ضروری ہے۔</p>
    </div>

</div>

</section><section id="education" class="section"><div class="hero">
    <h2>📚 تعلیم</h2>
    <p>علم حاصل کریں، ہنر سیکھیں اور آگے بڑھیں۔</p>
</div>

<div class="grid">

    <div class="card">
        <div class="icon">🎓</div>
        <h3>تعلیمی مواقع</h3>
        <p>طلبہ کے لیے تعلیمی مواقع اور رہنمائی۔</p>
    </div>

    <div class="card">
        <div class="icon">💻</div>
        <h3>آن لائن تعلیم</h3>
        <p>گھر بیٹھ کر نئی مہارتیں سیکھنے کے ذرائع۔</p>
    </div>

    <div class="card">
        <div class="icon">📖</div>
        <h3>مطالعہ</h3>
        <p>مطالعہ اور علم کی اہمیت۔</p>
    </div>

</div>

</section><section id="jobs" class="section"><div class="hero">
    <h2>💼 روزگار</h2>
    <p>ہنر اور روزگار کے مواقع کے لیے رہنمائی۔</p>
</div>

<div class="grid">

    <div class="card">
        <div class="icon">💻</div>
        <h3>آن لائن کام</h3>
        <p>فری لانسنگ اور آن لائن کام کی بنیادی معلومات۔</p>
    </div>

    <div class="card">
        <div class="icon">🛠️</div>
        <h3>ہنر</h3>
        <p>مستقبل کے لیے مفید ہنر سیکھنے کی رہنمائی۔</p>
    </div>

    <div class="card">
        <div class="icon">📄</div>
        <h3>CV</h3>
        <p>اچھی CV بنانے اور ملازمت کی تیاری کی رہنمائی۔</p>
    </div>

</div>

</section><section id="info" class="section"><div class="hero">
    <h2>ℹ️ معلومات</h2>
    <p>
        مختلف شعبوں سے متعلق مفید معلومات
        یہاں منظم انداز میں شامل کی جائیں گی۔
    </p>
</div>

<div class="grid">

    <div class="card">
        <div class="icon">📢</div>
        <h3>اہم اعلانات</h3>
        <p>عوامی فائدے کے اہم اعلانات۔</p>
    </div>

    <div class="card">
        <div class="icon">🔗</div>
        <h3>اہم لنکس</h3>
        <p>ضروری ویب سائٹس اور آن لائن وسائل۔</p>
    </div>

    <div class="card">
        <div class="icon">📑</div>
        <h3>دستاویزات</h3>
        <p>ضروری دستاویزات کے لیے الگ جگہ۔</p>
    </div>

</div>

</section><section id="contact" class="section"><div class="hero">

    <h2>📞 رابطہ</h2>

    <p>
        معلومات یا ویب سائٹ سے متعلق رہنمائی کے لیے رابطہ کریں۔
    </p>

    <div class="contact">

        <h3>WhatsApp</h3>

        <div class="number">
            03430450007
        </div>

        <br>

        <a
            class="btn"
            href="https://wa.me/923430450007"
            target="_blank"
        >
            WhatsApp پر رابطہ کریں
        </a>

    </div>

</div>

</section></div><footer>
    <strong>دل جان 1400</strong>
    <br>
    صحت، تعلیم اور روزگار کے لیے عوامی پلیٹ فارم
    <br>
    © 2026 Dil Jaan 1400
</footer><script>

function showSection(id, button){

    document.querySelectorAll('.section').forEach(function(section){
        section.classList.remove('active');
    });

    document.getElementById(id).classList.add('active');

    document.querySelectorAll('nav button').forEach(function(btn){
        btn.classList.remove('active');
    });

    if(button){
        button.classList.add('active');
    }

    window.scrollTo(0,0);
}


function searchCards(input){

    let text = input.value.toLowerCase();

    document.querySelectorAll('#health .searchable').forEach(function(card){

        let content = card.innerText.toLowerCase();

        if(content.includes(text)){
            card.style.display = '';
        }else{
            card.style.display = 'none';
        }

    });
}

</script></body>
</html>
