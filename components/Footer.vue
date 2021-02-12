<template>
  <footer class="text-white bg-jti-purple h-32">
    <div
      class="wrapper h-full flex justify-center flex-col-reverse lg:flex-row"
    >
      <div
        class="lg:w-1/2 font-bold flex text-xs md:text-base pb-2 justify-center"
      >
        <p class="text-xs md:text-base self-center">
          ©2021 Jornadas Técnicas de Ingeniería. Todos los derechos reservados
        </p>
      </div>
      <div class="lg:w-1/2 h-full flex flex-col justify-center">
        <div class="space-x-8 text-3xl flex self-center">
          <a href="https://www.linkedin.com/company/jtiesit/" target="_blank">
            <font-awesome-icon
              class="self-center"
              :icon="['fab', 'linkedin']"
            />
          </a>
          <a href="https://www.instagram.com/jtiesit/" target="_blank">
            <font-awesome-icon
              class="self-center"
              :icon="['fab', 'instagram']"
            />
          </a>
          <a href="https://twitter.com/jtiesit" target="_blank">
            <font-awesome-icon class="self-center" :icon="['fab', 'twitter']" />
          </a>
        </div>
        <span class="font-bold self-center mt-2">jtiesit@ull.edu.es</span>
      </div>
    </div>
  </footer>
</template>
