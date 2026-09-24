<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>Happy Birthday Agasthiya 💜</title>

<style>
*{
    margin:0;
    padding:0;
    box-sizing:border-box;
}

html,body{
    width:100%;
    min-height:100%;
    font-family:Arial, Helvetica, sans-serif;
    background:#10051f;
    color:white;
    overflow-x:hidden;
}

body{
    overflow-y:auto;
}

/* ================= BACKGROUND ================= */

body::before{
    content:"";
    position:fixed;
    inset:0;
    background:
        radial-gradient(circle at 20% 20%,rgba(180,90,255,.18),transparent 30%),
        radial-gradient(circle at 80% 80%,rgba(255,100,220,.15),transparent 30%),
        linear-gradient(135deg,#10051f,#21083b,#12051f);
    z-index:-5;
}

.stars{
    position:fixed;
    inset:0;
    pointer-events:none;
    z-index:-2;
    background-image:
        radial-gradient(white 1px,transparent 1px),
        radial-gradient(#d9a7ff 1px,transparent 1px);
    background-size:70px 70px,110px 110px;
    background-position:0 0,30px 40px;
    opacity:.35;
}

/* ================= FLOATING HEARTS ================= */

.float{
    position:fixed;
    bottom:-50px;
    font-size:20px;
    opacity:.5;
    animation:floatUp linear infinite;
    pointer-events:none;
    z-index:5;
}

@keyframes floatUp{
    from{
        transform:translateY(0) rotate(0deg);
        opacity:0;
    }
    15%{opacity:.6;}
    85%{opacity:.5;}
    to{
        transform:translateY(-110vh) rotate(360deg);
        opacity:0;
    }
}

/* ================= SLIDES ================= */

.slide{
    min-height:100vh;
    width:100%;
    padding:70px 25px 110px;
    display:none;
    align-items:center;
    justify-content:center;
    text-align:center;
    overflow-y:auto;
}

.slide.active{
    display:flex;
    animation:slideIn .8s ease;
}

@keyframes slideIn{
    from{
        opacity:0;
        transform:scale(.96) translateY(20px);
    }
    to{
        opacity:1;
        transform:scale(1) translateY(0);
    }
}

.content{
    width:min(850px,100%);
    padding:35px 25px;
}

.small{
    color:#d8a7ff;
    letter-spacing:3px;
    font-size:13px;
    margin-bottom:18px;
}

h1{
    font-size:clamp(45px,9vw,90px);
    line-height:1;
    margin:15px 0;
    background:linear-gradient(90deg,#fff,#df9cff,#fff);
    -webkit-background-clip:text;
    color:transparent;
    text-shadow:0 0 35px rgba(208,125,255,.4);
}

h2{
    font-size:clamp(30px,6vw,55px);
    margin-bottom:25px;
}

p{
    font-size:clamp(17px,2.5vw,22px);
    line-height:1.8;
    color:#eee1fa;
}

.highlight{
    color:#e2a6ff;
    font-weight:bold;
}

.card{
    margin:25px auto;
    padding:28px;
    border:1px solid rgba(220,160,255,.35);
    border-radius:25px;
    background:rgba(255,255,255,.06);
    backdrop-filter:blur(12px);
    box-shadow:
        0 0 30px rgba(176,80,255,.12),
        inset 0 0 20px rgba(255,255,255,.03);
}

.emoji{
    font-size:65px;
    margin-bottom:20px;
}

.big-heart{
    font-size:90px;
    animation:pulse 1.5s infinite;
}

@keyframes pulse{
    0%,100%{transform:scale(1);}
    50%{transform:scale(1.15);}
}

/* ================= BUTTON ================= */

button{
    border:none;
    padding:16px 30px;
    border-radius:50px;
    background:linear-gradient(90deg,#9b45ff,#e07cff);
    color:white;
    font-size:16px;
    font-weight:bold;
    cursor:pointer;
    box-shadow:0 0 30px rgba(195,90,255,.45);
    transition:.3s;
    margin-top:25px;
}

button:hover{
    transform:scale(1.06);
    box-shadow:0 0 45px rgba(220,120,255,.7);
}

/* ================= TIMELINE ================= */

.timeline{
    display:grid;
    grid-template-columns:repeat(4,1fr);
    gap:15px;
    margin-top:30px;
}

.timebox{
    padding:25px 10px;
    border-radius:20px;
    background:rgba(255,255,255,.06);
    border:1px solid rgba(216,160,255,.3);
}

.timebox h3{
    color:#d99cff;
    margin-bottom:10px;
}

.timebox p{
    font-size:15px;
    line-height:1.5;
}

/* ================= CRIMINAL RECORD ================= */

.crime{
    border:2px dashed #c77aff;
    background:rgba(90,20,120,.15);
    padding:30px;
    border-radius:20px;
}

.stamp{
    display:inline-block;
    border:3px solid #d786ff;
    color:#e09cff;
    padding:8px 15px;
    transform:rotate(-5deg);
    font-weight:bold;
    margin-bottom:20px;
}

/* ================= FINAL ================= */

.final{
    position:relative;
}

.blessing{
    font-size:clamp(23px,4vw,38px);
    color:#f0caff;
    margin:30px 0;
    line-height:1.7;
    font-weight:bold;
}

.signature{
    margin-top:30px;
    color:#dca3ff;
    font-size:18px;
}

/* ================= NAVIGATION ================= */

.nav{
    position:fixed;
    bottom:20px;
    left:50%;
    transform:translateX(-50%);
    display:flex;
    align-items:center;
    gap:15px;
    z-index:50;
}

.nav button{
    margin:0;
    width:50px;
    height:50px;
    padding:0;
    font-size:20px;
}

.counter{
    background:rgba(0,0,0,.45);
    padding:9px 16px;
    border-radius:30px;
    border:1px solid rgba(255,255,255,.15);
    font-size:13px;
}

.music{
    position:fixed;
    top:20px;
    right:20px;
    z-index:60;
    width:48px;
    height:48px;
    border-radius:50%;
    padding:0;
    margin:0;
    font-size:20px;
}

/* ================= REVEAL ================= */

.blackout{
    background:#000;
}

.blackout .content{
    animation:glowText 2s infinite alternate;
}

@keyframes glowText{
    from{text-shadow:0 0 10px #a94cff;}
    to{text-shadow:0 0 40px #e18aff;}
}

/* ================= CONFETTI ================= */

.confetti{
    position:fixed;
    width:8px;
    height:8px;
    top:-20px;
    z-index:100;
    pointer-events:none;
    animation:confettiFall 4s linear forwards;
}

@keyframes confettiFall{
    to{
        transform:translateY(110vh) rotate(720deg);
        opacity:0;
    }
}

/* ================= MOBILE ================= */

@media(max-width:700px){

    .slide{
        align-items:flex-start;
        padding-top:75px;
        padding-bottom:120px;
    }

    .content{
        padding:25px 12px;
    }

    .card{
        padding:22px 18px;
    }

    .timeline{
        grid-template-columns:1fr 1fr;
    }

    .timeline .timebox p{
        font-size:14px;
    }

    h1{
        font-size:55px;
    }

    .emoji{
        font-size:50px;
    }

    .big-heart{
        font-size:70px;
    }
}

@media(max-width:420px){

    .timeline{
        grid-template-columns:1fr;
    }

    p{
        font-size:16px;
    }

    h2{
        font-size:32px;
    }
}
</style>
</head>

<body>

<div class="stars"></div>

<!-- FLOATING DECORATIONS -->

<div class="float" style="left:5%;animation-duration:12s;">💜</div>
<div class="float" style="left:15%;animation-duration:15s;animation-delay:2s;">🤍</div>
<div class="float" style="left:28%;animation-duration:11s;animation-delay:4s;">🌸</div>
<div class="float" style="left:42%;animation-duration:14s;animation-delay:1s;">💜</div>
<div class="float" style="left:57%;animation-duration:13s;animation-delay:5s;">✨</div>
<div class="float" style="left:70%;animation-duration:16s;animation-delay:3s;">🤍</div>
<div class="float" style="left:84%;animation-duration:12s;animation-delay:6s;">🌷</div>
<div class="float" style="left:94%;animation-duration:14s;animation-delay:2s;">💜</div>


<!-- MUSIC BUTTON -->

<button class="music" onclick="toggleMusic()" id="musicBtn">🔇</button>


<!-- =====================================================
SLIDE 1
===================================================== -->

<section class="slide active">

<div class="content">

<div class="small">⚠ CLASSIFIED BIRTHDAY FILE ⚠</div>

<div class="emoji">💜</div>

<h1>AGASTHIYA</h1>

<p>
A very suspicious file has been discovered...
</p>

<div class="card">

<p>
Inside this file are classified memories,<br>
criminal activities, unfinished food promises,<br>
and one extremely crazy friendship.
</p>

</div>

<button onclick="startExperience()">
OPEN THE FILE 💜
</button>

<p style="font-size:13px;margin-top:20px;color:#aa91bd;">
🎵 Tap the button to start the birthday BGM
</p>

</div>

</section>


<!-- =====================================================
SLIDE 2
===================================================== -->

<section class="slide">

<div class="content">

<div class="small">FILE 001 • ORIGIN STORY</div>

<div class="emoji">🎓</div>

<h2>Once Upon A Time...</h2>

<div class="card">

<p>
First year...
</p>

<p>
We were just classmates.
</p>

<br>

<p>
Just normal friends.
</p>

<br>

<p>
Nothing suspicious.
Nothing dramatic.
Nothing special.
</p>

<br>

<p class="highlight">
AND THEN SECOND YEAR HAPPENED.
</p>

</div>

<p>
Somewhere between random conversations,
jokes, teasing and college chaos...
</p>

</div>

</section>


<!-- =====================================================
SLIDE 3
===================================================== -->

<section class="slide">

<div class="content">

<div class="small">THE EVOLUTION OF THIS FRIENDSHIP</div>

<h2>From Classmate → Best Friend 💜</h2>

<div class="timeline">

<div class="timebox">
<h3>1st YEAR</h3>
<p>
"Hi, friend."
<br><br>
Normal classmates.
</p>
</div>

<div class="timebox">
<h3>2nd YEAR</h3>
<p>
More conversations.
<br>
More jokes.
<br>
More chaos.
</p>
</div>

<div class="timebox">
<h3>3rd YEAR</h3>
<p>
Now we know
WAY TOO MUCH
about each other.
😭
</p>
</div>

<div class="timebox">
<h3>FINAL YEAR</h3>
<p>
Somehow...
you became
one of my closest people.
💜
</p>
</div>

</div>

<div class="card">

<p>
Funny how some people enter your life
as just classmates...
</p>

<br>

<p class="highlight">
and somehow become family-level friends.
</p>

</div>

</div>

</section>


<!-- =====================================================
SLIDE 4
===================================================== -->

<section class="slide">

<div class="content">

<div class="small">CONFIDENTIAL EVIDENCE</div>

<div class="emoji">🚨🐸🚨</div>

<h2>THE RENUKA INCIDENT</h2>

<div class="crime">

<div class="stamp">
CRIMINAL RECORD
</div>

<p>
HOD Renuka was teaching...
</p>

<br>

<p>
Meanwhile...
</p>

<br>

<p class="highlight">
THE TWO OF US:
<br>
🐸 "FROG THIS..."
<br>
🐸 "FROG THAT..."
</p>

<br>

<p>
Trying not to laugh while she was teaching
was basically a full-time job.
😭
</p>

<br>

<p>
And somehow...
we survived that class.
</p>

</div>

</div>

</section>


<!-- =====================================================
SLIDE 5
===================================================== -->

<section class="slide">

<div class="content">

<div class="small">CASE FILE 005</div>

<div class="emoji">🍞😭</div>

<h2>THE BREAD HALWA CASE</h2>

<div class="card">

<p>
First year:
</p>

<br>

<p class="highlight">
"Agasthiya, make me bread halwa."
</p>

<br>

<p>
Agasthiya:
<br>
"Sure sure..."
</p>

<br>

<p>
Years passed...
</p>

<br>

<p>
Third year...
</p>

<br>

<p>
Final year...
</p>

<br>

<p>
Graduation is approaching...
</p>

<br>

<h2 style="font-size:30px;">
THE HALWA IS STILL IN PRODUCTION.
😭🍞
</h2>

</div>

<p>
At this point I'm convinced
the bread halwa is a myth.
</p>

</div>

</section>


<!-- =====================================================
SLIDE 6
===================================================== -->

<section class="slide">

<div class="content">

<div class="small">🚨 SECRET ARCHIVES 🚨</div>

<h2>AGASTHIYA'S FILE</h2>

<div class="card">

<p>
📱 <span class="highlight">THE SNAPCHAT FILE</span>
</p>

<p>
The mysterious fake ID...
The flirting...
The investigations...
😭
</p>

</div>

<div class="card">

<p>
👀 <span class="highlight">THE DEVAN FILE</span>
</p>

<p>
"Don't look at his stories."
<br><br>
Meanwhile...
you're telling ME about the stories.
😭
</p>

</div>

<div class="card">

<p>
📖 <span class="highlight">THE MANI ARCHIVES</span>
</p>

<p>
So many stories about your school friend Mani...
</p>

<br>

<p>
Honestly,
your life has been running
like a podcast in my ears.
😂
</p>

</div>

</div>

</section>


<!-- =====================================================
SLIDE 7
===================================================== -->

<section class="slide blackout">

<div class="content">

<div class="small">WAIT...</div>

<h2>
YOU THOUGHT...
</h2>

<h1 style="font-size:clamp(45px,10vw,90px);">
THIS WAS JUST
A BIRTHDAY WEBSITE?
</h1>

<p>
😈
</p>

<br>

<p class="highlight">
NOPE.
</p>

</div>

</section>


<!-- =====================================================
SLIDE 8
===================================================== -->

<section class="slide">

<div class="content">

<div class="small">THE REAL MESSAGE</div>

<div class="big-heart">💜</div>

<h2>THANK YOU, AGASTHIYA.</h2>

<div class="card">

<p>
Thank you for all the random laughs.
</p>

<br>

<p>
Thank you for the stupid jokes.
</p>

<br>

<p>
Thank you for the college chaos.
</p>

<br>

<p>
Thank you for listening to
all my nonsense too.
😭
</p>

<br>

<p class="highlight">
Most importantly...
thank you for becoming
one of my closest friends.
</p>

</div>

<p>
We didn't start as best friends.
<br>
We became best friends somewhere
along the way.
💜
</p>

</div>

</section>


<!-- =====================================================
SLIDE 9
===================================================== -->

<section class="slide">

<div class="content">

<div class="small">FINAL YEAR • LAST COLLEGE BIRTHDAY</div>

<div class="emoji">🎓✨</div>

<h2>AND NOW...</h2>

<div class="card">

<p>
Final year.
</p>

<br>

<p>
Our last birthday together
as college students.
</p>

<br>

<p>
After this,
everyone will go in different directions.
</p>

<br>

<p class="highlight">
But I genuinely wish you the best.
</p>

</div>

<div class="card">

<p>
May you get a
<strong>GOOD JOB</strong>.
</p>

<br>

<p>
May you get a
<strong>HIGH SALARY</strong>.
💰
</p>

<br>

<p>
May your future be peaceful,
happy and full of success.
✨
</p>

</div>

</div>

</section>


<!-- =====================================================
SLIDE 10
===================================================== -->

<section class="slide final">

<div class="content">

<div class="small">FINAL MESSAGE</div>

<div class="emoji">🤍🌸🤍</div>

<h2>
Different backgrounds.<br>
Same friendship.
</h2>

<p style="font-size:45px;margin:25px;">
☪️ 🤍 🕉️ 🤍
</p>

<div class="blessing">

என் ஆசீர்வாதம் என்றும் உனக்கு உண்டு, மகளே. 🤍

</div>

<div class="card">

<p>
Whatever happens after college...
</p>

<br>

<p>
Keep that crazy smile.
😂
</p>

<br>

<p>
Keep being funny.
</p>

<br>

<p>
Keep annoying everyone.
😭
</p>

<br>

<p class="highlight">
AND PLEASE...
MAKE THAT BREAD HALWA.
🍞😭
</p>

</div>

<h1 style="font-size:clamp(40px,8vw,75px);">
HAPPY BIRTHDAY
<br>
AGASTHIYA 💜
</h1>

<p>
28 • SEPTEMBER
</p>

<div class="signature">
With lots of love & endless friendship 🤍
</div>

</div>

</section>


<!-- NAVIGATION -->

<div class="nav">

<button onclick="previousSlide()">‹</button>

<div class="counter">
<span id="current">1</span> / 10
</div>

<button onclick="nextSlide()">›</button>

</div>


<script>

/* =====================================================
SLIDE SYSTEM
===================================================== */

let currentSlide = 0;

const slides = document.querySelectorAll(".slide");
const currentCounter = document.getElementById("current");

function showSlide(index){

    if(index < 0) index = 0;

    if(index >= slides.length)
        index = slides.length - 1;

    slides.forEach(slide=>{
        slide.classList.remove("active");
    });

    slides[index].classList.add("active");

    currentSlide = index;

    currentCounter.textContent = index + 1;

    window.scrollTo({
        top:0,
        behavior:"smooth"
    });

    if(index === slides.length - 1){
        createConfetti();
    }
}

function nextSlide(){

    if(currentSlide < slides.length - 1){

        showSlide(currentSlide + 1);

        if(currentSlide === 6){
            blackoutEffect();
        }
    }
}

function previousSlide(){

    if(currentSlide > 0){
        showSlide(currentSlide - 1);
    }
}


/* =====================================================
KEYBOARD
===================================================== */

document.addEventListener("keydown",function(e){

    if(e.key === "ArrowRight"){
        nextSlide();
    }

    if(e.key === "ArrowLeft"){
        previousSlide();
    }

});


/* =====================================================
SYNTHESIZED BIRTHDAY BGM
NO EXTERNAL MP3 REQUIRED
===================================================== */

let audioContext;
let masterGain;
let musicPlaying = false;
let musicTimer;

const notes = [
    261.63,
    329.63,
    392.00,
    523.25,
    392.00,
    329.63,
    293.66,
    349.23
];

let noteIndex = 0;

function initMusic(){

    if(audioContext) return;

    audioContext =
        new (window.AudioContext || window.webkitAudioContext)();

    masterGain = audioContext.createGain();

    masterGain.gain.value = 0.08;

    masterGain.connect(audioContext.destination);
}


function playNote(){

    if(!musicPlaying) return;

    const osc = audioContext.createOscillator();

    const gain = audioContext.createGain();

    osc.type = "sine";

    osc.frequency.value = notes[noteIndex];

    gain.gain.setValueAtTime(
        0.0001,
        audioContext.currentTime
    );

    gain.gain.exponentialRampToValueAtTime(
        0.12,
        audioContext.currentTime + 0.05
    );

    gain.gain.exponentialRampToValueAtTime(
        0.0001,
        audioContext.currentTime + 1.2
    );

    osc.connect(gain);
    gain.connect(masterGain);

    osc.start();

    osc.stop(
        audioContext.currentTime + 1.3
    );

    noteIndex++;

    if(noteIndex >= notes.length){
        noteIndex = 0;
    }

    musicTimer = setTimeout(
        playNote,
        520
    );
}


function startMusic(){

    initMusic();

    if(audioContext.state === "suspended"){
        audioContext.resume();
    }

    if(!musicPlaying){

        musicPlaying = true;

        document.getElementById("musicBtn").textContent = "🎵";

        playNote();
    }
}


function stopMusic(){

    musicPlaying = false;

    clearTimeout(musicTimer);

    document.getElementById("musicBtn").textContent = "🔇";
}


function toggleMusic(){

    if(musicPlaying){
        stopMusic();
    }else{
        startMusic();
    }
}


/* =====================================================
OPEN EXPERIENCE
===================================================== */

function startExperience(){

    startMusic();

    createConfetti();

    showSlide(1);
}


/* =====================================================
BLACKOUT EFFECT
===================================================== */

function blackoutEffect(){

    setTimeout(()=>{

        const slide = slides[6];

        slide.style.background =
            "radial-gradient(circle,#25053d,#000 70%)";

    },100);
}


/* =====================================================
CONFETTI
===================================================== */

function createConfetti(){

    const symbols = [
        "💜",
        "🤍",
        "✨",
        "🌸",
        "🎉"
    ];

    for(let i=0;i<45;i++){

        const item =
            document.createElement("div");

        item.className = "confetti";

        item.textContent =
            symbols[
                Math.floor(
                    Math.random()*symbols.length
                )
            ];

        item.style.left =
            Math.random()*100 + "vw";

        item.style.animationDuration =
            (2 + Math.random()*3) + "s";

        item.style.fontSize =
            (10 + Math.random()*18) + "px";

        document.body.appendChild(item);

        setTimeout(()=>{
            item.remove();
        },5000);
    }
}


/* =====================================================
SWIPE SUPPORT
===================================================== */

let touchStartX = 0;

document.addEventListener("touchstart",function(e){

    touchStartX =
        e.changedTouches[0].screenX;

});

document.addEventListener("touchend",function(e){

    const touchEndX =
        e.changedTouches[0].screenX;

    const difference =
        touchStartX - touchEndX;

    if(Math.abs(difference) > 60){

        if(difference > 0){
            nextSlide();
        }else{
            previousSlide();
        }

    }

});

</script>

</body>
</html>
