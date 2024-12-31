<template>
  <div>
    <!-- Header -->
    <header class="header">
      <h1>Galeri Web Sekolah</h1>
      <p>Menampilkan dokumentasi kegiatan sekolah kami</p>
    </header>

    <!-- Main Gallery Section -->
    <main>
      <section class="gallery">
        <div v-for="(image, index) in images" :key="index" class="gallery-item">
          <a :href="image.src" target="_blank">
            <img :src="image.src" :alt="image.alt" />
          </a>
          <p>{{ image.title }}</p>
        </div>
      </section>
    </main>

    <!-- Footer -->
    <footer class="footer">
      <p>&copy; 2024 Sekolah Kita. Semua Hak Dilindungi.</p>
    </footer>
  </div>
</template>

<script>
export default {
  data() {
    return {
      images: [
        {
          src: "/img/kegiatan1.jpg",
          title: "Upacara Bendera",
          alt: "Upacara Bendera",
        },
        {
          src: "/img/kegiatan2.jpg",
          title: "Ekskul Tari Tradisional",
          alt: "Ekskul Tari Tradisional",
        },
        {
          src: "/img/kegiatan3.jpg",
          title: "Lomba Sains",
          alt: "Lomba Sains",
        },
        {
          src: "/img/kegiatan4.jpg",
          title: "Kegiatan Olahraga",
          alt: "Kegiatan Olahraga",
        },
      ],
    };
  },
};
</script>

<style>
/* Header Styles */
.header {
  text-align: center;
  background: #0275d8;
  color: white;
  padding: 20px 0;
}

.header h1 {
  margin: 0;
  font-size: 2.5rem;
}

.header p {
  margin: 10px 0 0;
  font-size: 1.2rem;
}

/* Gallery Styles */
.gallery {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
  gap: 20px;
  padding: 20px;
}

.gallery-item {
  text-align: center;
}

.gallery-item img {
  width: 100%;
  height: auto;
  border-radius: 5px;
  box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
  transition: transform 0.3s ease;
}

.gallery-item img:hover {
  transform: scale(1.05);
}

.gallery-item p {
  margin-top: 10px;
  font-size: 1rem;
  color: #555;
}

/* Footer Styles */
.footer {
  text-align: center;
  background: #333;
  color: white;
  padding: 10px 0;
  margin-top: 20px;
}
</style>
