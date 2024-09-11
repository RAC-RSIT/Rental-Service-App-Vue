<script setup>
import Navbar from "./components/Navbar.vue";
import PropertyList from "./components/PropertyList.vue";
</script>

<template>
  <section class="container mt-5">
    <div class="row">
      <div class="col-3 d-flex justify-content-center">
        <Navbar></Navbar>
      </div>
      <div class="col-9">
        <PropertyList></PropertyList>
      </div>
    </div>
  </section>
</template>
