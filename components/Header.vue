<template>
  <nav class="flex items-center p-3 flex-wrap bg-gradient-to-r from-jti-black to-jti-black sticky top-0 w-full">
    <a href="/2021/" class="mx-6  inline-flex items-center">
      <img
        class="bg-contain h-20 w-32"
        src="../assets/LogoJTI_negativo.png"
        alt="Jornada Técnica de Ingeniería"
      >
    <!--  <span class="text-jti-white h-12 w-40 ml-6 font-bold">Jornadas Técnica de Ingeniería</span>-->
    </a>
    <button
      class="text-jti-white inline-flex p-3 hover:bg-gray-800 rounded lg:hidden ml-auto hover:text-white outline-none nav-toggler"
      data-target="#navigation"
    >
      <i class="material-icons">menu</i>
    </button>
    <div
      id="navigation"
      class="hidden top-navbar w-full lg:inline-flex lg:w-auto text-jti-white"
    >
      <div
        class="lg:flex-row lg:ml-auto lg:w-auto w-full lg:items-center lg:h-auto"
      >
        <a
          href="/2021/sobre-el-evento"
          class="lg:w-auto w-full px-3 py-2 rounded items-center justify-center hover:bg-gray-800 hover:text-white"
        >
          <span>Programa</span>
        </a>
        <a
          href="/2021/organizadores"
          class="lg:w-auto w-full px-3 py-2 rounded items-center justify-center hover:bg-gray-800 hover:text-white"
        >
          <span>Organizadores/as</span>
        </a>
        <a
          href="/2021/patrocinadores"
          class="lg:w-auto w-full px-3 py-2 rounded items-center justify-center hover:bg-gray-800 hover:text-white"
        >
          <span>Patrocinadores</span>
        </a>
        <a
          href="/2021/#"
          class="lg:w-auto w-full px-3 py-2 rounded items-center justify-center hover:bg-gray-800 hover:text-white"
        >
          <span>Ediciones Anteriores</span>
        </a>
      </div>
    </div>
  </nav>
</template>

<style scoped>
nav {
  font-family: "Rubik", sans-serif;
}
</style>
