<template>
  <div>
    <div class="flex w-full bg-left relative jti-height hero bg-fix bg-cover" />
    <div class="w-full bg-jti-blue h-2 absolute -my-2" />

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

.jti-height {
  min-height: calc(100vh - 111px);
}
</style>
