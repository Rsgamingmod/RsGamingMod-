<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>RS GAMING MOD</title>

<style>
*{
    margin:0;
    padding:0;
    box-sizing:border-box;
    font-family:Arial,Helvetica,sans-serif;
    scroll-behavior:smooth;
}

body{
    background:#030303;
    color:#fff;
    overflow-x:hidden;
}

/* BACKGROUND */
body::before{
    content:"";
    position:fixed;
    inset:0;
    z-index:-2;

    background:
    radial-gradient(circle at 15% 20%,rgba(0,255,255,.12),transparent 28%),
    radial-gradient(circle at 85% 30%,rgba(255,0,150,.12),transparent 30%),
    radial-gradient(circle at 50% 90%,rgba(0,255,80,.10),transparent 30%);
}

/* HEADER */
header{
    position:sticky;
    top:0;
    z-index:1000;

    display:flex;
    justify-content:space-between;
    align-items:center;

    padding:17px 6%;

    background:rgba(0,0,0,.88);
    backdrop-filter:blur(12px);

    border-bottom:1px solid rgba(0,255,255,.35);
}

.logo{
    font-size:25px;
    font-weight:1000;

    color:#00ffff;

    text-shadow:
    0 0 8px #00ffff,
    0 0 20px #00ffff;
}

nav{
    display:flex;
    gap:22px;
}

nav a{
    color:#fff;
    text-decoration:none;
    font-weight:bold;
    transition:.3s;
}

nav a:hover{
    color:#00ffff;
    text-shadow:0 0 12px #00ffff;
}

/* HERO */
.hero{
    min-height:88vh;

    display:flex;
    justify-content:center;
    align-items:center;

    text-align:center;

    padding:50px 20px;
}

.hero-content{
    max-width:950px;
}

.welcome{
    color:#00ff88;
    font-size:22px;
    font-weight:bold;
    letter-spacing:6px;

    margin-bottom:15px;

    animation:pulse 2s infinite;
}

.hero h1{
    font-size:clamp(48px,10vw,90px);
    font-weight:1000;

    background:
    linear-gradient(
        90deg,
        #00ffff,
        #ff00ff,
        #ffff00,
        #00ff66,
        #ff0055,
        #00ffff
    );

    background-size:500%;

    -webkit-background-clip:text;
    color:transparent;

    animation:gradientMove 7s infinite;
}

.hero h2{
    margin-top:20px;

    color:#ffcc00;

    font-size:clamp(23px,5vw,40px);

    text-shadow:0 0 12px #ffcc00;
}

.hero p{
    margin-top:12px;

    color:#00ff99;

    font-size:20px;
    font-weight:bold;
}

/* HERO BUTTONS */
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

    color:#fff;
    text-decoration:none;

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

    box-shadow:
    0 0 20px #00ffff,
    0 0 40px #00ffff;
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

    text-shadow:
    0 0 10px #ff00ff,
    0 0 25px #ff00ff;
}

.section-title p{
    margin-top:10px;
    color:#00ffff;
}

/* CATEGORY GRID */
.category-grid{
    max-width:1150px;
    margin:auto;

    display:grid;

    grid-template-columns:
    repeat(auto-fit,minmax(280px,1fr));

    gap:25px;
}

/* CARD */
.card{
    position:relative;

    padding:28px;

    border-radius:22px;

    background:
    linear-gradient(
        145deg,
        rgba(255,255,255,.09),
        rgba(255,255,255,.02)
    );

    border:1px solid rgba(255,255,255,.2);

    overflow:hidden;

    transition:.4s;
}

.card::before{
    content:"";

    position:absolute;

    width:150px;
    height:150px;

    top:-60px;
    right:-60px;

    background:#00ffff;

    filter:blur(70px);

    opacity:.18;
}

.card:hover{
    transform:translateY(-10px);

    border-color:#00ffff;

    box-shadow:
    0 0 20px rgba(0,255,255,.35),
    0 0 50px rgba(255,0,255,.15);
}

/* NUMBER */
.number{
    color:#ffcc00;

    font-size:18px;

    font-weight:900;

    letter-spacing:2px;
}

/* CARD TITLE */
.card h3{
    margin:12px 0;

    color:#00ffff;

    font-size:23px;

    line-height:1.3;

    text-shadow:0 0 8px rgba(0,255,255,.5);
}

.sub{
    color:#ff66cc;

    margin-bottom:20px;

    font-weight:bold;
}

/* VERSION */
.version{
    display:flex;

    justify-content:space-between;
    align-items:center;

    gap:10px;

    padding:14px;

    margin:10px 0;

    background:rgba(0,0,0,.5);

    border-radius:13px;

    border:1px solid rgba(255,255,255,.08);
}

