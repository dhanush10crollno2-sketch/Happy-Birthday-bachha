<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Happy Birthday Surprise!</title>
    <style>
        body {
            font-family: 'Arial', sans-serif;
            background: linear-gradient(135deg, #ff9a9e, #fecfef, #ffecd2);
            color: #333;
            margin: 0;
            padding: 20px;
            text-align: center;
            overflow-x: hidden;
        }
        h1 {
            font-size: 2.5em;
            color: #ff4081;
            animation: bounce 2s infinite;
        }
        @keyframes bounce {
            0%, 20%, 50%, 80%, 100% { transform: translateY(0); }
            40% { transform: translateY(-10px); }
            60% { transform: translateY(-5px); }
        }
        .confetti {
            position: absolute;
            width: 10px;
            height: 10px;
            background: #ff4081;
            animation: fall 3s linear infinite;
        }
        @keyframes fall {
            to { transform: translateY(100vh); }
        }
        button {
            background: #ff4081;
            color: white;
            border: none;
            padding: 15px 30px;
            font-size: 1.2em;
            border-radius: 25px;
            cursor: pointer;
            margin: 20px;
            transition: background 0.3s;
        }
        button:hover { background: #e91e63; }
        #paragraph {
            display: none;
            background: rgba(255, 255, 255, 0.9);
            padding: 20px;
            border-radius: 15px;
            margin: 20px auto;
            max-width: 90%;
            font-size: 1.1em;
            line-height: 1.6;
            text-align: left;
        }
        #slideshow {
            display: none;
            margin: 20px auto;
            max-width: 90%;
        }
        .slide {
            display: none;
            background: rgba(255, 255, 255, 0.9);
            padding: 20px;
            border-radius: 15px;
            margin: 10px 0;
            animation: fadeIn 1s;
        }
        @keyframes fadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
        }
        #love-note {
            display: none;
            background: rgba(255, 255, 255, 0.9);
            padding: 20px;
            border-radius: 15px;
            margin: 20px auto;
            max-width: 90%;
            font-size: 1.2em;
            color: #ff4081;
            animation: heartPulse 2s infinite;
        }
        @keyframes heartPulse {
            0%, 100% { transform: scale(1); }
            50% { transform: scale(1.1); }
        }
        img {
            max-width: 100%;
            height: auto;
            border-radius: 10px;
        }
    </style>
