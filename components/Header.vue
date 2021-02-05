<template>
  <nav
    class="z-10 flex items-center p-3 flex-wrap bg-gradient-to-r bg-jti-purple sticky top-0 w-full"
  >
    <div class="mx-6 md:mx-10" @click="toggleMenu($event)">
      <NuxtLink to="/2021/">
        <div class="inline-flex items-center">
          <img
            class="bg-contain h-20 w-32"
            src="../assets/LogoJTI_negativo.svg"
            alt="Jornada Técnica de Ingeniería"
          />
        </div>
      </NuxtLink>
    </div>
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
        ref="menu"
        class="flex flex-wrap flex-col lg:flex-row lg:ml-auto lg:w-auto w-full lg:items-center lg:h-auto"
      >
        <NuxtLink to="/2021/programa">
          <div
            class="text-center lg:w-auto w-full px-3 py-2 rounded textunderline"
            @click="toggleMenu($event)"
          >
            <span>Programa</span>
          </div>
        </NuxtLink>

        <NuxtLink to="/2021/organizacion">
          <div
            class="text-center lg:w-auto w-full px-3 py-2 rounded textunderline"
            @click="toggleMenu($event)"
          >
            <span>Organización</span>
          </div>
        </NuxtLink>

        <NuxtLink to="/2021/participantes">
          <div
            class="text-center lg:w-auto w-full px-3 py-2 rounded textunderline"
            @click="toggleMenu($event)"
          >
            <span>Participantes</span>
          </div>
        </NuxtLink>

        <a
          href="https://eventos.ull.es/go/jtiesit2019"
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
    toggleMenu(event) {
      const activeElement = this.$refs.menu.querySelector(".active");
      if (activeElement) {
        activeElement.classList.remove("active");
      }

      if (event) {
        event.target.classList.add("active");
        if (event.target.src && !this.toggle) return;
      }

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
  text-decoration-thickness: 2px;
}

.active {
  font-weight: bold;
}
</style>