.version-name{
    color:#ffff00;

    font-weight:900;
}

/* DOWNLOAD BUTTON */
.download{
    display:inline-block;

    padding:9px 16px;

    border-radius:20px;

    background:#00ff66;

    color:#000;

    text-decoration:none;

    font-weight:1000;

    transition:.3s;

    box-shadow:0 0 10px rgba(0,255,102,.35);
}

.download:hover{
    background:#00ffff;

    transform:scale(1.08);

    box-shadow:
    0 0 15px #00ffff,
    0 0 30px #00ffff;
}

/* SOON */
.soon{
    color:#ff9900;

    font-weight:1000;

    text-shadow:0 0 8px rgba(255,153,0,.5);
}

/* LIVERY */
.livery-list{
    margin-top:15px;
}

.livery{
    display:flex;

    justify-content:space-between;
    align-items:center;

    gap:10px;

    padding:14px;

    margin:10px 0;

    border-radius:13px;

    background:rgba(0,0,0,.45);

    border:1px solid rgba(255,255,255,.08);
}

.livery strong{
    color:#ff66ff;

    font-size:14px;
}

/* RAIN DOWNLOAD */
.rain-download{
    display:block;

    padding:18px;
}

.rain-download .version-name{
    font-size:19px;
}

.rain-download .download{
    margin-top:12px;
}

.click-download{
    margin-top:10px;

    color:#00ffff;

    font-size:12px;

    font-weight:bold;

    letter-spacing:1px;

    animation:pulse 1.8s infinite;
}

/* WARNING */
.warning{
    max-width:900px;

    margin:20px auto;

    padding:35px;

    text-align:center;

    border:2px solid #ff2222;

    border-radius:22px;

    background:rgba(255,0,0,.07);

    box-shadow:
    0 0 25px rgba(255,0,0,.25);
}

.warning h2{
    color:#ff2222;

    font-size:32px;

    margin-bottom:18px;

    text-shadow:
    0 0 10px red,
    0 0 25px red;
}

.warning p{
    color:#ff7777;

    font-size:18px;

    font-weight:900;

    line-height:1.6;
}

/* COPYRIGHT */
.copyright{
    max-width:900px;

    margin:30px auto;

    padding:35px;

    text-align:center;

    border:1px solid #00ffff;

    border-radius:22px;

    background:rgba(0,255,255,.04);

    box-shadow:0 0 20px rgba(0,255,255,.08);
}

.copyright h2{
    color:#00ffff;

    margin-bottom:18px;

    text-shadow:0 0 10px #00ffff;
}

.copyright p{
    color:#ccc;

    line-height:1.8;

    font-size:15px;
}

/* FOOTER */
footer{
    text-align:center;

    padding:35px 15px;

    border-top:1px solid rgba(255,255,255,.15);

    background:#020202;
}

footer p{
    color:#777;

    font-size:14px;

    line-height:1.8;
}

/* ANIMATIONS */
@keyframes gradientMove{

    0%{
        background-position:0%;
    }

    50%{
        background-position:100%;
    }

    100%{
        background-position:0%;
    }
}

@keyframes pulse{

    0%,100%{
        opacity:1;
    }

    50%{
        opacity:.55;
    }
}

/* MOBILE */
@media(max-width:650px){

    header{
        flex-direction:column;

        gap:13px;

        padding:15px;
    }

    nav{
        gap:12px;
    }

    nav a{
        font-size:12px;
    }

    .hero{
        min-height:80vh;
    }

    .hero h1{
        font-size:48px;
    }

    .hero h2{
        font-size:24px;
    }

    .hero p{
        font-size:17px;
    }

    section{
        padding:60px 17px;
    }

    .section-title h2{
        font-size:31px;
    }

    .card{
        padding:22px;
    }

    .livery,
    .version{
        gap:8px;
    }

    .download{
        padding:8px 13px;

        font-size:12px;
    }

    .warning{
        padding:28px 18px;
    }

    .warning h2{
        font-size:27px;
    }

}
</style>
</head>


<body>


<!-- HEADER -->
<header>

    <div class="logo">
        RS GAMING MOD
    </div>

    <nav>

        <a href="#home">
            HOME
        </a>

        <a href="#bussid">
            BUSSID
        </a>

        <a href="#copyright">
            COPYRIGHT
        </a>

    </nav>

</header>


