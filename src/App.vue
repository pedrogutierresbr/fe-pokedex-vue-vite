<script setup>
</script>

<template>
  <nav class="navbar navbar-expand-lg navbar-dark bg-primary">
    <div class="container-fluid">
      <router-link class="navbar-brand" to="/">
        <img src="./assets/icon.svg" alt="Logo" width="30" height="30" class="d-inline-block align-text-top">
        PokeVite
      </router-link>
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav"
        aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarNav">
        <ul class="navbar-nav">
          <li class="nav-item">
            <router-link class="nav-link" aria-current="page" to="/">Home</router-link>
          </li>
          <li class=" nav-item">
            <router-link class="nav-link" to="/about">About</router-link>
          </li>
        </ul>
      </div>
    </div>
  </nav>

  <div class="main">
    <router-view></router-view>
  </div>

  <footer class="bg-primary text-light">
    <div>Design in{{ new Date().getFullYear() }}</div>
  </footer>
</template>

<style >
body {
  height: 100vh;
  background: rgb(45, 101, 253);
  background: linear-gradient(90deg, rgba(45, 101, 253, 1) 0%, rgba(106, 196, 233, 0.94) 100%);
}

footer {
  position: fixed;
  bottom: 0;
  width: 100%;
  height: 56px;
  display: flex;
  align-items: center;
  justify-content: center;
}
</style>
