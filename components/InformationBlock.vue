<template>
  <div class="w-full h-64 bg-gradient-to-tr from-jti-blue to-jti-purple-750">
    <div
      class="wrapper w-full flex flex-col h-full justify-center content-center flex-wrap lg:content-start"
    >
      <h1>{{ title }}</h1>
      <h3 class="self-center text-xl md:text-3xl lg:self-start">{{ description }}</h3>
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
