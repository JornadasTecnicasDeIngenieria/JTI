<template>
  <div class="w-full">
    <div
      class="wrapper flex flex-wrap justify-center md:justify-around"
    >
      <div class="w-72 py-6 px-4 flex flex-col">
        <font-awesome-icon
          class="text-6xl text-center self-center mb-4 text-blue-700"
          :icon="['fas', 'users']"
        />
        <h4 class="text-center mb-2">El mercado laboral</h4>
        <p class="text-center">
          ¿Ya sabes dónde quieres trabajar?, ¿no encuentras las empresas que
          encajan con la formación que has recibido? Hay una gran variedad de
          empresas en el sector de la ingeniería en Canarias que te están
          buscando. Conoce los intereses de cada una de ellas y así lograrás
          descubrir cuál es tu empresa ideal.
        </p>
      </div>

      <div class="w-72 py-8 px-4 flex flex-col">
        <font-awesome-icon
          class="text-6xl text-center self-center mb-4 text-yellow-600"
          :icon="['fas', 'lightbulb']"
        />
        <h4 class="text-center mb-2">Tu empleo ideal</h4>
        
        <p class="text-center">
          Seas industrial o informático, muchas son las opciones que se te abren
          al finalizar tu grado en la ESIT. Descubre de una manera más cercana
          cuáles son las labores que realmente se realizan en una empresa y
          dónde está tu lugar.
        </p>
      </div>

      <div class="w-72 py-8 px-4 flex flex-col">
        <font-awesome-icon
          class="text-6xl text-center self-center mb-4 text-jti-blue"
          :icon="['fas', 'chalkboard-teacher']"
        />
        <h4 class="text-center mb-2">Grandes profesionales</h4>

        <p class="text-center">
          Un gran número de profesionales del sector están invitados a dar su
          experiencia en el desempeño de sus labores así como contar cómo fue su
          proceso de selección. Además, podrás escuchar a egresados de la ESIT
          contándote de primera mano cómo ha sido su salto de la Universidad a
          la Empresa.
        </p>
      </div>
    </div>
  </div>
</template>
