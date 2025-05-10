# Kenangan-
<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8">
  <title>Perpisahan Sahabat Kerja</title>
  <style>
    body {
      background-color: #f0f4f8;
      font-family: 'Segoe UI', sans-serif;
      color: #333;
      text-align: center;
      padding: 50px;
    }
    .container {
      background: white;
      border-radius: 15px;
      padding: 30px;
      max-width: 600px;
      margin: auto;
      box-shadow: 0 8px 20px rgba(0, 0, 0, 0.15);
    }
    h1 {
      color: #2c3e50;
    }
    p {
      font-size: 18px;
      line-height: 1.7;
      margin: 20px 0;
    }
    .footer {
      margin-top: 30px;
      font-style: italic;
      color: #7f8c8d;
    }
    button {
      background-color: #2c3e50;
      color: white;
      border: none;
      padding: 10px 20px;
      border-radius: 5px;
      cursor: pointer;
      font-size: 16px;
    }
    button:hover {
      background-color: #34495e;
    }
  </style>
</head>
<body>

  <div class="container">
    <h1>Selamat Jalan, Sahabat</h1>
    <p>
      Di antara tawa yang kini tinggal kenangan,<br>
      Ada sejumput haru yang enggan hilang.<br>
      Waktu berjalan, dan kini kau melangkah,<br>
      Meninggalkan jejak dalam cerita kita.
    </p>
    <p>
      Terima kasih atas setiap hari yang kita bagi,<br>
      Untuk kerja sama, semangat, dan empati.<br>
      Semoga langkahmu selalu ringan,<br>
      Di mana pun kau berada, tetaplah bersinar terang.
    </p>
    <p>
      Perpisahan ini bukan akhir dari segalanya,<br>
      Tapi awal dari cerita baru dalam hidupmu.<br>
      Sampai jumpa lagi, di lain waktu dan kesempatan.
    </p>
    <div class="footer">
      - Dari kami yang akan selalu merindukanmu
    </div>
    <br><br>
    <button onclick="window.location.href='mailto:rekan@kerja.com'">Kirim Pesan</button>
  </div>

</body>
</html>
<!-- Musik Latar -->
<audio autoplay loop>
  <source src="musik-latar.mp3" type="audio/mpeg">
  Browser Anda tidak mendukung audio.
</audio>

<!-- Slideshow Foto -->
<div class="slideshow">
  <img src="foto1.jpg" class="slide-image active" alt="Kenangan 1">
  <img src="foto2.jpg" class="slide-image" alt="Kenangan 2">
  <img src="foto3.jpg" class="slide-image" alt="Kenangan 3">
</div>
.slideshow {
  position: relative;
  max-width: 100%;
  height: 400px;
  margin: 20px 0;
}
.slide-image {
  width: 100%;
  height: 100%;
  object-fit: cover;
  border-radius: 10px;
  box-shadow: 0 4px 10px rgba(0,0,0,0.1);
  position: absolute;
  opacity: 0;
  transition: opacity 1s ease-in-out;
}
.slide-image.active {
  opacity: 1;
  z-index: 1;
}
<script>
  // Script slideshow
  let currentSlide = 0;
  const slides = document.querySelectorAll('.slide-image');

  setInterval(() => {
    slides[currentSlide].classList.remove('active');
    currentSlide = (currentSlide + 1) % slides.length;
    slides[currentSlide].classList.add('active');
  }, 3000); // Ganti slide setiap 3 detik
</script>
