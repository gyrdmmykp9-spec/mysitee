<!DOCTYPE html>
<html lang="tr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Sadece Bizim İçin ❤️</title>
    <style>
        body {
            background-color: #ffe6e6;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
            margin: 0;
            text-align: center;
        }
        .card {
            background-color: white;
            padding: 30px;
            border-radius: 20px;
            box-shadow: 0 10px 25px rgba(0,0,0,0.1);
            max-width: 450px;
            width: 90%;
            margin: 20px auto;
        }
        h1 { color: #ff4d6d; margin-bottom: 20px; }
        p { color: #555; line-height: 1.6; font-size: 1.1rem; }
        input[type="password"] {
            width: 80%;
            padding: 10px;
            border: 2px solid #ffb3c1;
            border-radius: 10px;
            font-size: 16px;
            outline: none;
            text-align: center;
        }
        button {
            background-color: #ff4d6d;
            color: white;
            border: none;
            padding: 10px 20px;
            border-radius: 10px;
            font-size: 16px;
            cursor: pointer;
            margin-top: 15px;
            transition: 0.3s;
        }
        button:hover { background-color: #ff758f; }
        .hidden-content { display: none; }
        .heart { font-size: 45px; color: #ff4d6d; animation: beat 1s infinite alternate; }
        @keyframes beat { to { transform: scale(1.15); } }
        
        .album {
            display: flex;
            flex-direction: column;
            gap: 15px;
            margin: 20px 0;
        }
        img {
            max-width: 100%;
            border-radius: 15px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
            transition: transform 0.3s;
        }
        img:hover {
            transform: scale(1.03);
        }
    </style>
</head>
<body>

    <div class="card" id="loginCard">
        <div class="heart">🔒❤️</div>
        <h1>Giriş Yap</h1>
        <p>Lütfen sadece bizim bildiğimiz o şifreyi gir sevgilim... 🥰</p>
        <input type="password" id="passwordInput" placeholder="Şifreniz...">
        <br>
        <button onclick="checkPassword()">Giriş Yap</button>
    </div>

    <div class="card hidden-content" id="mainContent">
        <div class="heart">❤️</div>
        
        <h1>Selin & Berk</h1> 

        <p>Hayatımın en güzel detayına... İyi ki varsın, iyi ki hayatımdasın. Bu siteyi tamamen senin için hazırladım. Seni çok seviyorum! 💕</p>
        
        <div class="album">
            <img src="IMG_0085.jpeg" alt="Biz">
            <img src="IMG_3661.jpeg" alt="Biz">
            <img src="IMG_4603.jpeg" alt="Biz">
            <img src="IMG_6567.jpeg" alt="Biz">
            <img src="IMG_7598.jpeg" alt="Biz">
            <img src="IMG_7702.jpeg" alt="Biz">
            <img src="IMG_8024.jpeg" alt="Biz">
            <img src="IMG_8255.jpeg" alt="Biz">
            <img src="IMG_9654.jpeg" alt="Biz">
        </div>

    </div>

    <script>
        function checkPassword() {
            var password = document.getElementById("passwordInput").value;
            if (password.toLowerCase() === "sevgilim") { 
                document.getElementById("loginCard").style.display = "none";
                document.getElementById("mainContent").style.display = "block";
            } else {
                alert("Hatalı şifre! Tekrar dene sevgilim.. 🥺");
            }
        }
    </script>
</body>
</html>
