<template>
  <div class="w-full min-h-screen">
    <InformationBlock title="Patrocinadores" description="Quienes nos apoyan" />
    <Sponsorship title="Organizan" :companies="organizan" />
    <Sponsorship title="Colaboran" :companies="colaboran" />
    <Sponsorship title="Participan" :companies="participan"/>
  </div>
</template>

<script>
export default {
  data() {
    return {
      organizan: [{
        "name": "ull",
        "image": "~assets/colaboran/ull.jpg"
      },
      {
        "name": "fifede",
        "image": "~assets/colaboran/fifede.jpg"
      },
      {
        "name": "cabildo",
        "image": "~assets/colaboran/cabildo.jpg"
      }],
      colaboran: [],
      participan: []
    };
  }
};
</script>
