<h1>HAI, CANTIKK MY MINEE❤️<h1>
<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>HAI CANTIKK,SAYANGGKUU!</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            background: linear-gradient(to bottom, #ffe6f2, #ffb3d9);
            color: #d63384;
            overflow: hidden;
            height: 100vh;
            margin: 0;
        }
        h1 {
            font-size: 3em;
            margin-top: 20%;
            animation: bounce 2s infinite;
        }
        @keyframes bounce {
            0%, 20%, 50%, 80%, 100% { transform: translateY(0); }
            40% { transform: translateY(-10px); }
            60% { transform: translateY(-5px); }
        }
        .heart {
            position: absolute;
            color: #ff69b4;
            font-size: 2em;
            animation: fall 5s linear infinite;
        }
        @keyframes fall {
            0% { top: -10%; opacity: 1; }
            100% { top: 100%; opacity: 0; }
        }
    </style>
</head>
<body>
    <h1>I LOVEEE YOUUUU</h1>
    <p>Buat KAMU, TERSAYANG TERCINTAKU MY LOVE. Klik hati untuk pesan spesial! 💖</p>
    <div id="hearts"></div>

    <script>
        function createHeart() {
            const heart = document.createElement('div');
            heart.className = 'heart';
            heart.innerHTML = '❤️';
            heart.style.left = Math.random() * 100 + 'vw';
            heart.style.animationDuration = (Math.random() * 3 + 2) + 's';
            document.getElementById('hearts').appendChild(heart);
            setTimeout(() => heart.remove(), 5000);
        }
        setInterval(createHeart, 300);
        
        // Klik untuk pesan pop-up
        document.addEventListener('click', () => {
            alert('Aku sayang banget sama kamu muachh! 😘');
        });
    </script>
</body>
</html>
