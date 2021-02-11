<template>
  <div class="w-full min-h-screen">
    <InformationBlock
      title="Organización"
      description="El equipo que hace posible el evento"
    />
    <div class="flex flex-row flex-wrap justify-center wrapper py-8">
      <PersonCard
        :image-url="require('~/assets/organizadores/andreshdez.jpeg')"
        v-bind:information="{
          title: 'Organizador',
          name: 'Andrés Hernández',
          linkedin:
            'https://www.linkedin.com/in/andr%C3%A9s-hern%C3%A1ndez-a3ab4b134/',
        }"
      />

      <PersonCard
        :image-url="require('~/assets/organizadores/nahiaganuza.jpeg')"
        v-bind:information="{
          title: 'Organizadora',
          name: 'Nahia Ganuza',
          linkedin:
            'https://www.linkedin.com/in/nahia-ganuza-izaguirre-a56866205/',
        }"
      />

      <PersonCard
        :image-url="require('~/assets/organizadores/helenagarcia.jpeg')"
        v-bind:information="{
          title: 'Organizadora',
          name: 'Helena García',
          linkedin:
            'https://www.linkedin.com/in/helena-garc%C3%ADa-d%C3%ADaz-b1179a1bb/',
        }"
      />

      <PersonCard
        :image-url="require('~/assets/organizadores/ivanelias.jpeg')"
        v-bind:information="{
          title: 'Organizador',
          name: 'Iván Elías',
          linkedin: 'https://www.linkedin.com/in/ivaneliasarmas/',
        }"
      />

      <PersonCard
        :image-url="require('~/assets/organizadores/adrianglez.jpeg')"
        v-bind:information="{
          title: 'Organizador',
          name: 'Adrián González',
          linkedin: 'https://www.linkedin.com/in/adri%C3%A1n-gonz%C3%A1lez-hern%C3%A1ndez/',
        }"
      />

      <PersonCard
        :image-url="require('~/assets/organizadores/saracumplido.jpeg')"
        v-bind:information="{
          title: 'Asesora de diseño',
          name: 'Sara Cumplido',
          linkedin: 'https://www.linkedin.com/in/sara-cumplido-1b2a57205/',
        }"
      />

      <PersonCard
        :image-url="require('~/assets/organizadores/kevineliezer.jpeg')"
        v-bind:information="{
          title: 'Organizador',
          name: 'Kevin Eliezer',
          linkedin: 'https://www.linkedin.com/in/kevineliezer/',
        }"
      />
      <PersonCard
        :image-url="require('~/assets/organizadores/humbertojose.jpeg')"
        v-bind:information="{
          title: 'Coordinador JTI',
          name: 'Humberto J. Glez.',
          linkedin: 'https://www.linkedin.com/in/hgonarjr/',
        }"
      />
    </div>
  </div>
</template>
