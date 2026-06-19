<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Happy Birthday Ankita ❤️</title>
<style>
*{margin:0;padding:0;box-sizing:border-box;}
body{font-family:'Segoe UI',sans-serif;background:#000010;color:#fff0f5;overflow:hidden;height:100vh;width:100vw;}
canvas{position:fixed;top:0;left:0;z-index:0;}
.screen{position:fixed;top:0;left:0;width:100%;height:100%;display:flex;flex-direction:column;align-items:center;justify-content:center;z-index:10;transition:opacity 0.8s ease;opacity:1;}
.screen.hidden{opacity:0;pointer-events:none;}
#giftScreen{cursor:pointer;}
.gift-wrap{position:relative;width:160px;height:160px;margin-bottom:30px;}
.gift-box-body{position:absolute;bottom:0;left:0;width:160px;height:110px;background:linear-gradient(135deg,#e8005a,#ff6090);border-radius:6px;box-shadow:0 8px 30px rgba(255,80,140,0.5);}
.gift-box-lid{position:absolute;top:0;left:-8px;width:176px;height:45px;background:linear-gradient(135deg,#ff2070,#ff80b0);border-radius:6px;box-shadow:0 4px 15px rgba(255,80,140,0.4);transition:transform 0.5s ease,opacity 0.5s ease;}
.gift-ribbon-v{position:absolute;left:50%;transform:translateX(-50%);width:22px;height:100%;background:linear-gradient(to bottom,#fff0,#fffb,#fff5);z-index:2;}
.gift-ribbon-h{position:absolute;top:50%;transform:translateY(-50%);width:100%;height:22px;background:linear-gradient(to right,#fff0,#fffb,#fff5);z-index:2;}
.gift-bow{position:absolute;top:-22px;left:50%;transform:translateX(-50%);z-index:3;font-size:2.5rem;}
.bounce{animation:bounce 1.2s ease-in-out infinite;}
@keyframes bounce{0%,100%{transform:translateY(0)}50%{transform:translateY(-12px)}}
.gift-title{font-size:1.6rem;color:#ff9ec4;text-align:center;text-shadow:0 0 20px rgba(255,100,150,0.8);}
.gift-sub{font-size:0.9rem;color:#ffcce0;margin-top:10px;opacity:0.7;}
.sparkle{font-size:1.2rem;animation:spin 3s linear infinite;display:inline-block;}
@keyframes spin{to{transform:rotate(360deg)}}
#envelopeScreen{cursor:pointer;}
.envelope-wrap{position:relative;width:280px;height:180px;margin-bottom:30px;}
.envelope-body{width:280px;height:180px;background:linear-gradient(135deg,#2a0020,#4a0035);border:2px solid rgba(255,100,150,0.4);border-radius:8px;position:relative;box-shadow:0 10px 40px rgba(255,80,140,0.4);}
.envelope-flap{position:absolute;top:0;left:0;width:0;height:0;border-left:140px solid transparent;border-right:140px solid transparent;border-top:100px solid #ff6090;transform-origin:top center;transition:transform 1.2s cubic-bezier(0.4,0,0.2,1);z-index:5;}
.envelope-flap.open{transform:rotateX(180deg);}
.envelope-bottom{position:absolute;bottom:0;left:0;width:0;height:0;border-left:140px solid transparent;border-right:140px solid transparent;border-bottom:90px solid rgba(180,0,80,0.5);}
.envelope-left{position:absolute;top:0;left:0;width:0;height:0;border-top:90px solid transparent;border-bottom:90px solid transparent;border-left:130px solid rgba(200,0,90,0.3);}
.envelope-right{position:absolute;top:0;right:0;width:0;height:0;border-top:90px solid transparent;border-bottom:90px solid transparent;border-right:130px solid rgba(200,0,90,0.3);}
.envelope-heart{position:absolute;top:50%;left:50%;transform:translate(-50%,-20%);font-size:2rem;animation:beat 1s infinite alternate;}
@keyframes beat{from{transform:translate(-50%,-20%) scale(1)}to{transform:translate(-50%,-20%) scale(1.2)}}
.env-title{font-size:1.3rem;color:#ff9ec4;text-align:center;}
.env-sub{font-size:0.85rem;color:#ffcce0;margin-top:8px;opacity:0.7;}
#contentScreen{overflow:hidden;flex-direction:row;}
.pages-container{display:flex;height:100vh;width:100vw;will-change:transform;}
.page{min-width:100vw;height:100vh;overflow-y:auto;padding:30px 20px;display:flex;flex-direction:column;align-items:center;}
.page::-webkit-scrollbar{width:4px;}
.page::-webkit-scrollbar-thumb{background:rgba(255,100,150,0.4);border-radius:2px;}
.swipe-hint{position:fixed;bottom:25px;left:50%;transform:translateX(-50%);color:rgba(255,158,196,0.45);font-size:0.78rem;letter-spacing:2px;z-index:50;pointer-events:none;transition:opacity 1s ease;}
.card{background:rgba(255,255,255,0.06);max-width:700px;width:100%;margin:20px auto;padding:25px;border-radius:20px;box-shadow:0 10px 25px rgba(255,100,150,0.12);color:#ffe0ec;}
h1{font-size:2.2rem;color:#ff9ec4;text-align:center;margin-bottom:8px;text-shadow:0 0 20px rgba(255,100,150,0.5);}
h2{color:#ff9ec4;margin-bottom:15px;font-size:1.3rem;}
h3{color:#ffcce0;font-size:0.95rem;margin:10px 0;font-weight:400;}
.page-header{text-align:center;padding:30px 20px 10px;}
.page-header p{color:#ffcce0;font-size:1rem;opacity:0.8;}
.heart-anim{font-size:1.8rem;animation:beat 1s infinite alternate;display:inline-block;color:#ff6090;}
.story-chapter{margin-bottom:40px;opacity:0;transform:translateY(30px);transition:opacity 0.7s ease,transform 0.7s ease;}
.story-chapter.visible{opacity:1;transform:translateY(0);}
.chapter-title{color:#ff9ec4;font-size:1rem;font-weight:bold;margin-bottom:10px;padding-bottom:6px;border-bottom:1px solid rgba(255,150,180,0.2);}
.chapter-text{font-size:0.88rem;line-height:1.9;color:#ffe0ec;}
.story-divider{text-align:center;color:rgba(255,158,196,0.35);font-size:1rem;margin:5px 0 35px;letter-spacing:6px;}
.gallery{display:grid;grid-template-columns:repeat(auto-fit,minmax(180px,1fr));gap:12px;margin-top:10px;}
.gallery-item{height:180px;border-radius:12px;background:rgba(255,150,180,0.08);display:flex;align-items:center;justify-content:center;overflow:hidden;border:1px solid rgba(255,100,150,0.15);}
.gallery-item img{width:100%;height:100%;object-fit:cover;border-radius:12px;}
video{width:100%;max-width:600px;border-radius:12px;box-shadow:0 8px 20px rgba(255,100,150,0.25);margin:10px 0;}
.message-text{font-size:0.92rem;line-height:2.1;color:#ffe0ec;text-align:center;}
.confetti-piece{position:fixed;top:-10px;z-index:999;font-size:1.2rem;animation:fall linear forwards;}
@keyframes fall{to{transform:translateY(110vh) rotate(720deg);opacity:0;}}
audio{filter:invert(0.8) hue-rotate(300deg);width:100%;margin-top:10px;}
</style>
</head>
<body>

<canvas id="starCanvas"></canvas>

<!-- SCREEN 1: GIFT BOX -->
<div class="screen" id="giftScreen" onclick="openGift()">
  <div class="gift-wrap bounce">
    <div class="gift-box-body">
      <div class="gift-ribbon-v"></div>
      <div class="gift-ribbon-h"></div>
    </div>
    <div class="gift-box-lid" id="giftLid">
      <div class="gift-ribbon-v"></div>
      <div class="gift-ribbon-h"></div>
    </div>
    <div class="gift-bow">🎀</div>
  </div>
  <div class="gift-title"><span class="sparkle">✨</span> Happy Birthday Ankita! <span class="sparkle">✨</span></div>
  <div class="gift-sub">Click the gift to open 🎁</div>
</div>

<!-- SCREEN 2: ENVELOPE -->
<div class="screen hidden" id="envelopeScreen" onclick="openEnvelope()">
  <div class="envelope-wrap">
    <div class="envelope-body">
      <div class="envelope-flap" id="envFlap"></div>
      <div class="envelope-bottom"></div>
      <div class="envelope-left"></div>
      <div class="envelope-right"></div>
      <div class="envelope-heart">💌</div>
    </div>
  </div>
  <div class="env-title">A letter for you 💕</div>
  <div class="env-sub">Click the envelope to open</div>
</div>

<!-- SCREEN 3: CONTENT PAGES -->
<div class="screen hidden" id="contentScreen">
  <div class="pages-container" id="pagesContainer">

    <!-- PAGE 1 -->
    <div class="page" id="page0">
      <div class="page-header">
        <h1>Happy Birthday Ankitaa ❤️😊</h1>
        <p>God bless you mera bccha. Bhgwan ji aapko Humesha khush rakhe jii. ❤️❤️</p>
        <div class="heart-anim">💖</div>
      </div>
      <div class="card">
        <h2>Our Song 🎶</h2>
        <audio controls loop>
          <source src="Mehak - Kartik prod. ABS _ (Official Visualiser) _ 5.5 Records.mp3" type="audio/mpeg">
        </audio>
      </div>
    </div>

    <!-- PAGE 2: STORY -->
    <div class="page" id="page1">
      <div class="card" style="max-width:700px;margin-bottom:40px;">
        <h2>Our Story ❤️😝🧿</h2>

        <div class="story-chapter">
          <div class="chapter-title">📖 Chapter - 0 - Introduction</div>
          <div class="chapter-text">"I'll never fall in love, again until I found her ...and i would never fall unless it's I've fallen to ..I lost " ah ...ohh toh tumne mujhe dhud liya ....Toh ab kese dhunda ye sb formality hatate h ...
Ye hai meri kahani jha mai mila uss shaks se jo mere liye aage chlke itna khaas hogya ki mene uske liye hrr chiz hasil Krli ( ofc jo mere bss mei tha 🤧)
.....Toh shuru krte h ..ye baat h uss zamane kiii....oh sorry 😅 ye baat h 2024 ki...I saw a girl..Kya lgta h 😂...Ese describe kri hogi....Nh nh nh 😂Listen ...let's imagine....
A school corridor.. usme ek ldki aayi chlke uske baal aadhe brown or aadhe black esa rang jisme koi bhi insan khona chahega ofc mai khoya ... Pr chhodo abhi..Uski aakhe itni pyari..Unn aakho ki itna gehra hona hi khaas tha.....
Vo aakhe ager kisi laash ko dekhle toh use zinda krr de vo aakho ne uss vkt mujhe dekha..........
Socho mera kya hua hoga yaar 😂, khair ....Aage chlte h......
Ab nain naksh ki baat hogyi h toh ab hotho ki trf chlte h..Unn hotho ka rang gulabi jese khud gulab ne vha se janam liya ho jese unhe hi dekh ke bhgwan ne vo rang bnaya ho.....Unn hotho se jo shbd nikle maano jese humare kaano ke liye koi geet
Unka Hnji or ji hi hume itna pyara lgta tha jese bss vo bolti jaaye or hum sunte rhe
Ab agrr niche aaye toh ab sharir ki baat krte h..Unnka chal chalan toh maano jese laxmi ji mere samne chl rhi ho ek ek kadam sakshat kamal ka phool jese lgta tha...
.Or agrr hum unke kadmo ki baat krr hi rhe h toh unke pero ki baat hi krr lete h ...unke per toh mano jese vo phool ki trh thy jise agr chu le toh chune vala amar ho jaye unke pero ki ungliyo tb ko phoolo ki pankhudi jesa bnaya tha bhgwan ne...Toh ab aage chlte h ..
Farmaish h ki kitab ko chhoti rkhna h toh koshish krte h😂....Ab jese ki mene btaya unki nazron ne hume dekha toh hum toh khone hi thy, b agrr hum kho chuke toh unke toh hone hi thy...Heina......Khair,
Kaash vo pll humara hota,
Uss vkt sath bss hum dono ka hota,
Magar kismat ka chaha kux or tha,
Kisi or ldke ki dakhalandazi nh hoti,
Toh aaj vo pll bhi humara hota.........
Samaye bit ta gya humare alg hone ka samaye nazdeek tha magar kismat ka chakkar fir ghuma...
Unka hello humpe khud aaya,
Humari Khushi ka thikana nh tha humne kisiko btana nh tha humne bss baate krni thi or subha tk sona nh tha....
Fir jb humara samay aa hi gya toh ab ye majboor kya krta iss aakho ke doobe shaks ne unse khata krr hi di ki kya vo humse mohobbat krne ki khata krenge...........
Unka jawab hn aaya or unhone humari zindagi ko bhi apne jesa gulab krr diya ab humari zindagi mei kisi ldki or ldki ka ana hi humare liye bhot bdi khata hogi....
Akhir mei sb khata ko hatate hai bhgwan kre aapko bhi ek nh ek din koi axi mahila mile jo aapse bhi mohabbat krne ki khata kre.....</div>
        </div>

        <div class="story-divider">· · · ❤️ · · ·</div>

        <div class="story-chapter">
          <div class="chapter-title">📖 Chapter 1 — The First Glance</div>
          <div class="chapter-text">hmmm..sooo our story begins with the simple eye contact.... Shuru se shuru krte h ...so hua ye ki one day i'm waiting for auto ghar jaane ke liye kiuki school end hogya tha... toh mai auto ka wait krra tha ..tb i know a girl named "deepika"...so deepika bhi auto ke liye aa rhi thi toh uske sath uski ek friend bhi thi....bhyiiii...scchii Love at first sight hogya jiii .....umm hmm ..toh ab aage hum auto mei bethe or mai full bhyi try krra hu ki nh dekhu prr yrr yk ..dil nhi manta.. 🥹</div>
        </div>

        <div class="story-divider">· · · ❤️ · · ·</div>

        <div class="story-chapter">
          <div class="chapter-title">👀 Chapter 2 — Eye Contact Era</div>
          <div class="chapter-text">..okii fir aage kux time tk toh same rha ...uske baad achanak se humari pyaari madam ne eye contact krna shuru kr diya bhyiiii...mtlb thodi halt toh khrab hui meri ..but koi nh okii...toh eye contact hne laga fir vo class mei hoti thi tb jb bhi mai bhar ki trf jata tha ...mtlb bhgwan bhi sath thy thode — madam ki or meri class aas paas ...lesss gooo! 🔥</div>
        </div>

        <div class="story-divider">· · · ❤️ · · ·</div>

        <div class="story-chapter">
          <div class="chapter-title">👋 Chapter 3 — The Wave</div>
          <div class="chapter-text">toh jb bhi bhar se jata tha toh tb bhi eye contact hone laga ...uske baad madam ji ne wave krna shuru krr diya ....bhyii pehle toh lga ki deepika ko krti h lekin nhiii... vo mere liye hi tha...hehe.. toh fir uske baad dheere dheere meri Ankita ji ne hume marna shuru kra — matlb marna vo ni ki kut hi diya ..pyar se yrr! 😄🥹</div>
        </div>

        <div class="story-divider">· · · ❤️ · · ·</div>

        <div class="story-chapter">
          <div class="chapter-title">🤝 Chapter 4 — The Hand Hold</div>
          <div class="chapter-text">toh ye sb tb ek din bhyiii mai exam deke class mei jara tha — vo madam ne mera haath hi pakad liyaaa .....aaaaaaa umm hmm toh haath pakad liya yrr! itna tez heartbeat hua or mai khush andr se huaa yayyyyyyyyy.... mere dost ne bhi chhedna shuru kra ki "iski ek dost h 11th 'b' mei ..DEVVVV" hnn uske baad merko sharam toh aati thi ki yrr ese kiu bolre — prr under se khush...ek dum khush lalalala 😂❤️</div>
        </div>

        <div class="story-divider">· · · ❤️ · · ·</div>

        <div class="story-chapter">
          <div class="chapter-title">📱 Chapter 5 — Instagram Hello</div>
          <div class="chapter-text">mere school life ka THE END... uske baad farewell aayi toh mene miss. Ankita Negi ji ko instagram prr request bheji kiuki mere recommendations mei aaye thy maam...request bheji prr message ni kra sochra tha ki awkward lagega...prr yk — merko samne se maam ka "hello" aaya! lesss goooooo..... "2nd february" — tbhi toh mai asli anniversary ise manta hu kiuki isi din maam ne merko message kiya tha 💌</div>
        </div>

        <div class="story-divider">· · · ❤️ · · ·</div>

        <div class="story-chapter">
          <div class="chapter-title">💘 Chapter 6 — I Love You</div>
          <div class="chapter-text">"12th february, 2025" ko madam ko bola...mene msg kra tha ki "I LIKE YOU"...hnn mene pehle i like you bola tha...hn hn thik h gadha hu mai 😂...toh fir madam ne reject krr diya....kiuki unhe interest hi nhi tha relationship mei...prr mere thode mnane ke baad mene bola "I LOVE YOU" — toh maam bolti h "abhi toh like you tha" aree yrr 😭 uske baad thoda mnane ke baad maam ne kal ka time manga — prr merko aaj hi answer chahiye tha! toh mene bola "mera recharge khtm ho jayega shaam tk" 😄 toh maan gyi maam...thank god!</div>
        </div>

        <div class="story-divider">· · · ❤️ · · ·</div>

        <div class="story-chapter">
          <div class="chapter-title">🌅 Chapter 7 — The Answer</div>
          <div class="chapter-text">Time hora tha shyd 4 ya 4:30 pm ka aas paas...shaam ka time, dil mei dhak dhak ki kya javab hoga...bhyiii literally haath kapre thy mere...toh uske baad madam ka javab aaya...or javab tha — "ab hrr baar sorry bolne ke liye tyar ho jao" 🎉🎉🎉 bhyiiii mai khush ki yayyyyy lesss goooooo... 🥹❤️</div>
        </div>

        <div class="story-divider">· · · ❤️ · · ·</div>

        <div class="story-chapter">
          <div class="chapter-title">🥹 Chapter 8 — Us</div>
          <div class="chapter-text">uske baad hum shaam tk baate krte gye or humari first relationship ki raat gyi h ludo khelke 😄...toh humne pehli baar haath pakada, fir kux time baad humne hug kra first time — lala sukoon ka naam suna h...hn vhi sukoon merko mila 🥹...tb ese hi time beetta gya...december aa gya...or 28th december ko — WE KISSED 😘❤️ YESS BROOOOO WE KISSED! our first kiss — relationship mei bhi or vese bhi! toh ese hi moments share krte krte aaj hume almost 1 saal hone ko aa gya...</div>
        </div>

        <div class="story-divider">· · · 🌌 · · ·</div>

        <div class="story-chapter" style="text-align:center;">
          <div style="font-size:2rem;">❤️</div>
          <div style="font-size:1.2rem;color:#ff9ec4;font-weight:bold;margin:10px 0;">HAPPY BIRTHDAY MERA BCCHA 😊❤️</div>
          <div style="font-size:0.9rem;color:#ffcce0;line-height:2;">I Love You Forever & Always 🌌✨</div>
          <div style="margin-top:20px;"><img src="717153891_953578660820852_309478251932703800_n.jpg" alt="us" style="width:270px;height:400px;object-fit:cover;border-radius:15px;"></div>
          <div style="margin-top:15px;"><img src="WhatsApp Image 2026-02-12 at 5.49.34 PM.jpeg" alt="us" style="width:270px;height:400px;object-fit:cover;border-radius:15px;"></div>
        </div>

      </div>
    </div>

    <!-- PAGE 3: MEMORIES -->
    <div class="page" id="page2">
      <div class="card" style="margin-bottom:40px;">
        <h2>Our Memories 📸</h2>
        <h3>we can't meet regulary because of our long distance, so we generate AI image to show our connection❤️😝..</h3>
        <div class="gallery">
          <div class="gallery-item"><img src="5fac86a7-be7c-41c5-b575-1e88a6ddbd8f.jpg" alt="memory"></div>
          <div class="gallery-item"><img src="94861747-1b1a-4083-9149-ced39cdbd7d0.jpg" alt="memory"></div>
          <div class="gallery-item"><img src="WhatsApp Image 2026-01-27 at 10.38.11 PM.jpeg" alt="memory"></div>
          <div class="gallery-item"><img src="WhatsApp Image 2026-01-27 at 10.38.10 PM.jpeg" alt="memory"></div>
        </div>

        <h2 style="margin-top:25px;">Our Memories 📸</h2>
        <h3>Our Ghibli trend..HEHE 😝❤️..</h3>
        <div class="gallery">
          <div class="gallery-item"><img src="05530801-5f3e-4c44-9c79-61f911585351.jpg" alt="ghibli"></div>
          <div class="gallery-item"><img src="09bfac91-ac9d-4ea2-aa02-ab90373788c7.jpg" alt="ghibli"></div>
          <div class="gallery-item"><img src="5d935f2e-a6a2-44d8-9f5c-e13ba2f76450.jpg" alt="ghibli"></div>
          <div class="gallery-item"><img src="da69fff3-7e60-4308-8b1f-0f29c26a2ef8.jpg" alt="ghibli"></div>
          <div class="gallery-item"><img src="7ba50ddd-6564-44b3-8c7a-dd822e3c5d30.jpg" alt="ghibli"></div>
        </div>

        <h2 style="margin-top:25px;">Our Memories 📸</h2>
        <h3>The special moments and memories we share together🥹❤️🧿..</h3>
        <div class="gallery">
          <div class="gallery-item"><img src="5faa31b2-5c74-4f6c-a53a-16dcbb4cd73d.jpg" alt="moment"></div>
          <div class="gallery-item"><img src="8fc396d4-3958-49d6-8d2b-71af2dc01cdd.jpg" alt="moment"></div>
          <div class="gallery-item"><img src="e34b387f-731f-40f1-a7ef-4065f50fe0c9.jpg" alt="moment"></div>
          <div class="gallery-item"><img src="f6bd4f61-79b3-40e8-8212-39a1778eaa27.jpg" alt="moment"></div>
          <div class="gallery-item"><img src="e32a8f28-a65d-46f9-8401-53665bd17f93.jpg" alt="moment"></div>
        </div>

        <div class="card" style="margin-top:20px;">
          <h2>Our Memories 📸</h2>
          <div class="gallery">
            <h3>The first love letter you gave me ❤️😝..</h3>
            <div class="gallery-item"><img src="7c8d548c-2fbd-43d4-9eb2-7b71c42dd1e0.jpg" alt="letter"></div>
            <h3>The gift you made for me on my birthday (15 december,2025)❤️..</h3>
            <div class="gallery-item"><img src="a3240363-9fd3-4d26-b216-f952f3c0fcd2.jpg" alt="gift"></div>
          </div>

          <h2 style="margin-top:20px;">flowers 📸</h2>
          <div class="gallery">
            <div class="gallery-item"><img src="b109e79d-57c0-40b7-bfc7-76858df225d6.jpg" alt="flowers"></div>
            <h3>The flowers I give to her, on our first meeting ❤️😝..</h3>
          </div>

          <h2 style="margin-top:20px;">Gifts 📸</h2>
          <h3>The gifts i give to her, on her birthday (20th june, 2025)❤️😝..</h3>
          <div class="gallery">
            <div class="gallery-item"><img src="1cfe8034-ef8f-45f4-9455-e96cb182c290.jpg" alt="birthday gift"></div>
          </div>
        </div>

      </div>
    </div>

    <!-- PAGE 4: VIDEOS -->
    <div class="page" id="page3">
      <div class="card" style="margin-bottom:40px;">
        <h2>Our Special Videos 🎥</h2>
        <video controls><source src="WhatsApp Video 2026-01-27 at 10.38.20 PM.mp4" type="video/mp4"></video>
        <video controls><source src="WhatsApp Video 2026-01-27 at 10.38.25 PM.mp4" type="video/mp4"></video>
        <video controls><source src="WhatsApp Video 2026-01-27 at 10.38.40 PM (1).mp4" type="video/mp4"></video>
        <video controls><source src="WhatsApp Video 2026-01-27 at 10.38.41 PM.mp4" type="video/mp4"></video>
        <video controls><source src="WhatsApp Video 2026-01-27 at 10.38.40 PM.mp4" type="video/mp4"></video>
        <video controls><source src="WhatsApp Video 2026-01-27 at 11.39.12 PM.mp4" type="video/mp4"></video>
      </div>
    </div>

    <!-- PAGE 5: MESSAGE -->
    <div class="page" id="page4">
      <div class="card" style="margin-bottom:40px;">
        <h2>A Message for You 💌</h2>
        <p class="message-text">
        hmmm🧐🤔...toh aapka aaj birthday hai 😍😍, sbse pehle aapko HAPPY BIRTHDAY MERA BCCHA❤️😘...humesha khush rehna okiii jese abhi tk ho or mai toh rkhne ki koshish krunga hi ji toh bss😊❤️ ..,
        baaki aap sab filhal pehle se thoda acha krre ho😁💕 , jese ki MERKO PARESHAAAAN😫😫....HMMMMMM😒... hehe😂 mazak krra jii mai pareshan nhi hota aapse
        bss aapko smjhata hu ki thik rha kro apna dhyan rkha kro , ab aapke alava dusri girfriend nhi hai nh meri ya kehlo biwi nhi hai koi dusri 😘😏..
        toh hn mai kehra tha , ki aap pehle se thoda thik krre ho apna dhyan rkhre ho pani thik se pire ki nhi pta nhi prr pina hai okii bccha , 
        fir abhi pdhai ka toh nhi h kux prr vo bhi krte hi thy aap fir baaki mai aapke liye pyaar or kisi chiz ki kaami toh nhi h baaki agar aapko lge ki mai badal gya hu ya aapka ab dhyan nhi rkhta 
        aaap merko bol skte ho bcche, thik hai , baaki apna dhyan rkhna , or yaad rkhna ki  I LOVE YOU ANKITA JI😘❤️ OR HAPPY BIRTHDAY BBU❤️😘
        </p>
        <br>
        <div style="text-align:center;color:#ff9ec4;font-size:1.1rem;margin-top:15px;">
          Made with ❤️ by Dev for Ankita<br>
          <span style="font-size:0.85rem;color:#ffcce0;opacity:0.7;">Forever & Always ✨</span>
        </div>
      </div>
    </div>

  </div>

  <div class="swipe-hint" id="swipeHint">← swipe to navigate →</div>
</div>

<script>
const canvas=document.getElementById('starCanvas');
const ctx=canvas.getContext('2d');
function resizeCanvas(){canvas.width=window.innerWidth;canvas.height=window.innerHeight;}
resizeCanvas();
window.addEventListener('resize',resizeCanvas);
const stars=Array.from({length:250},()=>({x:Math.random()*canvas.width,y:Math.random()*canvas.height,r:Math.random()*2+0.4,alpha:Math.random(),speed:Math.random()*0.012+0.003}));
function drawStars(){ctx.clearRect(0,0,canvas.width,canvas.height);ctx.fillStyle='#000010';ctx.fillRect(0,0,canvas.width,canvas.height);stars.forEach(s=>{s.alpha+=s.speed;if(s.alpha>1||s.alpha<0)s.speed*=-1;ctx.beginPath();ctx.arc(s.x,s.y,s.r,0,Math.PI*2);ctx.fillStyle=`rgba(255,255,255,${s.alpha})`;ctx.fill();});requestAnimationFrame(drawStars);}
drawStars();

function spawnConfetti(){const emojis=['🎉','✨','💖','🌸','💕','🎊','⭐','🥹'];for(let i=0;i<40;i++){const el=document.createElement('div');el.className='confetti-piece';el.textContent=emojis[Math.floor(Math.random()*emojis.length)];el.style.left=Math.random()*100+'vw';el.style.animationDuration=(Math.random()*2+1.5)+'s';el.style.animationDelay=Math.random()*1+'s';document.body.appendChild(el);setTimeout(()=>el.remove(),4000);}}

function openGift(){
  const lid=document.getElementById('giftLid');
  lid.style.transform='translateY(-80px) rotate(-15deg)';
  lid.style.opacity='0';
  setTimeout(()=>{
    document.getElementById('giftScreen').classList.add('hidden');
    document.getElementById('envelopeScreen').classList.remove('hidden');
  },700);
}

function openEnvelope(){
  document.getElementById('envFlap').classList.add('open');
  spawnConfetti();
  setTimeout(()=>{
    document.getElementById('envelopeScreen').classList.add('hidden');
    document.getElementById('contentScreen').classList.remove('hidden');
    initSwipe();
    initScrollReveal();
    setTimeout(()=>{
      const h=document.getElementById('swipeHint');
      if(h){h.style.opacity='0';}
    },3000);
  },1300);
}

let currentPage=0;
const totalPages=5;

function goToPage(n){
  currentPage=Math.max(0,Math.min(totalPages-1,n));
  const pc=document.getElementById('pagesContainer');
  pc.style.transition='transform 0.45s cubic-bezier(0.4,0,0.2,1)';
  pc.style.transform=`translateX(${currentPage*-100}vw)`;
}

function initSwipe(){
  const pc=document.getElementById('pagesContainer');
  const cs=document.getElementById('contentScreen');
  let touchStartX=0,touchStartY=0,lockAxis=null,isDragging=false,startTranslate=0;

  cs.addEventListener('touchstart',(e)=>{
    touchStartX=e.touches[0].clientX;
    touchStartY=e.touches[0].clientY;
    isDragging=true;
    lockAxis=null;
    startTranslate=currentPage*-100;
    pc.style.transition='none';
  },{passive:true});

  cs.addEventListener('touchmove',(e)=>{
    if(!isDragging)return;
    const dx=e.touches[0].clientX-touchStartX;
    const dy=e.touches[0].clientY-touchStartY;

    if(!lockAxis){
      if(Math.abs(dx)>Math.abs(dy)) lockAxis='x';
      else lockAxis='y';
    }

    if(lockAxis==='y') return; // let page scroll vertically

    e.preventDefault(); // block scroll only when swiping horizontally
    const newX=startTranslate+(dx/window.innerWidth*100);
    pc.style.transform=`translateX(${newX}vw)`;
  },{passive:false});

  cs.addEventListener('touchend',(e)=>{
    if(!isDragging)return;
    isDragging=false;
    if(lockAxis==='y'){
      pc.style.transition='transform 0.45s cubic-bezier(0.4,0,0.2,1)';
      pc.style.transform=`translateX(${currentPage*-100}vw)`;
      return;
    }
    const dx=e.changedTouches[0].clientX-touchStartX;
    if(dx<-60) goToPage(currentPage+1);
    else if(dx>60) goToPage(currentPage-1);
    else goToPage(currentPage);
  },{passive:true});

  // desktop mouse drag
  let mouseDown=false,mouseStartX=0;
  cs.addEventListener('mousedown',(e)=>{mouseDown=true;mouseStartX=e.clientX;startTranslate=currentPage*-100;pc.style.transition='none';});
  cs.addEventListener('mousemove',(e)=>{if(!mouseDown)return;const dx=e.clientX-mouseStartX;pc.style.transform=`translateX(${startTranslate+(dx/window.innerWidth*100)}vw)`;});
  cs.addEventListener('mouseup',(e)=>{if(!mouseDown)return;mouseDown=false;const dx=e.clientX-mouseStartX;if(dx<-60)goToPage(currentPage+1);else if(dx>60)goToPage(currentPage-1);else goToPage(currentPage);});
  cs.addEventListener('mouseleave',()=>{if(!mouseDown)return;mouseDown=false;goToPage(currentPage);});
}

function initScrollReveal(){
  const chapters=document.querySelectorAll('.story-chapter');
  const obs=new IntersectionObserver(entries=>{entries.forEach(e=>{if(e.isIntersecting)e.target.classList.add('visible');});},{threshold:0.1});
  chapters.forEach(c=>obs.observe(c));
}
</script>
</body>
</html>
