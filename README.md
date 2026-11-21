
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>The Mexican Revolution | An Animated Story</title>
<style>
:root{--ink:#263238;--paper:#fff8e9;--red:#b83b32;--green:#28734d;--gold:#e6b44c}
*{box-sizing:border-box}
body{margin:0;background:#f2e6cf;color:var(--ink);font-family:Georgia,serif}
header{text-align:center;padding:24px 16px 12px;background:#fff8e9}
h1{margin:0;color:#8d302b;font-size:clamp(1.8rem,5vw,3rem)}
header p{margin:8px auto 0;max-width:760px;font:1rem/1.5 Arial,sans-serif}
main{max-width:1050px;margin:20px auto;padding:0 14px}
.stage{background:#fff8e9;border:5px solid #573d2e;border-radius:18px;overflow:hidden;box-shadow:0 8px 24px #4b342533}
.scene-top{display:flex;justify-content:space-between;gap:10px;padding:12px 16px;background:#573d2e;color:white;font:bold 14px Arial,sans-serif}
svg{display:block;width:100%;height:auto;background:#9bd3df}
.land{fill:#b6a36b}.hill{fill:#8b9d62}.sun{fill:#f8d66d}
.building{fill:#e8d2a6;stroke:#75553d;stroke-width:4}.roof{fill:#a94d3e}
.person{transform-box:fill-box;transform-origin:center bottom}
.walk{animation:walk 1s ease-in-out infinite alternate}
@keyframes walk{from{transform:translateX(-5px) rotate(-2deg)}to{transform:translateX(5px) rotate(2deg)}}
.cloud{fill:#fff;opacity:.9}
.bubble{fill:#fff;stroke:#573d2e;stroke-width:3}
.bubbletext{font:bold 19px Arial,sans-serif;fill:#263238}
.dialogue{padding:18px 20px;text-align:center;min-height:130px}
.speaker{font:bold 14px Arial,sans-serif;text-transform:uppercase;letter-spacing:1.5px;color:#8d302b}
.line{font:clamp(1.05rem,2.6vw,1.45rem)/1.55 Arial,sans-serif;margin:8px auto;max-width:850px}
.line strong{color:#a3332b}
.line u{text-decoration-color:#28734d;text-decoration-thickness:2px;text-underline-offset:4px}
.controls{display:flex;flex-wrap:wrap;justify-content:center;gap:10px;padding:0 16px 18px}
button{border:0;border-radius:30px;padding:12px 20px;background:#28734d;color:white;font:bold 15px Arial,sans-serif;cursor:pointer}
button.secondary{background:#573d2e}
button:disabled{opacity:.45;cursor:not-allowed}
.progress{height:9px;background:#e4d7bd}
.bar{height:100%;width:0;background:#b83b32;transition:width .3s}
section.info{display:none;margin:24px 0;background:#fff8e9;border-radius:16px;padding:22px}
section.info h2{color:#8d302b;margin-top:0}
.events{display:grid;grid-template-columns:repeat(auto-fit,minmax(230px,1fr));gap:14px}
.event{padding:15px;border-left:5px solid var(--green);background:#f4ecd9;border-radius:8px;font:15px/1.5 Arial,sans-serif}
.event h3{margin:0 0 7px;color:#8d302b}
.transcript{white-space:pre-wrap;font:15px/1.7 Arial,sans-serif;background:#f4ecd9;padding:16px;border-radius:10px}
footer{text-align:center;padding:20px;color:#665747;font:13px Arial,sans-serif}
@media(max-width:600px){.scene-top{font-size:12px}.bubbletext{font-size:15px}.dialogue{min-height:155px}}
</style>
</head>
<body>

<header>
<h1>The Mexican Revolution</h1>
<p>An animated story about the people, ideas, and events that changed Mexico (1910–1917).</p>
</header>

<main>
<div class="stage">
 <div class="scene-top">
  <span id="chapter">Chapter 1 of 6</span>
  <span id="year">1910</span>
 </div>

 <svg id="picture" viewBox="0 0 900 430" role="img" aria-label="Animated illustration of the Mexican Revolution">
  <circle class="sun" cx="760" cy="78" r="42"/>
  <path class="cloud" d="M80 90q5-30 38-22 20-34 52-5 35-4 37 27z"/>
  <path class="hill" d="M0 270Q180 190 360 270T720 250T900 270V430H0Z"/>
  <path class="land" d="M0 330Q220 290 450 340T900 320V430H0Z"/>

  <g id="town">
   <rect class="building" x="65" y="170" width="210" height="160"/>
   <path class="roof" d="M45 175L170 90 295 175Z"/>
   <rect x="145" y="235" width="52" height="95" fill="#78523c"/>
   <rect x="90" y="205" width="40" height="38" fill="#83b6c2"/>
   <rect x="210" y="205" width="40" height="38" fill="#83b6c2"/>
  </g>

  <g id="hero" class="person walk">
   <circle cx="0" cy="0" r="23" fill="#9b5e3c"/>
   <path d="M-27 -7Q0 -45 28 -7Z" fill="#6b442e"/>
   <path d="M-22 25Q0 13 22 25L30 112H-30Z" fill="#28734d"/>
   <path d="M-18 110L-22 175M18 110L22 175" stroke="#49352b" stroke-width="13" stroke-linecap="round"/>
   <path d="M-26 45L-52 90M26 45L52 90" stroke="#9b5e3c" stroke-width="11" stroke-linecap="round"/>
  </g>

  <g id="friend" class="person">
   <circle cx="0" cy="0" r="22" fill="#b8784c"/>
   <path d="M-26 -8Q0 -43 27 -8Z" fill="#5b3929"/>
   <path d="M-24 25Q0 14 24 25L29 110H-29Z" fill="#b83b32"/>
   <path d="M-16 108L-20 170M16 108L20 170" stroke="#49352b" stroke-width="13" stroke-linecap="round"/>
   <path d="M-23 48L-48 88M23 48L48 88" stroke="#b8784c" stroke-width="11" stroke-linecap="round"/>
  </g>

  <g id="horse" style="display:none">
   <path d="M0 0q35-35 70-5l22 35-12 13-20-24-30 8-20-15-18 22-10-8z" fill="#70462f"/>
   <path d="M15 38l-5 40m35-40l5 40m25-45l7 45" stroke="#49352b" stroke-width="8"/>
   <path d="M62 -10l20-25 9 4-12 28" fill="#70462f"/>
  </g>

  <g id="speech" style="display:none">
   <rect class="bubble" x="380" y="35" width="450" height="100" rx="22"/>
   <path class="bubble" d="M430 132l-25 30 65-28"/>
   <text id="bubbleText" class="bubbletext" x="405" y="75"></text>
  </g>
 </svg>

 <div class="progress"><div class="bar" id="bar"></div></div>

 <div class="dialogue">
  <div class="speaker" id="speaker">Narrator</div>
  <div class="line" id="line">Press play to begin the story.</div>
 </div>

 <div class="controls">
  <button id="play">▶ Play story</button>
  <button class="secondary" id="pause" disabled>Pause</button>
  <button class="secondary" id="restart">Start again</button>
 </div>
</div>

<section class="info" id="summary">
 <h2>Six important moments of the Mexican Revolution</h2>

 <div class="events">
  <article class="event">
   <h3>1. The Plan of San Luis (1910)</h3>
   Francisco I. Madero called for an uprising against Porfirio Díaz and demanded free elections.
  </article>

  <article class="event">
   <h3>2. The uprising begins (November 20, 1910)</h3>
   Revolutionary groups in different parts of Mexico took up the call to challenge Díaz's government.
  </article>

  <article class="event">
   <h3>3. Díaz resigns (May 1911)</h3>
   After the revolutionaries gained strength, Porfirio Díaz resigned and went into exile.
  </article>

  <article class="event">
   <h3>4. The Decena Trágica (February 1913)</h3>
   A coup removed Madero from power. He and Vice President José María Pino Suárez were later assassinated.
  </article>

  <article class="event">
   <h3>5. The struggle against Huerta (1913–1914)</h3>
   Constitutionalist forces led by Venustiano Carranza, with important leaders such as Villa and Zapata, fought Huerta's government.
  </article>

  <article class="event">
   <h3>6. The Constitution of 1917</h3>
   The new Constitution established important social rights, including education, labor protections, and rules about land.
  </article>
 </div>

 <h2 style="margin-top:28px">Complete story transcript</h2>
 <div class="transcript" id="transcript"></div>
</section>
</main>

<footer>Educational project · The Mexican Revolution · 1910–1917</footer>

<script>
const scenes=[
 {
  year:"1910",
  place:"A town in Mexico",
  t:"At the beginning of the twentieth century, Porfirio Díaz had ruled Mexico for many years. Many people wanted fair elections and better opportunities.",
  x:"Madero",
  y:"People should be able to choose their president. <b>Therefore</b>, I am calling for a new beginning.",
  friend:"Villager",
  p:"A new beginning? What can we do?",
  horse:false
 },
 {
  year:"November 20, 1910",
  place:"The call to rise up",
  t:"In the Plan of San Luis, Francisco I. Madero called on Mexicans to rise up on November 20, 1910. Rebellions began in several regions.",
  x:"Revolutionary",
  y:"The call has reached us! <u>On November 20</u>, we will rise up.",
  friend:"Villager",
  p:"We want change, <b>because</b> our voices must be heard.",
  horse:true
 },
 {
  year:"May 1911",
  place:"The end of Díaz's rule",
  t:"The revolutionary movement grew. <u>In May 1911</u>, Porfirio Díaz resigned and left Mexico. Madero later won the presidential election.",
  x:"Villager",
  y:"Díaz has resigned. Is this the change we hoped for?",
  friend:"Madero supporter",
  p:"It is an important step, <b>but</b> the country still faces many challenges.",
  horse:false
 },
 {
  year:"February 1913",
  place:"Mexico City",
  t:"In February 1913, a coup known as the Decena Trágica brought a violent end to Madero's government. Victoriano Huerta took power. Madero and Pino Suárez were assassinated.",
  x:"Messenger",
  y:"Huerta has taken power. The struggle is not over.",
  friend:"Citizen",
  p:"<u>After</u> this coup, many people joined the fight against Huerta.",
  horse:false
 },
 {
  year:"1913–1914",
  place:"Across Mexico",
  t:"Venustiano Carranza led the Constitutionalist movement against Huerta. Revolutionary leaders such as Francisco Villa and Emiliano Zapata also shaped the struggle, although they had different goals.",
  x:"Constitutionalist",
  y:"We must end Huerta's government, <b>so</b> Mexico can move forward.",
  friend:"Villager",
  p:"Our communities also need land and justice.",
  horse:true
 },
 {
  year:"1917",
  place:"A new Constitution",
  t:"The Constitution of 1917 was adopted on February 5. It included major social reforms involving education, labor rights, and land. The armed conflict continued in some areas, <b>but</b> the Constitution became a foundation for a new political era.",
  x:"Teacher",
  y:"The Constitution recognizes important rights for the people.",
  friend:"Student",
  p:"<u>From now on</u>, we must work to make those rights real.",
  horse:false
 }
];

let index=0,playing=false,paused=false,step=0;
let utterance=null;
const $=id=>document.getElementById(id);

function esc(s){
 return s.replace(/&/g,"&amp;").replace(/</g,"&lt;").replace(/>/g,"&gt;");
}

function render(){
 const s=scenes[index];

 $("chapter").textContent=`Chapter ${index+1} of 6 · ${s.place}`;
 $("year").textContent=s.year;

 $("hero").setAttribute("transform",`translate(${index%2?300:250},220)`);
 $("friend").setAttribute("transform",`translate(${index%2?610:650},220)`);

 $("horse").style.display=s.horse?"":"none";
 $("horse").setAttribute("transform","translate(700,290)");

 $("speech").style.display="none";
 $("line").innerHTML="Press <b>Play story</b> to hear the next part.";
 $("speaker").textContent="Narrator";
 $("bar").style.width=`${index/scenes.length*100}%`;
}

function speak(text,who,done){
 $("speaker").textContent=who;
 $("line").innerHTML=text;

 if(!("speechSynthesis" in window)){
  done();
  return;
 }

 speechSynthesis.cancel();

 utterance=new SpeechSynthesisUtterance(text.replace(/<[^>]*>/g,""));
 utterance.lang="en-US";
 utterance.rate=.88;

 const voices=speechSynthesis.getVoices();
 const voice=voices.find(v=>v.lang.startsWith("en"));
 if(voice)utterance.voice=voice;

 utterance.onend=done;
 utterance.onerror=done;

 speechSynthesis.speak(utterance);
}

function playStep(){
 if(!playing||paused)return;

 const s=scenes[index];

 if(step===0){
  $("speech").style.display="";
  $("bubbleText").textContent=s.t.slice(0,65)+"…";
  speak(esc(s.t),"Narrator",()=>{
   step++;
   playStep();
  });
 }
 else if(step===1){
  $("bubbleText").textContent=s.x+": "+s.y.slice(0,45)+"…";
  speak(esc(s.y),s.x,()=>{
   step++;
   playStep();
  });
 }
 else if(step===2){
  $("bubbleText").textContent=s.p.slice(0,55)+"…";
  speak(esc(s.p),s.friend,()=>{
   index++;
   step=0;

   if(index<scenes.length){
    render();
    playStep();
   }else{
    finish();
   }
  });
 }
}

function finish(){
 playing=false;
 paused=false;

 $("play").disabled=false;
 $("pause").disabled=true;
 $("play").textContent="▶ Play story";
 $("bar").style.width="100%";
 $("speaker").textContent="The End";

 $("line").textContent="The story is complete. Explore the six important moments and read the full transcript below.";

 $("summary").style.display="block";
 $("summary").scrollIntoView({behavior:"smooth"});
}

function start(){
 if(index>=scenes.length){
  index=0;
  step=0;
  render();
 }

 playing=true;
 paused=false;

 $("play").disabled=true;
 $("pause").disabled=false;
 $("play").textContent="Playing…";

 playStep();
}

$("play").addEventListener("click",start);

$("pause").addEventListener("click",()=>{
 if(!playing)return;

 if(!paused){
  paused=true;
  speechSynthesis.pause();
  $("pause").textContent="Resume";
 }else{
  paused=false;
  speechSynthesis.resume();
  $("pause").textContent="Pause";

  if(!speechSynthesis.speaking)playStep();
 }
});

$("restart").addEventListener("click",()=>{
 if("speechSynthesis" in window)speechSynthesis.cancel();

 playing=false;
 paused=false;
 index=0;
 step=0;

 $("summary").style.display="none";
 $("pause").disabled=true;
 $("pause").textContent="Pause";
 $("play").disabled=false;
 $("play").textContent="▶ Play story";

 render();
});

$("transcript").textContent=scenes.map((s,i)=>
 `CHAPTER ${i+1} — ${s.year}
NARRATOR: ${s.t}
${s.x.toUpperCase()}: ${s.y.replace(/<[^>]*>/g,"")}
${s.friend.toUpperCase()}: ${s.p.replace(/<[^>]*>/g,"")}`
).join("\n\n");

render();
</script>
</body>
</html>
