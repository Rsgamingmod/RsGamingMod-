<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>RS GAMING MOD | BUSSID & BUSSIN Mods</title>

<style>
*{
    margin:0;
    padding:0;
    box-sizing:border-box;
    font-family:Arial,Helvetica,sans-serif;
    scroll-behavior:smooth;
}

body{
    background:#050505;
    color:white;
    overflow-x:hidden;
}

/* BACKGROUND */
body::before{
    content:"";
    position:fixed;
    width:100%;
    height:100%;
    background:
        radial-gradient(circle at 20% 20%,rgba(0,255,255,.12),transparent 30%),
        radial-gradient(circle at 80% 40%,rgba(255,0,120,.12),transparent 30%),
        radial-gradient(circle at 50% 90%,rgba(0,255,80,.10),transparent 30%);
    z-index:-2;
}

/* HEADER */
header{
    position:sticky;
    top:0;
    z-index:1000;
    background:rgba(0,0,0,.88);
    backdrop-filter:blur(12px);
    border-bottom:1px solid rgba(0,255,255,.3);
    padding:16px 5%;
    display:flex;
    justify-content:space-between;
    align-items:center;
}

.logo{
    font-size:25px;
    font-weight:900;
    color:#00ffff;
    text-shadow:0 0 15px #00ffff;
}

nav a{
    color:white;
    text-decoration:none;
    margin-left:22px;
    font-weight:bold;
    transition:.3s;
}

nav a:hover{
    color:#00ffff;
    text-shadow:0 0 10px #00ffff;
}

/* HERO */
.hero{
    min-height:90vh;
    display:flex;
    justify-content:center;
    align-items:center;
    text-align:center;
    padding:50px 20px;
}

.hero-content{
    max-width:900px;
}

.welcome{
    font-size:22px;
    color:#00ff88;
    letter-spacing:5px;
    margin-bottom:15px;
    animation:pulse 2s infinite;
}

.hero h1{
    font-size:clamp(45px,10vw,90px);
    font-weight:1000;
    background:linear-gradient(
        90deg,
        #00ffff,
        #ff00ff,
        #ffff00,
        #00ff66,
        #ff0055
    );
    background-size:400%;
    -webkit-background-clip:text;
    color:transparent;
    animation:gradient 6s infinite;
}

.hero h2{
    margin-top:20px;
    color:#ffcc00;
    font-size:clamp(22px,5vw,40px);
}

.hero p{
    margin-top:12px;
    color:#00ff99;
    font-size:20px;
}

.hero-buttons{
    margin-top:35px;
    display:flex;
    justify-content:center;
    flex-wrap:wrap;
    gap:15px;
}

.btn{
    display:inline-block;
    padding:14px 25px;
    border-radius:30px;
    text-decoration:none;
    color:white;
    font-weight:bold;
    border:2px solid #00ffff;
    background:rgba(0,255,255,.08);
    box-shadow:0 0 15px rgba(0,255,255,.4);
    transition:.3s;
}

.btn:hover{
    transform:translateY(-5px) scale(1.05);
    background:#00ffff;
    color:#000;
    box-shadow:0 0 30px #00ffff;
}

/* SECTION */
section{
    padding:80px 6%;
}

.section-title{
    text-align:center;
    margin-bottom:45px;
}

.section-title h2{
    font-size:42px;
    color:#ff00ff;
    text-shadow:0 0 15px #ff00ff;
}

.section-title p{
    margin-top:10px;
    color:#00ffff;
}

/* CATEGORY GRID */
.category-grid{
    max-width:1100px;
    margin:auto;
    display:grid;
    grid-template-columns:repeat(auto-fit,minmax(280px,1fr));
    gap:25px;
}

/* CARD */
.card{
    position:relative;
    background:linear-gradient(
        145deg,
        rgba(255,255,255,.08),
        rgba(255,255,255,.02)
    );
    border:1px solid rgba(255,255,255,.2);
    border-radius:20px;
    padding:28px;
    overflow:hidden;
    transition:.4s;
}

