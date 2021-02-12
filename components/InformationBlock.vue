<template>
  <div class="h-48 w-full sm:h-64 bg-gradient-to-tr from-jti-purple to-jti-blue">
    <div
      class="text-sm md:text-base wrapper w-full flex flex-col h-full justify-center content-center flex-wrap lg:content-start"
    >
      <h1>{{ title }}</h1>
      <h3 class="text-base self-center md:text-3xl lg:self-start">{{ description }}</h3>
    </div>
  </div>
</template>

<script>
export default {
  name: "InformationBlock",
  props: {
    title: {
      type: String,
      default: "",
    },
    description: {
      type: String,
      default: "",
    },
  },
};
</script>

<style scoped>
</style>