</head>
<body>
    <h1>Happy Birthday, My Bachaa! 🎉</h1>
    <p>Click below for your first surprise!</p>
    <button onclick="revealParagraph()">Reveal My Message</button>

    <div id="paragraph">
        <h2>A Very Special Birthday Message for You, Darling 💖</h2>
        <p>Happyyyyyy Birthdayyyyy meri pyaari bachiiii😘😚😚😚💗🫂🫂🫶 🥳 Aajj ka din bohot zyada special hai kyunki aaj tera birthday hai, jiska main kitne mahino se wait kar raha tha I know abhi exams hain, toh tu tension mat le, bas padhai kar. Hum next year tera birthday aur bhi zyada dhoomdhaam se manayenge! 🥳✨</p>
        
        <p>Mujhe pata hai hum ab roz mil nahi payenge aur mujhe wo hamari masti, wo hugs,kisses, teri kamar pe hath rakhna thighs pe face pe lips pe sab jagha pe hi hath rakhna aur tera milna bohot yaad aayega. 😥 Múje aasa feel hota hai ki tuu sirff merii hii haii mana ki ham door rahege Par main hamesha tere saath hu, darling. Kuch bhi ho jaye, main tujhe kabhi nahi chhodne wala. Mujhe puri life tere saath rehni hai aur bohot kuch experience karna hai. 🫂💗</p>
        
        <p>You know what? Tu meri life ki wo blessing hai jise me har pal celebrate karna chahta hu Har baar jab main tujhe dekhta hu main bas yahi sochta hu ki koi itna Sexyyy aur itna Hot kaise ho sakta hai 🤤🤤Seriously  teri hotness ka koi jawab nahi! 🥵🤤 Mera dil aaj bhi tujhe dekh kar waise hi dhadakta hai jaise pehli baar dhadka tha. 💗</p>
        
        <p>Par meri Jaan, sirf looks hi nahi, tera wo jo bachpana hai na, wo mujhe sabse zyada pasand hai. 😚🥰 Jab tu ek chhoti si bachi ban kar mujhse ladti hai ya pyaar karti hai, mera dil karta hai tujhe duniya se chhupa kar apne seene se laga lu🙈🫂 Tu meri sabse pyaari Cutie hai main duniya ka sabse khushnaseeb insaan huu kyunki mere paas tu hai🫶🧿✨</p>
        
        <p>I promise main hamesha teri side khada rahunga. Tu mera sukoon hai, meri himmat hai, aur meri sabse badi khushi. ❤️‍🩹 Hum dher saari memories banayenge aur budhape tak ek doosre ka haath aise hi thame rakhenge Tu jaisi hai mere liye bilkul perfect hai merii soulmate hai tuu😚🫶💍</p>
        
        <p>I loveeeeeeeeeeee youhhhhhhhhhhhhh infiniteeeeeeee bachaaa 😚😘🥰🫂💗</p>
        
        <p>Kuchh liness tere liye darling</p>
        <p>Mana ki kitabein abhi tere haath mein hain,</p>
        <p>Par dekh, mera dil har pal tere saath mein hai. 📖❤️</p>
        <p>Exam ki tension ko thoda door kar de,</p>
        <p>Apni smile se mera din thoda aur noor kar de. 😊✨</p>
        <p>Padh le abhi, phir saath mein sukoon payenge,</p>
        <p>Agla birthday hum sabse yaadgaar banayenge! 🎂🎉</p>
        <p>All the best, my Jaan! You’ve got this! 😚😘💪"</p>
        <p>Happiest Birthday once again Babyyyyy Enjoy your day 🎉😍🤭</p>
    </div>

    <button onclick="revealSlideshow()" style="display:none;" id="nextBtn">Next Surprise: Virtual Gifts!</button>

    <div id="slideshow">
        <div class="slide" id="slide1">
            <h3>Surprise 1: A Virtual Rose Bouquet for My Baby 🌹</h3>
            <img src="https://tse2.mm.bing.net/th/id/OIP.AeioLDwQ_1hL9TthbzmflQHaHa?rs=1&pid=ImgDetMain&o=7&rm=3com/300x200/ff4081/ffffff?text=Roses+for+You" alt="Roses">
            <p>Imagine these red roses in your hands – one for each reason I love you, Jaan!</p>
        </div>
       <div class="slide" id="slide2">
    
        <div class="slide" id="slide3">
            <h3>Surprise 2: A Promise Note for My Bachaa 💌</h3>
            <p>I promise to always make you laugh, hold your hand through tough times, and love you endlessly. You're my forever, Baby.
           <P> Dear Riddhi,</P>

<P>In your eyes, I see my forever. Today, I promise to:
</P>
<P>Love you unconditionally, through every high and low</P>
<P>Support your dreams and be your biggest cheerleader.</P>
<P>Communicate openly and honestly, no matter what.</P>
<P>Cherish every moment we share and make new memories together.</P>
<P>Grow with you, learning and evolving as a team.</P>
<P>These aren't just words they're my commitment to you. I choose you every day.</P>

<p>With all my love,</P>
<P>Dhanush</P>
15/02/2026.</p>
        </div>
    </div>

    <button onclick="revealLoveNote()" style="display:none;" id="finalBtn">Final Surprise: A Love Note</button>

    <div id="love-note">
        <h3>💖 My Heart Says to My Jaan... 💖</h3>
        <p>You are the beat in my heart, the light in my life, and the love of my soul. Happy Birthday, my queen! I love you infinitely, Darling. missing you sooo much bachaa ❤️</p>
    </div>

    <script>
        // Confetti effect on load
        for (let i = 0; i < 50; i++) {
            let confetti = document.createElement('div');
            confetti.className = 'confetti';
            confetti.style.left = Math.random() * 100 + 'vw';
            confetti.style.animationDelay = Math.random() * 3 + 's';
            document.body.appendChild(confetti);
        }

        function revealParagraph() {
            document.getElementById('paragraph').style.display = 'block';
            document.getElementById('nextBtn').style.display = 'inline-block';
        }

        function revealSlideshow() {
            document.getElementById('slideshow').style.display = 'block';
            let slides = document.querySelectorAll('.slide');
            slides.forEach((slide, index) => {
                setTimeout(() => { slide.style.display = 'block'; }, index * 2000);
            });
            document.getElementById('finalBtn').style.display = 'inline-block';
        }

        function revealLoveNote() {
            document.getElementById('love-note').style.display = 'block';
        }
    </script>
</body>
</html>
