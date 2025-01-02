<template>
  <div class="container">
    <h1 class="text-center">Kegiatan</h1>
    <div class="row pb-5">
      <div v-for="(kegiatan, i) in galeri" :key="i" class="col-lg-3">
        <img :src="kegiatan.poto" class="img-thumbnail" alt="..." />
      </div>
    </div>
  </div>
  <div class="container">
    <h1 class="text-center">Baju Seragam</h1>
    <div class="row pb-5">
      <div v-for="(seragam, i) in poto" :key="i" class="col-lg-3">
        <img :src="seragam.foto" class="img-thumbnail" alt="..." />
      </div>
    </div>
  </div>
</template>

<script setup>
useHead({
  title: "galeri",
  meta: [
    {
      name: "description",
      content: "galeri",
    },
  ],
});
const supabase = useSupabaseClient();

const galeri = ref([]);

const poto = ref([]);

const getData = async () => {
  const { data } = await supabase.from("galeri").select(`*`);
  if (data) galeri.value = data;
};
const getPhoto = async () => {
  const { data } = await supabase.from("seragam").select(`*`);
  if (data) poto.value = data;
};

onMounted(() => {
  getData();
  getPhoto();
});
</script>