<!-- HOME PAGE -->
<section class="hero" id="home">

    <div class="hero-content">

        <div class="welcome">
            WELCOME TO
        </div>

        <h1>
            RS GAMING MOD
        </h1>

        <h2>
            BUSSID / BUSSIN MOD STORE
        </h2>

        <p>
            DOWNLOAD FREE &amp; EASY
        </p>


        <div class="hero-buttons">

            <a href="#bussid" class="btn">
                🚌 BUSSID MODS
            </a>

            <a href="#bussid" class="btn">
                🚍 BUSSIN MODS
            </a>

            <a href="#bussid" class="btn">
                📥 FREE DOWNLOADS
            </a>

        </div>

    </div>

</section>


<!-- BUSSID CATEGORY -->
<section id="bussid">

    <div class="section-title">

        <h2>
            BUSSID CATEGORY
        </h2>

        <p>
            BUSSID &amp; BUSSIN MODS
        </p>

    </div>


    <div class="category-grid">


        <!-- 01 LIVERYS -->
        <div class="card">

            <div class="number">
                01
            </div>

            <h3>
                BUSSID/N LIVERYS
            </h3>

            <div class="sub">
                KSRTC • KKRTC • NWKRTC
            </div>


            <div class="livery-list">

                <div class="livery">

                    <strong>
                        KSRTC LIVERY
                    </strong>

                    <a href="#" class="download">
                        DOWNLOAD
                    </a>

                </div>


                <div class="livery">

                    <strong>
                        KKRTC LIVERY
                    </strong>

                    <a href="#" class="download">
                        DOWNLOAD
                    </a>

                </div>


                <div class="livery">

                    <strong>
                        NWKRTC LIVERY
                    </strong>

                    <a href="#" class="download">
                        DOWNLOAD
                    </a>

                </div>

            </div>

        </div>


        <!-- 02 BUSSID STEERING -->
        <div class="card">

            <div class="number">
                02
            </div>

            <h3>
                BUSSID STEERING WHEEL MOD
            </h3>


            <div class="version">

                <span class="version-name">
                    V4.5.2
                </span>

                <a href="#" class="download">
                    DOWNLOAD
                </a>

            </div>


            <div class="version">

                <span class="version-name">
                    V4.5.3
                </span>

                <span class="soon">
                    SOON
                </span>

            </div>

        </div>


        <!-- 03 BUSSIN STEERING -->
        <div class="card">

            <div class="number">
                03
            </div>

            <h3>
                BUSSIN STEERING WHEEL MOD
            </h3>


            <div class="version">

                <span class="version-name">
                    V1.0.1
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


        <!-- 04 HORN SOUND -->
        <div class="card">

            <div class="number">
                04
            </div>

            <h3>
                BUSSID HORN SOUND MOD
            </h3>


            <div class="version">

                <span class="version-name">
                    V4.5.2
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


        <!-- 05 REALISTIC RAIN -->
        <div class="card">

            <div class="number">
                05
            </div>

            <h3>
                BUSSID REALISTIC RAIN 🌧️ MOD
            </h3>

            <div class="sub">
                REALISTIC WEATHER MOD
            </div>


            <!-- V4.5.2 -->
            <div class="version rain-download">

                <span class="version-name">
                    V4.5.2
                </span>

                <a
                    href="https://sharemods.com/qulwt9z7rnom/BUSSID_V4.5.2_RAIN__COLOUR_LIGHT__x27_S_MOD.7z.html"
                    target="_blank"
                    rel="noopener noreferrer"
                    class="download"
                >
                    DOWNLOAD
                </a>

                <div class="click-download">
                    CLICK HERE TO DOWNLOAD
                </div>

            </div>


            <!-- V4.5.3 -->
            <div class="version">

                <span class="version-name">
                    V4.5.3
                </span>

                <span class="soon">
                    SOON
                </span>

            </div>


            <!-- V4.5.4 -->
            <div class="version">

                <span class="version-name">
                    V4.5.4
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

        <h2>
            ⚠️ WARNING
        </h2>

        <p>
            DON'T RE-EDIT OR RE-UPLOAD THIS FILE
        </p>

    </div>


    <!-- COPYRIGHT -->
    <div class="copyright" id="copyright">

        <h2>
            © COPYRIGHT POLICY
        </h2>

        <p>
            All files, mods and liveries available on
            this website are protected by copyright.
            <br><br>

            Don't re-edit, re-upload or redistribute
            any file without permission.
        </p>

    </div>

</section>


<!-- FOOTER -->
<footer>

    <p>
        BUSSID / BUSSIN MOD STORE
    </p>

    <p>
        © 2026 All Rights Reserved.
    </p>

</footer>


</body>
</html>
