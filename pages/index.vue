<template>
  <div class="w-full header-offset flex justify-center align-center">
    <a
      href="https://eventos.ull.es/go/jtiesit2019"
      class="
        w-40
        h-40
        rounded-xl
        bg-jti-purple-750
        text-white text-4xl
        m-12
        hover:bg-jti-purple
        flex
        content-center
        justify-center
      "
      target="_blank"
    >
      <span class="mt-10"> 2019 </span>
    </a>
    <NuxtLink
      to="/2021"
      class="
        w-40
        h-40
        rounded-xl
        bg-jti-purple-750
        text-white text-4xl
        m-12
        hover:bg-jti-purple
        flex
        content-center
        justify-center
      "
    >
      <div class="mt-10">2021</div>
    </NuxtLink>
  </div>
</template>

<script>
export default {
  layout: "editions",
};
</script>

<style>
.header-offset {
  min-height: calc(100vh - 111px);
}
</style>
