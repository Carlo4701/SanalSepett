# SanalSepett
Sende Ucuza Satın Al
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>SanalSepet</title>
    <style>
        /* Genel sayfa stilini ayarla */
        body {
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
            background: linear-gradient(135deg, #ffddc1, #ffd5e5, #f6c1ff, #d0c1ff);
            font-family: Arial, sans-serif;
            overflow: hidden;
        }

        /* Başlık stilini ayarla */
        h1 {
            font-size: 80px;
            font-weight: bold;
            background: linear-gradient(90deg, #ff6347, #ffd700, #40e0d0, #ff69b4, #ba55d3);
            -webkit-background-clip: text;
            color: transparent;
            animation: colorChange 5s infinite;
            margin-bottom: 20px;
        }

        /* Renk geçişi animasyonu */
        @keyframes colorChange {
            0% { color: #ff6347; }
            20% { color: #ffd700; }
            40% { color: #40e0d0; }
            60% { color: #ff69b4; }
            80% { color: #ba55d3; }
            100% { color: #ff6347; }
        }

        /* Giriş butonu stili */
        .login-button {
            font-size: 24px;
            padding: 15px 30px;
            border: none;
            border-radius: 8px;
            background-color: #ff69b4;
            color: white;
            cursor: pointer;
            transition: background-color 0.3s;
            text-decoration: none;
            margin-top: 20px;
        }

        .login-button:hover {
            background-color: #ff6347;
        }

        /* Satış sayfası stilini gizle */
        .products {
            display: none;
            text-align: center;
            margin-top: 30px;
        }

        /* Satış linkleri için büyük buton stili */
        .product-link {
            display: inline-block;
            font-size: 24px;
            padding: 20px 40px;
            background-color: #ff4500;
            color: white;
            margin: 15px; /* Butonlar arasındaki boşluğu artır */
            border-radius: 10px;
            text-decoration: none;
            font-weight: bold;
            transition: background-color 0.3s, transform 0.3s;
        }

        .product-link:hover {
            background-color: #ff6347;
            transform: scale(1.1);
        }
    </style>
</head>
<body>
    <h1>SanalSepet</h1>
    
    <!-- Giriş butonu -->
    <a href="#products" class="login-button">Login</a>

    <!-- Ürünler ve Satış Linkleri -->
    <section id="products" class="products">
        <h2>Ürünler</h2>
        <a href="https://example.com/urun1" class="product-link">100 Adet Discord Botu - 80TL Satın Al</a>
        <a href="https://example.com/urun2" class="product-link">100 Adet Instagram Takipçi - 40TL Satın Al</a>
        <a href="https://example.com/urun3" class="product-link">100 Adet Tiktok Takipçi - 70TL Satın Al</a>
    </section>

    <script>
        // Giriş butonuna tıklayınca ürünleri göster
        document.querySelector('.login-button').addEventListener('click', function(event) {
            event.preventDefault();
            document.querySelector('.products').style.display = 'block';
        });
    </script>
</body>
</html>
