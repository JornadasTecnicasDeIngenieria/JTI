<template>
  <div>
    <div
      class="w-full bg-left min-h-screen hero bg-fix bg-cover relative"
    ></div>
    <div class="w-full bg-jti-blue h-2"></div>
    <AboutTheEvent />
    <div class="w-full bg-white py-6">
      <ValuesCards />
      <Map />
    </div>
  </div>
</template>

<script>
import Vue from "vue";

export default Vue.extend({});
</script>

<style>
.hero {
  background-image: url("~assets/fondo_jtiesit_texto.jpg");
}

@media (max-width: 684px) {
  .bg-fix {
    background-position: 13% 0;
  }
}
</style>
