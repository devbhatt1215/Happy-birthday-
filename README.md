<!DOCTYPE html><html lang="en"><head>
    <meta charset="UTF-8">
    <title>Ankita ❤️ Dev</title>
    <style>
        body {
            margin: 0;
            font-family: 'Segoe UI', sans-serif;
            background: #000010;
            color: #fff0f5;
            text-align: center;
            position: relative;
            overflow-x: hidden;
        }

        header { padding: 60px 20px; }
        header h1 { font-size: 3rem; margin-bottom: 10px; }
        header p { font-size: 1.2rem; }
        section { padding: 40px 20px; }

        .card {
            background: rgba(255, 255, 255, 0.08);
            max-width: 900px;
            margin: 30px auto;
            padding: 30px;
            border-radius: 20px;
            box-shadow: 0 10px 25px rgba(255,100,150,0.15);
            color: #ffe0ec;
        }

        h2 { color: #ff9ec4; margin-bottom: 20px; }

        .gallery {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 15px;
        }

        .gallery div {
            height: 200px;
            border-radius: 15px;
            background: rgba(255, 150, 180, 0.1);
            display: flex;
            align-items: center;
            justify-content: center;
            color: #ffcce0;
        }

        .video-box { margin-top: 20px; }

        video {
            width: 100%;
            max-width: 700px;
            border-radius: 15px;
            box-shadow: 0 8px 20px rgba(255,100,150,0.3);
        }

        footer { padding: 30px; font-size: 1rem; color: #ffcce0; }

        .heart {
            font-size: 1.5rem;
            animation: beat 1s infinite alternate;
            color: #ff6090;
        }

        @keyframes beat {
            from { transform: scale(1); }
            to { transform: scale(1.2); }
        }

        audio { filter: invert(0.8) hue-rotate(300deg); }

        /* ========== STORY SCROLL ========== */
        .story-book {
            max-width: 700px;
            margin: 0 auto;
            text-align: left;
            padding: 10px 0;
        }

        .story-chapter {
            margin-bottom: 60px;
            opacity: 0;
            transform: translateY(50px);
            transition: opacity 0.8s ease, transform 0.8s ease;
        }

        .story-chapter.visible {
            opacity: 1;
            transform: translateY(0);
        }

        .chapter-title {
            color: #ff9ec4;
            font-size: 1.05rem;
            font-weight: bold;
            margin-bottom: 12px;
            padding-bottom: 8px;
            border-bottom: 1px solid rgba(255,150,180,0.25);
        }

        .chapter-text {
            font-size: 0.95rem;
            line-height: 1.95;
            color: #ffe0ec;
        }

        .story-divider {
            text-align: center;
            color: rgba(255,158,196,0.4);
            font-size: 1.2rem;
            margin: 10px 0 50px;
            letter-spacing: 8px;
        }

        .story-end {
            text-align: center;
            padding: 30px 0 10px;
            opacity: 0;
            transform: translateY(50px);
            transition: opacity 0.8s ease, transform 0.8s ease;
        }

        .story-end.visible {
            opacity: 1;
            transform: translateY(0);
        }
    </style></head><body><canvas id="starCanvas" style="position:fixed; top:0; left:0; z-index:-1;"></canvas><header>
    <h1>Happy Birthday Ankitaa❤️😊</h1>
    <p>God bless you mera bccha. Bhgwan ji aapko Humesha khush rakhe jii.❤️❤️</p>
    <div class="heart">💖</div></header><section>
    <div class="card">
        <h2>Our Song 🎶</h2>
        <audio controls loop>
            <source src="Chaar Kadam - PK 320 Kbps.mp3" type="audio/mpeg">
        </audio>
    </div>

    <!-- STORY SCROLL SECTION -->
    <div class="card">
        <h2>Our Story ❤️😝🧿</h2>

        <div class="story-book">


             <div class="story-chapter">
                <div class="chapter-title">📖 Chapter - 0 - Introduction</div>
                <div class="chapter-text"> "I'll never fall in love, again until I found her ...and i would never fall unless it's I've fallen to ..I lost " ah ...ohh toh tumne mujhe dhud liya ....Toh ab kese dhunda ye sb formality hatate h ...Ye hai meri kahani jha mai mila uss shaks se jo mere liye aage chlke itna khaas hogya ki mene uske liye hrr chiz hasil Krli ( ofc jo mere bss mei tha 🤧).....Toh shuru krte h ..ye baat h uss zamane kiii....oh sorry 😅 ye baat h 2024 ki...I saw a girl..Kya lgta h 😂...Ese describe kri hogi....Nh nh nh 😂Listen ...let's imagine....A school corridor.. usme ek ldki aayi chlke uske baal aadhe brown or aadhe black esa rang jisme koi bhi insan khona chahega ofc mai khoya ... Pr chhodo abhi..Uski aakhe itni pyari..Unn aakho ki itna gehra hona hi khaas tha.....Vo aakhe ager kisi laash ko dekhle toh use zinda krr de vo aakho ne uss vkt mujhe dekha..........Socho mera kya hua hoga yaar 😂, khair ....Aage chlte h......Ab nain naksh ki baat hogyi h toh ab hotho ki trf chlte h..Unn hotho ka rang gulabi jese khud gulab ne vha se janam liya ho jese unhe hi dekh ke bhgwan ne vo rang bnaya ho.....Unn hotho se jo shbd nikle maano jese humare kaano ke liye koi geet Unka Hnji or ji  hi hume itna pyara lgta tha jese bss vo bolti jaaye or hum sunte rheAb agrr niche aaye toh ab sharir ki baat krte h..Unnka chal chalan toh maano jese laxmi ji mere samne chl rhi ho ek ek kadam sakshat kamal ka phool jese lgta tha....Or agrr hum unke kadmo ki baat krr hi rhe h toh unke pero ki baat hi krr lete h ...unke per toh mano jese vo phool ki trh thy jise agr chu le toh chune vala amar ho jaye unke pero ki ungliyo tb ko phoolo ki pankhudi jesa bnaya tha bhgwan ne...Toh ab aage chlte h ..Farmaish h ki kitab ko chhoti rkhna h toh koshish krte h😂....Ab jese ki mene btaya unki nazron ne hume dekha toh hum toh khone hi thy, b agrr hum kho chuke toh unke toh hone hi thy...Heina......Khair,Kaash vo pll humara hota,Uss vkt sath bss hum dono ka hota,Mgr kismat ka chaha kux or tha,Kisi or ldke ki dakhalandazi nh hoti,Toh aaj vo pll bhi humara hota.........Samaye bit ta gya humare alg hone ka samaye nazdeek tha magar kismat ka chakkar fir ghuma...Unka hello humpe khud aaya,Humari Khushi ka thikana nh tha humne kisiko btana nh tha humne bss baate krni thi or subha tk sona nh tha....Fir jb humara samay aa hi gya toh ab ye majboor kya krta iss aakho ke doobe shaks ne unse khata krr hi di ki kya vo humse mohobbat krne ki khata krenge...........Unka jawab hn aaya or unhone humari zindagi ko bhi apne jesa gulab krr diya ab humari zindagi mei kisi ldki or ldki ka ana hi humare liye bhot bdi khata hogi....Akhir mei sb khata ko hatate hai bhgwan kre aapko bhi ek nh ek din koi axi mahila mile jo aapse bhi mohabbat krne ki khata kre.....</div>
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

            <div class="story-end">
                <div style="font-size: 2.5rem;">❤️</div>
                <br>
                <div style="font-size: 1.4rem; color: #ff9ec4; font-weight: bold;">HAPPY BIRTHDAY MERA BCCHA 😊❤️</div>
                <br>
                <div style="font-size: 0.95rem; color: #ffcce0; line-height: 2;">I Love You Forever & Always 🌌✨</div>


                 <div><img src="717153891_953578660820852_309478251932703800_n.jpg" alt="images" width="270" height="400"></div>

            </div>

        </div>
    </div>

    <div class="card">
        <h2>Our Memories 📸</h2>
        <h3>we can't meet regulary because of our long distance, so we generate AI image to show our connection❤️😝..</h3>
        <div class="gallery">
            <div><img src="5fac86a7-be7c-41c5-b575-1e88a6ddbd8f.jpg" alt="images" width="270" height="200"></div>
            <div><img src="94861747-1b1a-4083-9149-ced39cdbd7d0.jpg" alt="images" width="271" height="200"></div>
            <div><img src="WhatsApp Image 2026-01-27 at 10.38.11 PM.jpeg" alt="images" width="235" height="200"></div>
            <div><img src="WhatsApp Image 2026-01-27 at 10.38.10 PM.jpeg" alt="images" width="230" height="200"></div>
        </div>

        <h2>Our Memories 📸</h2>
        <h3>Our Ghibli trend..HEHE 😝❤️..</h3>
        <div class="gallery">
            <div><img src="05530801-5f3e-4c44-9c79-61f911585351.jpg" alt="images" width="300" height="200"></div>
            <div><img src="09bfac91-ac9d-4ea2-aa02-ab90373788c7.jpg" alt="images" width="300" height="200"></div>
            <div><img src="5d935f2e-a6a2-44d8-9f5c-e13ba2f76450.jpg" alt="images" width="300" height="200"></div>
            <div><img src="da69fff3-7e60-4308-8b1f-0f29c26a2ef8.jpg" alt="images" width="300" height="200"></div>
            <div><img src="7ba50ddd-6564-44b3-8c7a-dd822e3c5d30.jpg" alt="images" width="300" height="200"></div>
        </div>

        <h2>Our Memories 📸</h2>
        <h3>The special moments and memories we share together🥹❤️🧿..</h3>
        <div class="gallery">
            <div><img src="5faa31b2-5c74-4f6c-a53a-16dcbb4cd73d.jpg" alt="images" width="300" height="200"></div>
            <div><img src="8fc396d4-3958-49d6-8d2b-71af2dc01cdd.jpg" alt="images" width="300" height="200"></div>
            <div><img src="e34b387f-731f-40f1-a7ef-4065f50fe0c9.jpg" alt="images" width="300" height="200"></div>
            <div><img src="f6bd4f61-79b3-40e8-8212-39a1778eaa27.jpg" alt="images" width="300" height="200"></div>
            <div><img src="e32a8f28-a65d-46f9-8401-53665bd17f93.jpg" alt="images" width="300" height="215"></div>
        </div>

        <div class="card">
            <h2>Our Memories 📸</h2>
            <div class="gallery">
                <h3>The first love letter you gave me ❤️😝..</h3>
                <div><img src="7c8d548c-2fbd-43d4-9eb2-7b71c42dd1e0.jpg" alt="images" width="300" height="200"></div>
                <h3>The gift you made for me on my birthday (15 december,2025)❤️..</h3>
                <div><img src="a3240363-9fd3-4d26-b216-f952f3c0fcd2.jpg" alt="images" width="300" height="200"></div>
            </div>

            <h2>flowers 📸</h2>
            <div class="gallery">
                <div><img src="b109e79d-57c0-40b7-bfc7-76858df225d6.jpg" alt="images" width="270" height="200"></div>
                <h3>The flowers I give to her, on our first meeting ❤️😝..</h3>
            </div>

            <h2>Gifts 📸</h2>
            <h3>The gifts i give to her, on her birthday (20th june, 2025)❤️😝..</h3>
            <div class="gallery">
                <div><img src="1cfe8034-ef8f-45f4-9455-e96cb182c290.jpg" alt="images" width="250" height="200"></div>
            </div>
        </div>
    </div>

    <div class="card">
        <h2>Our Special Videos 🎥</h2>
        <div class="video-box">
            <video controls><source src="WhatsApp Video 2026-01-27 at 10.38.20 PM.mp4" type="video/mp4"></video>
        </div>
        <div class="video-box">
            <video controls><source src="WhatsApp Video 2026-01-27 at 10.38.25 PM.mp4" type="video/mp4"></video>
        </div>
        <div class="video-box">
            <video controls><source src="WhatsApp Video 2026-01-27 at 10.38.40 PM (1).mp4" type="video/mp4"></video>
        </div>
        <div class="video-box">
            <video controls><source src="WhatsApp Video 2026-01-27 at 10.38.41 PM.mp4" type="video/mp4"></video>
        </div>
        <div class="video-box">
            <video controls><source src="WhatsApp Video 2026-01-27 at 10.38.40 PM.mp4" type="video/mp4"></video>
        </div>
        <div class="video-box">
            <video controls><source src="WhatsApp Video 2026-01-27 at 11.39.12 PM.mp4" type="video/mp4"></video>
        </div>
    </div>

    <div class="card">
        <h2>A Message for You 💌</h2>
        <p>
           Thank you Ankita 🥹...aap jo bhi krte ho mere liye meri hrr glti ko maaf krr dete ho ..
           mai fir bhi krta hu aap tb bhi maaf krr dete ho ..jyada pareshan krta hu aap vo bhi seh lete ho 🥲🥹
           aap mera dhyan bhi rkhte ho khud ke baare mei nhi sochte 🥹
           or abhi aap dur ho tb itna saath dete ho..
            jb paas rhoge tb toh aap kitna rkhoge bta nhi skta 😭🥹
            toh uss sb ke liye thank you so much Ankita jii ❤️🥹....
             I'll promise you ki mai aapse hi shaadi krunga 🥹....
             and you'll not gonna regret your decision to have relationship with me 🥹❤️
            I'll love you forever Ankita jii 🥹❤️
            Mujhe pta h ki Kbhi kbhi mai aapko irritate krta hu 🥹, kbhi kbhi hurt krta hu 🥲
            or kbhi kbhi mai overreact bhi krr deta hu 🫠,
            but ankita 🥹❤️
            ye sb kiuki mai aapke sath comfortable feel krta hu 🫠❤️
            you complete me ankita 🥹❤️ aapke aane ke baad mai complete hua hu 🫠❤️....
            isliye I love you Ankita 🧿🫠❤️ please merko kbhi chhod ke mtt jana jii 🫠❤️
        </p>
    </div></section><footer>
    Made with ❤️ by Dev for Ankita <br>
    Forever & Always ✨</footer><script>// ===== STAR BACKGROUND =====const canvas = document.getElementById('starCanvas');const ctx = canvas.getContext('2d');function resize() {
    canvas.width = window.innerWidth;
    canvas.height = document.body.scrollHeight;}resize();const stars = Array.from({length: 300}, () => ({
    x: Math.random() * canvas.width,
    y: Math.random() * canvas.height,
    r: Math.random() * 2 + 0.5,
    alpha: Math.random(),
    speed: Math.random() * 0.015 + 0.003}));function drawStars() {
    ctx.clearRect(0, 0, canvas.width, canvas.height);
    ctx.fillStyle = '#000010';
    ctx.fillRect(0, 0, canvas.width, canvas.height);
    stars.forEach(s => {
        s.alpha += s.speed;
        if (s.alpha > 1 || s.alpha < 0) s.speed *= -1;
        ctx.beginPath();
        ctx.arc(s.x, s.y, s.r, 0, Math.PI * 2);
        ctx.fillStyle = `rgba(255,255,255,${s.alpha})`;
        ctx.fill();
    });
    requestAnimationFrame(drawStars);}drawStars();window.addEventListener('resize', () => {
    resize();
    stars.forEach(s => {
        s.x = Math.random() * canvas.width;
        s.y = Math.random() * canvas.height;
    });});// ===== SCROLL REVEAL =====const chapters = document.querySelectorAll('.story-chapter, .story-end');const observer = new IntersectionObserver((entries) => {
    entries.forEach(entry => {
        if (entry.isIntersecting) {
            entry.target.classList.add('visible');
        }
    });}, { threshold: 0.15 });chapters.forEach(chapter => observer.observe(chapter));</script></body></html>
