<template>
  <nav
    class="
      z-10
      flex
      items-center
      p-3
      flex-wrap
      bg-gradient-to-r bg-jti-purple
      sticky
      top-0
      w-full
      flex
    "
  >
    <div class="mx-6 md:mx-10">
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
      class="
        text-jti-white
        inline-flex
        p-3
        rounded
        lg:hidden
        ml-auto
        hover:text-white
        outline-none
        nav-toggler
      "
    >
      <i ref="menuicon" class="material-icons">menu</i>
    </button>
    <div
      ref="navigation"
      class="hidden top-navbar w-full lg:inline-flex lg:w-auto text-jti-white"
    >
      <div
        ref="menu"
        class="
          flex flex-wrap flex-col
          lg:flex-row
          lg:ml-auto
          lg:w-auto
          w-full
          lg:items-center
          lg:h-auto
        "
      ></div>
    </div>
  </nav>
</template>

<script>
export default {
  name: "HeaderEditions",
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
