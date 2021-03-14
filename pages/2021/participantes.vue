<template>
  <div class="w-full min-h-screen">
    <InformationBlock title="Participantes" description="Quienes hacen posible el evento" />
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
      colaboran: [
        {
          name: "COITIC",
          image: "../img/colaboran/COITIC.png",
        },
        {
          name: "COITITF",
          image: "../img/colaboran/COITITF.png",
        },
        {
          name: "Recinto Ferial",
          image: "../img/colaboran/RecintoFerial.png",
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
