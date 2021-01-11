<template>
  <div class="w-full h-80 bg-green-500">
    <div class="wrapper flex flex-col h-full justify-center content-center flex-wrap md:content-start">
      <h1>{{ title }}</h1>
      <h2>{{ description }}</h2>
    </div>
  </div>
</template>

<script>
export default {
  name: 'InformationBlock',
  props: {
    title: {
      type: String,
      default: ''
    },
    description: {
      type: String,
      default: ''
    }
  }
};
</script>

<style scoped>
h1 {
  font-weight: bold;
}
</style>