.card::before{
    content:"";
    position:absolute;
    width:120px;
    height:120px;
    background:#00ffff;
    filter:blur(70px);
    opacity:.18;
    top:-50px;
    right:-50px;
}

.card:hover{
    transform:translateY(-10px);
    border-color:#00ffff;
    box-shadow:
        0 0 20px rgba(0,255,255,.3),
        0 0 50px rgba(255,0,255,.15);
}

.number{
    color:#ffcc00;
    font-size:18px;
    font-weight:bold;
}

.card h3{
    margin:12px 0;
    color:#00ffff;
    font-size:24px;
}

.card .sub{
    color:#ff66cc;
    margin-bottom:20px;
}

.version{
    display:flex;
    justify-content:space-between;
    align-items:center;
    padding:14px;
    margin:10px 0;
    background:rgba(0,0,0,.5);
    border-radius:12px;
}

.version-name{
    color:#ffff00;
    font-weight:bold;
}

.download{
    padding:9px 16px;
    border-radius:20px;
    background:#00ff66;
    color:#000;
    text-decoration:none;
    font-weight:900;
    transition:.3s;
}

.download:hover{
    background:#00ffff;
    box-shadow:0 0 20px #00ffff;
    transform:scale(1.08);
}

.soon{
    color:#ff9900;
    font-weight:bold;
}

/* LIVERY CARD */
.livery-list{
    margin-top:15px;
}

.livery{
    margin:10px 0;
    padding:14px;
    border-radius:12px;
    background:rgba(0,0,0,.45);
    display:flex;
    justify-content:space-between;
    align-items:center;
}

.livery strong{
    color:#ff66ff;
}

/* WARNING */
.warning{
    max-width:900px;
    margin:30px auto;
    padding:35px;
    text-align:center;
    border:2px solid #ff2222;
    border-radius:20px;
    background:rgba(255,0,0,.07);
    box-shadow:0 0 25px rgba(255,0,0,.25);
}

.warning h2{
    color:#ff2222;
    font-size:32px;
    text-shadow:0 0 15px red;
    margin-bottom:18px;
}

.warning p{
    color:#ff7777;
    font-size:18px;
    font-weight:bold;
}

/* COPYRIGHT */
.copyright{
    max-width:900px;
    margin:30px auto;
    padding:35px;
    text-align:center;
    border:1px solid #00ffff;
    border-radius:20px;
    background:rgba(0,255,255,.04);
}

.copyright h2{
    color:#00ffff;
    margin-bottom:15px;
}

.copyright p{
    color:#cccccc;
    line-height:1.7;
}

/* FOOTER */
footer{
    text-align:center;
    padding:30px 15px;
    border-top:1px solid rgba(255,255,255,.15);
    background:#020202;
}

footer .brand{
    color:#ff00ff;
    font-size:22px;
    font-weight:bold;
}

footer p{
    margin-top:10px;
    color:#888;
}

/* ANIMATION */
@keyframes gradient{
    0%{background-position:0%}
    50%{background-position:100%}
    100%{background-position:0%}
}

@keyframes pulse{
    0%,100%{opacity:1}
    50%{opacity:.55}
}

/* MOBILE */
@media(max-width:650px){

    header{
        flex-direction:column;
        gap:12px;
    }

    nav a{
        margin:0 7px;
        font-size:13px;
    }

    .hero{
        min-height:80vh;
    }

    .hero h1{
        font-size:48px;
    }

    .hero h2{
        font-size:25px;
    }

    section{
        padding:60px 18px;
    }

    .section-title h2{
        font-size:32px;
    }

    .card{
        padding:22px;
    }

    .livery,
    .version{
        gap:10px;
    }
}
</style>
</head>

<body>

<!-- HEADER -->
<header>

    <div class="logo">RS GAMING MOD</div>

    <nav>
        <a href="#home">HOME</a>
        <a href="#bussid">BUSSID</a>
        <a href="#copyright">COPYRIGHT</a>
    </nav>

</header>


