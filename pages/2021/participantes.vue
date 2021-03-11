<template>
  <div class="w-full min-h-screen">
    <InformationBlock title="Participantes" description="Quienes hacen posible el evento" />
    <Sponsorship title="Organizan" :companies="organizan" />
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
      participan: [{
        name: "tenerife juega",
        image: "../img/participan/logotenerifejuega.png"
      },
      {
        name: "Innovalia",
        image: "../img/participan/logoinnovalia.jpg"
      },
      {
        name: "Scytl",
        image:  "../img/participan/logoscytl.jpg"
      },
      {
        name: "Metrotenerife",
        image:  "../img/participan/logometrotenerife.jpg"
      }],
    };
  },
};
</script>
