<template>
  <div class="w-full min-h-screen">
    <InformationBlock title="Participantes" description="Quienes nos apoyan" />
    <Sponsorship title="Organizan" :companies="organizan" />
    <Sponsorship title="Colaboran" :companies="colaboran" />
    <Sponsorship title="Participan" :companies="participan" />
  </div>
</template>

<script>
export default {
  data() {
    return {
      organizan: [
        {
          name: "ull",
          image: "../img/organizan/ull.png",
        },
        {
          name: "fifede",
          image: "../img/organizan/fifede.png",
        },
        {
          name: "cabildo",
          image: "../img/organizan/cabildo.png",
        },
      ],
      colaboran: [],
      participan: [],
    };
  },
};
</script>
