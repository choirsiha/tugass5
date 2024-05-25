<template>
  <div class="q-pa-md">
    <q-carousel
      animated
      v-model="slide"
      arrows
      navigation
      infinite
    >
      <q-carousel-slide :name="1" img-src="/images/gambar4.jpg" />
      <q-carousel-slide :name="2" img-src="/images/gambar5.jpg" />
      <q-carousel-slide :name="3" img-src="/images/gambar6.jpg" />
      <q-carousel-slide :name="4" img-src="/images/gambar7.jpg" />
    </q-carousel>
  </div>
  <div class="landing-page">
    <nav>
      <ul>
        <li><a href="#home">Home</a></li>
        <li><a href="#produk">Produk</a></li>
        <li><a href="#about">About</a></li>
      </ul>
    </nav>
    
    <header>
      <h1>Salima Karya</h1>
      <p>Toko Online Pilihan Anda</p>
    </header>
    
    <section class="featured-products" id="produk">
      <h2>Produk Unggulan</h2>
      <div class="product">
        <img src="/images/gambar1.jpg" alt="Gorengan">
        <h3>Gorengan</h3>
        <p>makan banyak minyak</p>
      </div>
      <div class="product">
        <img src="/images/gambar2.jpg" alt="Udang Bakar">
        <h3>Udang Bakar</h3>
        <p>di ambil lansung dari laut asli</p>
      </div>
      <div class="product">
        <img src="/images/gambar3.jpg" alt="Kerang Laut">
        <h3>Kerang Laut</h3>
        <p>terdapat banyak protein</p>
      </div>
    </section>
    
    <section class="about-us" id="about">
      <h2>Tentang Kami</h2>
      <p>Salima Karya adalah toko online yang menyediakan berbagai macam produk berkualitas dengan harga terjangkau. Kami berkomitmen untuk memberikan layanan terbaik kepada pelanggan kami.</p>
    </section>
    <div class="q-pa-md">
    <q-card class="my-card">
    <q-video src="https://www.youtube.com/embed/go8iyVrehGw?rel=0" />

      <q-card-section>
        <div class="text-h6">Merpati Band - Buka Puasa (Official Music Video NAGASWARA)</div>
        <div class="text-subtitle2">Merpati band</div>
      </q-card-section>

      <q-card-section class="q-pt-none">
        “Jadi lagu ‘Buka Puasa’ ini terinspirasi dari keseharian suasana di bulan puasa, mulai dari niat puasa, makan sahur, seharian menahan lapar, haus, menjaga emosi, dan menjelang magrib kita ngabuburit, pas buka puasanya dengan membaca doa buka puasa, setelah itu sholat tarawih, tadarusan alquran, dan ibadah ibadah-ibadah lainnyalah, termasuk sholat lima waktu jangan sampai ketinggalan. “Jelas Andi.
      </q-card-section>
    </q-card>
  </div>
    <footer>
      <p>&copy; RAJA @All rights reserved.</p>
    </footer>
  </div>
</template>

<script>
import { ref } from 'vue'

export default {
  setup () {
    return {
      slide: ref(1)
    }
  }
}
</script>

<style scoped>
/* Gaya CSS */
.landing-page {
  font-family: Arial, sans-serif;
  max-width: 1200px;
  margin: 0 auto;
  padding: 20px;
  text-align: center;
}

nav {
  background-color: #333;
  color: #fff;
  padding: 10px 20px;
}

nav ul {
  list-style-type: none;
  padding: 0;
}

nav ul li {
  display: inline;
  margin-right: 20px;
}

nav ul li a {
  color: #fff;
  text-decoration: none;
}

nav ul li a:hover {
  text-decoration: underline;
}

header {
  background-color: #fff;
  padding: 20px;
  border-bottom: 1px solid #ddd;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
}

header h1 {
  font-size: 36px;
  color: #333;
}

header p {
  font-size: 18px;
  color: #666;
  margin-bottom: 30px;
}

.featured-products {
  margin-bottom: 50px;
}

.featured-products h2 {
  font-size: 24px;
  color: #333;
  margin-bottom: 20px;
}

.product {
  background-color: #fff;
  border-radius: 8px;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
  transition: transform 0.3s ease-in-out;
  display: inline-block;
  margin: 0 20px;
  text-align: center;
}

.product:hover {
  transform: translateY(-5px);
}

.product img {
  width: 150px;
  height: 150px;
  border-radius: 50%;
  margin-bottom: 10px;
}

.product h3 {
  font-size: 20px;
  color: #333;
}

.product p {
  color: #666;
}

.about-us {
  background-color: #f9f9f9;
  padding: 30px 20px;
  border-radius: 8px;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
  margin-bottom: 50px;
}

.about-us h2 {
  font-size: 24px;
  color: #333;
  margin-bottom: 20px;
}

.my-card {
  width: 100%;
  max-width: 300px;
}

footer {
  background-color: #333;
  color: #fff;
  padding: 30px 20px;
  font-size: 16px;
}
</style>
