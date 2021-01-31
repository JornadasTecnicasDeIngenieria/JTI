<template>
  <div class="wrapper">
    <h3 class="py-8">{{ this.title }}</h3>
    <div>
      <span>BLOQUE DE EMPRESAS</span>
      <ul id="example-1">
        <li v-for="item in companies">
          <img :src="item.image"/>
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: "Sponsorship",
  props: {
    title: {
      type: String,
      required: true,
    },
    companies: {
      type: Array,
      required: true,
    },
  },
};
</script>
