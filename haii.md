# HAII-CANTIIKK
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>I LOVE YOU</title>
    <style>
        body {
            background-image: url('https://images.unsplash.com/photo-1518709268805-4e9042af2176?ixlib=rb-4.0.3&auto=format&fit=crop&w=1000&q=80'); /* Gambar background romantis (hati dan bunga) */
            background-size: cover;
            background-position: center;
            font-family: Arial, sans-serif;
            text-align: center;
            overflow: hidden;
            position: relative;
            height: 100vh;
        }
        h1 {
            font-size: 4em;
            color: white;
            text-shadow: 2px 2px 4px rgba(0,0,0,0.5);
            margin-top: 10%;
        }
        img {
            max-width: 300px;
            height: auto;
            border-radius: 10px;
            margin-top: 20px;
            box-shadow: 0 4px 8px rgba(0,0,0,0.3);
        }
        .heart {
            position: absolute;
            font-size: 2em;
            color: red;
            animation: fall 5s linear infinite;
        }
        @keyframes fall {
            0% { top: -10%; left: 50%; }
            100% { top: 100%; left: calc(50% + 100px); }
        }
        iframe {
            margin-top: 20px;
            border: none;
        }
    </style>
</head>
<body>
    <h1>I LOVEEE YOUUUU</h1>
    <!-- Foto tambahan: Gambar pasangan romantis -->
    <img src="https://images.unsplash.com/photo-1521737604893-d14cc237f11d?ixlib=rb-4.0.3&auto=format&fit=crop&w=400&q=80" alt="Romantic couple">
    
    <!-- Embed YouTube untuk lagu romantis "Perfect" oleh Ed Sheeran -->
    <iframe width="560" height="315" src="https://www.youtube.com/embed/2Vv-BfVoq4g?autoplay=1&loop=1&playlist=2Vv-BfVoq4g" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
    
    <script>
        // Script untuk membuat hati jatuh secara acak
        function createHeart() {
            const heart = document.createElement('div');
            heart.className = 'heart';
            heart.innerHTML = '❤️';
            heart.style.left = Math.random() * 100 + '%';
            heart.style.animationDuration = (Math.random() * 3 + 2) + 's';
            document.body.appendChild(heart);
            setTimeout(() => {
                heart.remove();
            }, 5000);
        }
        setInterval(createHeart, 500); // Buat hati baru setiap 0.5 detik
    </script>
</body>
</html>
