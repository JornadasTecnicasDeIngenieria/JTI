<template>
  <nav
    class="z-10 flex items-center p-3 flex-wrap bg-gradient-to-r from-jti-black to-jti-black sticky top-0 w-full"
  >
<<<<<<< HEAD
    <NuxtLink to="/2021/">
      <div class="mx-6 md:mx-10 inline-flex items-center">
        <img
          class="bg-contain h-20 w-32"
          src="../assets/LogoJTI_negativo.svg"
=======
    <NuxtLink to="/2021/programa">
      <div class="mx-6 md:mx-10 inline-flex items-center">
        <img
          class="bg-contain h-20 w-32"
          src="../assets/LogoJTI_negativo2.svg"
>>>>>>> b305212b8ff1f73e9ad6a0f84d32581d7d2ddcd5
          alt="Jornada Técnica de Ingeniería"
        >
        <!--  <span class="text-jti-white h-12 w-40 ml-6 font-bold">Jornadas Técnica de Ingeniería</span>-->
      </div>
    </NuxtLink>
    <button
      class="text-jti-white inline-flex p-3 rounded lg:hidden ml-auto hover:text-white outline-none nav-toggler"
      @click="toggleMenu()"
    >
      <i ref="menuicon" class="material-icons">menu</i>
    </button>
    <div
      ref="navigation"
      class="hidden top-navbar w-full lg:inline-flex lg:w-auto text-jti-white"
    >
      <div
        class="flex flex-wrap flex-col lg:flex-row lg:ml-auto lg:w-auto w-full lg:items-center lg:h-auto"
      >
        <NuxtLink to="/2021/programa">
          <div
            class="text-center lg:w-auto w-full px-3 py-2 rounded textunderline"
          >
            <span>Programa</span>
          </div>
        </NuxtLink>

        <NuxtLink to="/2021/organizacion">
          <div
            class="text-center lg:w-auto w-full px-3 py-2 rounded textunderline"
          >
            <span>Organización</span>
          </div>
        </NuxtLink>

<<<<<<< HEAD
        <NuxtLink to="/2021/participantes">
          <div
            class="text-center lg:w-auto w-full px-3 py-2 rounded textunderline"
          >
            <span>Participantes</span>
=======
        <NuxtLink to="/2021/patrocinadores">
          <div
            class="text-center lg:w-auto w-full px-3 py-2 rounded textunderline"
          >
            <span>Patrocinadores</span>
>>>>>>> b305212b8ff1f73e9ad6a0f84d32581d7d2ddcd5
          </div>
        </NuxtLink>

        <a
          href="https://eventos.ull.es/31301/detail/jornada-tecnica-de-ingenieria.html"
          class="text-center lg:w-auto w-full px-3 py-2 rounded textunderline"
          target="_blank"
        >
          <span>Edición Anterior</span>
        </a>
      </div>
    </div>
  </nav>
</template>

<script>
export default {
  name: "Header",
  data: () => {
    return {
      toggle: false,
    };
  },
  methods: {
    toggleMenu() {
      if (this.toggle) {
        this.$refs.navigation.classList.add("hidden");
        this.$refs.menuicon.textContent = "menu";
      } else {
        this.$refs.navigation.classList.remove("hidden");
        this.$refs.menuicon.textContent = "close";
      }
      this.toggle = !this.toggle;
    },
  },
};
</script>
<style scoped>
#navigation {
  font-family: "Rubik", sans-serif;
}

.textunderline:hover {
  text-decoration: underline;
  text-decoration-color: #1d9cd8;
  text-underline-offset: 4px;
}
</style>
