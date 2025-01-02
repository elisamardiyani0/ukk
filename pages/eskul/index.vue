<template>
  <div class="container">
    <h2 class="text-center mb-4">Ekstrakulikuler</h2>
    <div class="row">
      <div v-for="(data, i) in eskul" :key="i" class="col-lg-6">
        <div class="card mb-3" style="max-width: 540px">
          <div class="row g-0">
            <div class="col-md-4">
              <img :src="data.poto" class="img-fluid rounded-start" alt="..." />
            </div>
            <div class="col-md-8">
              <div class="card-body">
                <h5 class="card-title">{{ data.nama }}</h5>
                <h6 clas="card-title">{{ data.ket }}</h6>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
useHead({
  title: "Ekstrakurikuler",
  meta: [
    {
      name: "description",
      content: "Ekstrakurikuler",
    },
  ],
});
const supabase = useSupabaseClient();

const eskul = ref([]);

const getData = async () => {
  const { data } = await supabase.from("eskul").select(`*, nama,poto`);
  if (data) eskul.value = data;
};

onMounted(() => {
  getData();
});
</script>



































<!-- <template>
  <div class="container">
    <h2 class="text-center mb-4">Ekstrakulikuler</h2>
    <div class="row">
      <div v-for="(data, i) in eskul" :key="i" class="col-lg-6">
        <div class="card mb-3" style="max-width: 540px">
          <div class="row g-0">
            <div class="col-md-4">
              <img :src="data.poto" class="img-fluid rounded-start" alt="..." />
            </div>
            <div class="col-md-8">
              <div class="card-body">
                <h5 class="card-title">{{ data.nama }}</h5>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template> -->