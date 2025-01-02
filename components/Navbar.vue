<template>
  <nav class="navbar navbar-expand-lg bg-secondary sticky-top" style="width: 100%">
    <div class="container-fluid">
      <a class="navbar-brand" href="#">
        <img src="~assets/img/logo.png" alt="logo" width="70" />
      </a>
      <h3 class="text-white">SMKN Negeri 4 Tasikmalaya</h3>
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav"
        aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse justify-content-end" id="navbarNav">
        <ul class="navbar-nav">
          <nuxt-link to="/">
            <li class="nav-item">
              <h4 class="nav-link active" aria-current="page" href="#">
                Beranda
              </h4>
            </li>
          </nuxt-link>
          <nuxt-link to="/profil">
            <li class="nav-item">
              <h4 class="nav-link" href="">Profil</h4>
            </li>
          </nuxt-link>
          <nuxt-link to="/galeri">
            <li class="nav-item">
              <a class="nav-link" href="">Galeri</a>
            </li>
          </nuxt-link>
          <nuxt-link to="/eskul">
            <li class="nav-item">
              <a class="nav-link" href="">Ekstrakurikuler</a>
            </li>
          </nuxt-link>
          <nuxt-link to="/kontak">
            <li class="nav-item">
              <a class="nav-link" href="">Kontak</a>
            </li>
          </nuxt-link>
        </ul>
      </div>
    </div>
  </nav>
</template>

<style scoped>
a {
  text-decoration: none;
}
</style>

<script setup>
useHead({
  title: "profil",
  meta: [
    {
      name: "description",
      content: "profil",
    },
  ],
});
</script>