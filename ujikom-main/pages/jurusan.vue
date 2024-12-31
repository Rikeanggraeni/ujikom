<template>
  <div class="container mt-4">
    <h1 class="text-center mb-4">Jurusan Sekolah</h1>

    <!-- Daftar Jurusan -->
    <section class="row">
      <!-- Jurusan 1: IPA -->
      <div class="col-md-4 mb-4">
        <div class="card">
          <img src="/assets/img/RPL.jpeg" alt="Basketball" class="card-img-top" style="height: 200px; object-fit: cover" />
          <div class="card-body">
            <h5 class="card-title">JURUSAN PPLG</h5>
            <p class="card-text">
              Jurusan PPLG atau Pengembangan Perangkat Lunak dan Gim adalah merupakan jurusan yang mempelajari tentang perkembangan perangkat lunak meliputi pembuatan, manajemen organisasi pengembangan perangkat lunak, pemeliharaan dan
              manajemen kualitas. .
            </p>
            <a href="/jurusan/ipa" class="btn btn-primary">Lihat Detail</a>
          </div>
        </div>
      </div>

      <!-- Jurusan 2: IPS -->
      <div class="col-md-4 mb-4">
        <div class="card">
          <img src="/assets/img/tkj.jpeg" alt="Basketball" class="card-img-top" style="height: 200px; object-fit: cover" />
          <div class="card-body">
            <h5 class="card-title">JURUSAN TJKT</h5>
            <p class="card-text">
              Teknik Jaringan Komputer dan Telekomunikasi (TJKT) merupakan program keahlian yang membekali peserta didik dengan keterampilan, pengetahuan, dan sikap agar kompeten dalam merakit, menginstall program, merawat dan memperbaiki
              komputer serta jaringannya..
            </p>
            <a href="/jurusan/ips" class="btn btn-primary">Lihat Detail</a>
          </div>
        </div>
      </div>

      <!-- Jurusan 3: Bahasa -->
      <div class="col-md-4 mb-4">
        <div class="card">
          <img src="/assets/img/tbsm.jpeg" alt="Basketball" class="card-img-top" style="height: 200px; object-fit: cover" />
          <div class="card-body">
            <h5 class="card-title">JURUSAN TBSM</h5>
            <p class="card-text">
              Teknik Bisnis Sepeda Motor adalah kompetensi keahlian pada Bidang Studi Keahlian Teknologi dan Rekayasa Program Studi Keahlian Teknik Otomotif yang menekankan pada keterampilan pelayanan jasa mekanik kendaraan sepeda motor
              roda dua..
            </p>
            <a href="/jurusan/bahasa" class="btn btn-primary">Lihat Detail</a>
          </div>
        </div>
      </div>
    </section>
  </div>
</template>

<script>
export default {
  name: "Jurusan",
};
</script>

<style scoped>
/* Styling tambahan untuk halaman jurusan */
.card {
  border-radius: 10px;
  border: 1px solid #ddd;
}

.card-img-top {
  height: 200px;
  object-fit: cover;
}

h2 {
  color: #0056b3;
  font-weight: bold;
  margin-bottom: 20px;
}

.table {
  background-color: #fff;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
}

.table th,
.table td {
  text-align: center;
  vertical-align: middle;
}

.table-bordered {
  border: 1px solid #ddd;
}

.table th {
  background-color: #f8f9fa;
  color: #0056b3;
}

.card-body {
  padding: 20px;
}
</style>