<!-- HOME -->
<section class="hero" id="home">

    <div class="hero-content">

        <div class="welcome">
            WELCOME TO
        </div>

        <h1>RS GAMING MOD</h1>

        <h2>BUSSID / BUSSIN MOD STORE</h2>

        <p>DOWNLOAD FREE &amp; EASY</p>

        <div class="hero-buttons">
            <a href="#bussid" class="btn">🚌 BUSSID MODS</a>
            <a href="#bussid" class="btn">🚍 BUSSIN MODS</a>
            <a href="#bussid" class="btn">📥 FREE DOWNLOADS</a>
        </div>

    </div>

</section>


<!-- BUSSID CATEGORY -->
<section id="bussid">

    <div class="section-title">
        <h2>BUSSID CATEGORY</h2>
        <p>BUSSID &amp; BUSSIN MODS</p>
    </div>


    <div class="category-grid">


        <!-- 1 LIVERY -->
        <div class="card">

            <div class="number">01</div>

            <h3>BUSSID/N LIVERYS</h3>

            <div class="sub">
                KSRTC • KKRTC • NWKRTC
            </div>

            <div class="livery-list">

                <div class="livery">
                    <strong>KSRTC LIVERY</strong>
                    <a href="#" class="download">DOWNLOAD</a>
                </div>

                <div class="livery">
                    <strong>KKRTC LIVERY</strong>
                    <a href="#" class="download">DOWNLOAD</a>
                </div>

                <div class="livery">
                    <strong>NWKRTC LIVERY</strong>
                    <a href="#" class="download">DOWNLOAD</a>
                </div>

            </div>

        </div>


        <!-- 2 BUSSID STEERING -->
        <div class="card">

            <div class="number">02</div>

            <h3>BUSSID STEERING WHEEL MOD</h3>

            <div class="version">

                <span class="version-name">
                    v4.5.2
                </span>

                <a href="#" class="download">
                    DOWNLOAD
                </a>

            </div>

            <div class="version">

                <span class="version-name">
                    v4.5.3
                </span>

                <span class="soon">
                    SOON
                </span>

            </div>

        </div>


        <!-- 3 BUSSIN STEERING -->
        <div class="card">

            <div class="number">03</div>

            <h3>BUSSIN STEERING WHEEL MOD</h3>

            <div class="version">

                <span class="version-name">
                    v1.0.1
                </span>

                <a href="#" class="download">
                    DOWNLOAD
                </a>

            </div>

            <div class="version">

                <span class="version-name">
                    NEXT UPDATE
                </span>

                <span class="soon">
                    SOON
                </span>

            </div>

        </div>


        <!-- 4 HORN -->
        <div class="card">

            <div class="number">04</div>

            <h3>BUSSID HORN SOUND MOD</h3>

            <div class="version">

                <span class="version-name">
                    v4.5.2
                </span>

                <a href="#" class="download">
                    DOWNLOAD
                </a>

            </div>

            <div class="version">

                <span class="version-name">
                    NEXT UPDATE
                </span>

                <span class="soon">
                    SOON
                </span>

            </div>

        </div>


    </div>

</section>


<!-- WARNING -->
<section>

    <div class="warning">

        <h2>⚠️ WARNING</h2>

        <p>
            DON'T RE-EDIT OR RE-UPLOAD THIS FILE
        </p>

    </div>


    <!-- COPYRIGHT -->
    <div class="copyright" id="copyright">

        <h2>© COPYRIGHT POLICY</h2>

        <p>
            All files, mods and liveries available on
            <strong>RS GAMING MOD</strong>
            are protected by copyright.
            <br><br>
            Don't re-edit, re-upload or redistribute
            any file without permission.
        </p>

    </div>

</section>


<!-- FOOTER -->
<footer>

    <div class="brand">
        RS GAMING MOD
    </div>

    <p>
        BUSSID / BUSSIN MOD STORE
    </p>

    <p>
        © 2026 RS GAMING MOD. All Rights Reserved.
    </p>

</footer>


</body>
</html>
