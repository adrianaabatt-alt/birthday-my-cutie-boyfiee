# birthday-my-cutie-boyfiee
# birthday baby sayang
<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Happy Birthday Baby Sayang! 💝</title>
    <style>
        body {
            font-family: 'Arial', sans-serif;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            text-align: center;
            color: white;
            padding: 50px;
        }
        
        .card {
            background: rgba(255, 255, 255, 0.1);
            backdrop-filter: blur(10px);
            border-radius: 20px;
            padding: 40px;
            max-width: 600px;
            margin: 0 auto;
            box-shadow: 0 8px 32px rgba(0, 0, 0, 0.3);
        }
        
        h1 {
            font-size: 3em;
            margin-bottom: 20px;
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.3);
        }
        
        .message {
            font-size: 1.2em;
            line-height: 1.6;
            margin: 20px 0;
        }
        
        .hearts {
            font-size: 2em;
            margin: 20px 0;
        }
        
        button {
            background: #ff6b6b;
            color: white;
            border: none;
            padding: 15px 30px;
            font-size: 1.1em;
            border-radius: 50px;
            cursor: pointer;
            margin: 10px;
            transition: transform 0.3s;
        }
        
        button:hover {
            transform: scale(1.1);
        }
        
        .hidden-message {
            display: none;
            margin-top: 20px;
            padding: 20px;
            background: rgba(255, 255, 255, 0.2);
            border-radius: 10px;
        }
    </style>
</head>
<body>
    <div class="card">
        <div class="hearts">💖🎂🎉</div>
        <h1>Happy Birthday To My favorite personn🎂</h1>
        
        <div class="message">
            <p>Selamat ulang tahun yang ke -<span id="age">16</span> tahun!</p>
            <p>Happy Birthday My Handsome Boyy!, hari ini hari yang special kan bagi babyy sayang, btw kan baby tau takk sejak baby ada dalam hidup sayang, sayang lagi happy tauu sayang rasa disayangi,dihargai, sayang rasa sayang dah selesa sangat sangat dengan baby hihi sayang tatau la mcm mne nak cakap lagi tapi sayang memang tanak hilang baby. walau macam mana pon sayang tetap akan pilih baby .</p>
            <p>Sayang doakan semoga babyy sentiasa sihat ,dikurniakan rezeki yang berpanjangan, dapat banggakan ibu dan ayah dan juga berjaya di dunia dan akhiratt.</p>
        </div>
        
        <div class="hearts">💝🎁✨</div>
        
        <button onclick="showMessage()">Klik sini baby! 💌</button>
        
        <div id="specialMessage" class="hidden-message">
            <h3>Untuk Baby Sayangg🤍</h3>
            <p>baby mesti da tahu kan yang baby tk sama langsung dengan lelaki lain, baby baik dengan sayang, and baby tk penah marah sayang lepastu kalau sayang ada silap baby mesti tegur baik baik, baby tak penah gagal untuk buat sayang senyum ,buat sayang rasa bahagia,sayang tak pernah dapat macam ni dari orang lain. baby selalu layan perangai sayang dan baby yang selalu ada bila sayang ada masalah. baby je tempat yang paling selesa untuk sayang meluah. kehadiran baby dalam hidup sayang memang buat hidup sayang berubah ,berubah banyak sangat. sayang takkan tinggalkan baby dan sayang nk tepati janji sayang untuk jaga baby , sayang nak ada dengan baby sentiasa,sayang nak ada time baby nges,sayang nak peluk baby kalau baby ada masalah,sayang nak lap air mata baby kalau baby menanges,sayang nak jaga baby macam mana ibu jaga baby. sayang sayang sangat dengan baby dan sayang harap relay kita boleh bertahan lama.</p>
            <p>Sayanng bersyukur sangat sebab baby ada dalam hidup sayang,</p>
        </div>
    </div>

    <script>
        function showMessage() {
            const message = document.getElementById('specialMessage');
            message.style.display = 'block';
            
            // Tambah efek confetti
            createHearts();
        }
        
        function createHearts() {
            for (let i = 0; i < 20; i++) {
                setTimeout(() => {
                    const heart = document.createElement('div');
                    heart.innerHTML = '💖';
                    heart.style.position = 'fixed';
                    heart.style.left = Math.random() * 100 + 'vw';
                    heart.style.top = '-50px';
                    heart.style.fontSize = (Math.random() * 20 + 10) + 'px';
                    heart.style.animation = `fall ${Math.random() * 3 + 2}s linear forwards`;
                    
                    document.body.appendChild(heart);
                    
                    // Hapus heart setelah animasi selesai
                    setTimeout(() => {
                        heart.remove();
                    }, 5000);
                }, i * 200);
            }
        }
        
        // Tambah style untuk animasi jatuh
        const style = document.createElement('style');
        style.innerHTML = `
            @keyframes fall {
                to {
                    transform: translateY(100vh) rotate(360deg);
                    opacity: 0;
                }
            }
        `;
        document.head.appendChild(style);
    </script>
</body>
</html>
