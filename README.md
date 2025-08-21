<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>ZOYA PAYMENT</title>
  <style>
    @import url('https://fonts.googleapis.com/css2?family=Share+Tech+Mono&display=swap');

    body {
      margin: 0;
      padding: 30px 15px;
      font-family: 'Share Tech Mono', monospace;
      background: #000;
      color: #00ff99;
      display: flex;
      flex-direction: column;
      align-items: center;
      min-height: 100vh;
      background-image: linear-gradient(to bottom, #000000, #001a00);
      animation: matrixScroll 30s linear infinite;
    }

    @keyframes matrixScroll {
      from { background-position: 0 0; }
      to { background-position: 0 1000px; }
    }

    h1 {
      color: #00ffcc;
      text-align: center;
      font-size: 2.5em;
      margin-bottom: 10px;
    }

    .thumbnail {
      width: 160px;
      height: 160px;
      border-radius: 12px;
      box-shadow: 0 0 20px #00ff99;
      margin: 20px 0;
    }

    .section {
      display: flex;
      flex-direction: column;
      gap: 12px;
      width: 100%;
      max-width: 350px;
      margin-bottom: 40px;
    }

    .product-card {
      background: rgba(0, 30, 0, 0.6);
      border: 1px solid #00ff99;
      border-radius: 12px;
      padding: 15px;
      box-shadow: 0 0 15px #004d26;
      cursor: pointer;
      transition: all 0.3s ease;
    }

    .product-card:hover {
      background: rgba(0, 50, 0, 0.7);
      transform: scale(1.03);
    }

    .product-title {
      font-size: 1.1em;
      font-weight: bold;
      color: #00ffcc;
    }

    .price {
      font-size: 0.95em;
      margin: 6px 0;
      color: #66ffcc;
    }

    .product-detail {
      display: none;
      margin-top: 8px;
      font-size: 0.85em;
      color: #99ffcc;
      white-space: pre-line;
    }

    button {
      background-color: #00ff99;
      color: black;
      border: none;
      padding: 10px;
      border-radius: 8px;
      font-weight: bold;
      font-family: inherit;
      box-shadow: 0 0 10px #00ff99;
      cursor: pointer;
      transition: all 0.2s ease-in-out;
    }

    button:hover {
      transform: scale(1.05);
    }

    hr {
      width: 80%;
      border: none;
      height: 1px;
      background-color: #004400;
      margin: 30px 0;
    }

    .note {
      color: #ccc;
      font-size: 0.9em;
      text-align: center;
    }
  </style>
</head>
<body>

  <h1>Zoya Payment</h1>
  <img src="https://files.catbox.moe/4ujxca.jpg" class="thumbnail" />

  <!-- QRIS & DUKUNGAN -->
  <div class="section">
    <button onclick="window.open('https://files.catbox.moe/genea2.jpg', '_blank')">QRIS</button>
    <button onclick="event.preventDefault()">DANA: 082138040496</button>
    <button onclick="event.preventDefault()">GOPAY: 082138040496</button>
  </div>
  <div class="note">Atas Nama: <strong>Muhammad Fadhil Ardiansyah </strong></div>

  <hr />

  <!-- Produk Section -->
  <div class="section">

    <div class="product-card" onclick="toggleDetail(this)">
      <div class="product-title">Telegram Premium</div>
      <div class="price">Mulai Rp57.000</div>
      <div class="product-detail">
      </div>
    </div>

    <div class="product-card" onclick="toggleDetail(this)">
      <div class="product-title">Sc Shiroy</div>
      <div class="price">Rp100.000</div>
      <div class="product-detail">
Benefit:
- Get Akses Reseller
- Bisa jual no up dan Full up
- bisa add token sendiri
      </div>
    </div>

    <div class="product-card" onclick="toggleDetail(this)">
      <div class="product-title">Sc Destroyed</div>
      <div class="price">Rp100.000</div>
      <div class="product-detail">
Bot Telegram Bug WhatsApp Destroyed
Dengan Sistem Perlindungan Bypass & Fitur Licenser
      </div>
    </div>

    <div class="product-card" onclick="toggleDetail(this)">
      <div class="product-title">Sc Xmd invasionCode</div>
      <div class="price">Rp50.000</div>
      <div class="product-detail">
Get full up script
      </div>
    </div>

  </div>

  <script>
    function toggleDetail(card) {
      const detail = card.querySelector('.product-detail');
      detail.style.display = detail.style.display === 'block' ? 'none' : 'block';
    }
  </script>

</body>
</html>
