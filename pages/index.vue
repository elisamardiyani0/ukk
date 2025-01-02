<template>
  <div class="container-fuild">
    <div class="carousel-inner">
      <div class="carousel-item active custom-bg">
        <div class="overlay">
          <div>
            <h1 class="custom-text text-center">
              Selamat Datang di Sekolah Pusat Keunggulan SMKN 4 Tasikmalaya
            </h1>
          </div>
        </div>
      </div>
    </div>

    <div class="text-center p-5">
      <div class="row">
        <div class="col-lg-4">
          <img src="/assets/img/kepsek.jpeg" alt="" style="width: 25rem" class="p-2" />
          <p class="fs-2">Kurniawan,S.Pd,M.pd</p>
        </div>
        <div class="col-lg-8 p-5 mt-5">
          <p class="fs-1">SAMBUTAN KEPALA SEKOLAH</p>
          <p style="text-align: justify">
            Assalamualaikum Warahmatullahi Wabarakatuh Selamat datang di SMKN 4
            Tasikmalaya. Segala puji dan syukur kita panjatkan kehadirat Allah
            SWT, semoga kita semua ada dalam lindungan-Nya. Dan atas
            perkenan-Nya pula kami dapat menghadirkan website SMK Negeri 4
            Tasikmalaya ini. Kami berharap dengan adanya website di SMK Negeri 4
            Tasikmalaya ini para pengunjung dapat mengenal lebih jauh tentang
            sekolah kami sehingga dapat mempererat tali silaturrahmi antara
            sekolah dengan masyarakat demi kemajuan kita bersama. Tiada gading
            yang tak retak, website kami ini masih dalam proses pengembangan,
            masih banyak kekurangan yang harus kami perbaiki. Kritik dan
            sarannya yang membangun sangat kami harapkan untuk pengembangan ke
            depan. Akhirnya,saya mengucapkan terimakasih yang sebesar-besarnya
            kepada semua pihak yang tidak dapat disebutkan satu segala bantuan
            dan persatu atas fasilitasnya yang telah diberikan semoga semua yang
            kita lakukan bermanfaat bagi masyarakat. Wassalamu'alaikum
            Warahmatullahi Wabarakatuh.
          </p>
        </div>
      </div>
    </div>
    <div class="text-center">
      <h1 class="text-center mt-5 mb-5">Ujikompetensi Keahlian</h1>
    </div>
    <div class="container bg-secondary">
      <div class="row p-5">
        <div class="col-lg-4">
          <div class="card" style="width: 15rem">
            <img src="/assets/img/pplg.png" class="card-img-top" alt="..." />
            <div class="card-body">
              <h5 class="card-title">
                PPLG (pengembangan perangkat lunak dan Gim)
              </h5>
            </div>
          </div>
        </div>
        <div class="col-lg-4">
          <div class="card" style="width: 15rem">
            <img src="/assets/img/tkjt.png" class="card-img-top" alt="..." />
            <div class="card-body">
              <h5 class="card-title">
                TJKT(Teknik Jaringan Komputer Dan Telekomunikasi )
              </h5>
            </div>
          </div>
        </div>
        <div class="col-lg-4">
          <div class="card" style="width: 15rem">
            <img src="/assets/img/tbsm.png" class="card-img-top" alt="..." />
            <div class="card-body">
              <h5 class="card-title">TBSM (Teknik Dan Bisnis Sepeda Motor)</h5>
            </div>
          </div>
        </div>
        <div class="col-lg-4 pt-5">
          <div class="card" style="width: 15rem">
            <img src="/assets/img/toi.png" class="card-img-top" alt="..." />
            <div class="card-body">
              <h5 class="card-title">TOI(Teknik Otomasi Industri)</h5>
            </div>
          </div>
        </div>
        <div class="col-lg-4 pt-5">
          <div class="card" style="width: 15rem">
            <img src="/assets/img/dkv.png" class="card-img-top" alt="..." />
            <div class="card-body">
              <h5 class="card-title">DKV(Desain Komunikasi Visual)</h5>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="container">
      <div class="judul">
        <h1 class="text-center mt-5 mb-5">STATISIK</h1>
      </div>
      <div class="row">
        <div class="col-6 P-5">
          <div class="card m-5 p-5 bg-secondary light">
            <div class="row">
              <div class="col">
                <h3 class="text-white">GURU</h3>
              </div>
              <div class="col">
                <h3 class="text-white">80</h3>
              </div>
            </div>
          </div>
        </div>
        <div class="col-6 P-5">
          <div class="card m-5 p-5 bg-secondary">
            <div class="row">
              <div class="col">
                <h3 class="text-white">SISWA</h3>
              </div>
              <div class="col">
                <h3 class="text-white">1500</h3>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
    <!-- <div class="container">
      <h1 class="text-center mt-5 mb-5">Berita</h1>
      <div class="row mb-5">
        <div v-for="(berita, i) in cover" :key="i" class="col-lg-4">
          <div class="card" style="width: 18rem">
            <img :src="berita.poto" class="card-img-top" alt="..." />
            <div class="card-body">
              <h5 class="card-title">{{ berita.nama }}</h5>
              <a
                href="https://radartasik.id/2024/05/16/smk-negeri-4-tasikmalaya-ikuti-pelatihan-safety-riding-yang-diselenggarakan-pt-daya-adicipta-motora/"
                class="btn btn-primary"
                >Go somewhere</a
              >
            </div>
          </div>
        </div>
      </div>
    </div> -->
  </div>
</template>

<style scoped>
.custom-bg {
  position: relative;
  height: 100vh;
  background-image: url("assets/img/home.jpeg");
  background-size: cover;
  /* Resize the background image */
  background-position: center;
  /* Center the image */
}

.overlay {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  display: flex;
  align-items: center;
  justify-content: center;
}

.custom-text {
  color: white;
  background-color: rgba(13, 110, 253, 0.5);
  font-weight: bold;
}
</style>

<script setup>
useHead({
  title: "Beranda",
  meta: [
    {
      name: "description",
      content: "Beranda",
    },
  ],
});
// const supabase = useSupabaseClient();

// const cover = ref([]);

// const getData = async () => {
//   const { data } = await supabase.from("berita").select(`*`);
//   if (data) cover.value = data;
// };

// onMounted(() => {
//   getData();
// });
</script>