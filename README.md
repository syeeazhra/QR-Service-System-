<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Warung Mie Ayam & Bakso Mas Joko</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background: #f7f2ea;
      margin: 0;
      color: #2d2d2d;
    }

    .container {
      max-width: 420px;
      margin: auto;
      padding: 20px;
    }

    .header {
      background: #5a3825;
      color: white;
      border-radius: 20px;
      padding: 25px;
      text-align: center;
    }

    .header h1 {
      margin: 0;
      font-size: 32px;
    }

    .card {
      background: white;
      border-radius: 18px;
      padding: 18px;
      margin-top: 20px;
      box-shadow: 0 4px 10px rgba(0,0,0,0.08);
    }

    .menu-item {
      display: flex;
      justify-content: space-between;
      margin: 12px 0;
      border-bottom: 1px solid #eee;
      padding-bottom: 10px;
    }

    button {
      background: #2d6a4f;
      color: white;
      border: none;
      padding: 12px;
      width: 100%;
      border-radius: 12px;
      font-size: 16px;
      margin-top: 15px;
      cursor: pointer;
    }

    .qris {
      text-align: center;
    }

    .fake-qr {
      width: 220px;
      height: 220px;
      margin: auto;
      background:
      linear-gradient(90deg,#000 10%,transparent 10%),
      linear-gradient(#000 10%,transparent 10%);
      background-size: 22px 22px;
      background-color: white;
      border: 12px solid white;
      box-shadow: 0 0 10px rgba(0,0,0,0.2);
    }

    textarea, input {
      width: 100%;
      padding: 12px;
      margin-top: 10px;
      border-radius: 10px;
      border: 1px solid #ccc;
      box-sizing: border-box;
    }

    .footer {
      text-align: center;
      margin-top: 25px;
      color: #666;
      font-size: 14px;
    }
  </style>
</head>
<body>
  <div class="container">

    <div class="header">
      <h1>Warung Mie Ayam & Bakso Mas Joko</h1>
      <p>Scan • Order • Bayar</p>
      <p>WA Order: 0812-3456-7890</p>
    </div>

    <div class="card">
      <h2>Daftar Menu</h2>

      <div class="menu-item">
        <span>Mie Ayam</span>
        <strong>Rp12.000</strong>
      </div>

      <div class="menu-item">
        <span>Bakso</span>
        <strong>Rp13.000</strong>
      </div>

      <div class="menu-item">
        <span>Mie Ayam + Bakso Besar</span>
        <strong>Rp20.000</strong>
      </div>

      <div class="menu-item">
        <span>Mie Ayam + Bakso Kecil</span>
        <strong>Rp15.000</strong>
      </div>

      <div class="menu-item">
        <span>Es Teh Manis</span>
        <strong>Rp4.000</strong>
      </div>

      <button onclick="document.getElementById('popup').style.display='block'">Pesan Sekarang</button>
    
      <div id="popup" style="display:none; position:fixed; top:0; left:0; width:100%; height:100%; background:rgba(0,0,0,0.6);">
        <div style="background:white; max-width:350px; margin:80px auto; padding:20px; border-radius:20px;">
          <h2>Pilih Menu</h2>
          <label><input type='checkbox'> Mie Ayam - Rp12.000</label><br><br>
          <label><input type='checkbox'> Bakso - Rp13.000</label><br><br>
          <label><input type='checkbox'> Mie Ayam + Bakso Besar - Rp20.000</label><br><br>
          <label><input type='checkbox'> Es Teh Manis - Rp4.000</label><br><br>
          <button onclick="alert('Pesanan berhasil dibuat!');">Checkout</button>
          <button onclick="document.getElementById('popup').style.display='none'" style="background:#999; margin-top:10px;">Tutup</button>
        </div>
      </div>
    </div>

    <div class="card qris">
      <h2>Pembayaran QRIS</h2>
      <img src="WhatsApp Image 2026-05-07 at 20.10.39.jpeg" alt="QRIS" style="width:220px;border-radius:20px;box-shadow:0 0 10px rgba(0,0,0,0.2);">
      <p><b>Demo QRIS</b></p>
      <p>Scan untuk simulasi pembayaran</p>
    </div>

    <div class="card">
      <h2>Kritik & Saran</h2>

      <input type="text" placeholder="Nama (opsional)">

      <textarea rows="5" placeholder="Tulis kritik dan saran di sini..."></textarea>

      <button onclick="alert('Terima kasih atas kritik dan sarannya 😊')">Kirim Masukan</button>
    </div>

    <div class="footer">
      Terima kasih sudah berkunjung 🍜
    </div>

  </div>
</body>
</html>
