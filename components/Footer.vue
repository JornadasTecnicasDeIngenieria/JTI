<template>
  <footer class="text-white bg-jti-black h-32">
    <div
      class="wrapper h-full flex justify-center flex-col-reverse md:flex-row"
    >
      <div class="md:w-1/2 font-bold flex text-xs md:text-base pb-2 justify-center">
        <p class="self-center">
          ©2021 Jornadas Técnicas de Ingeniería. All rights reserved
        </p>
      </div>
      <div
        class="md:w-1/2 h-full flex flex-col justify-center"
      >
        <div class="space-x-8 text-3xl flex self-center">
          <font-awesome-icon class="self-center" :icon="['fab', 'linkedin']" />
          <font-awesome-icon class="self-center" :icon="['fab', 'instagram']" />
          <font-awesome-icon class="self-center" :icon="['fab', 'twitter']" />
        </div>
        <span class="font-bold self-center mt-2">jtiesit@ull.edu.es</span>
      </div>
    </div>
  </footer>
</template>
