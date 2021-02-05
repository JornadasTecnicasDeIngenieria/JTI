<template>
  <div class="wrapper py-6">
    <h2 class="text-center lg:text-left">{{ this.title }}</h2>
    <div class="shadow overflow-hidden rounded border-b border-gray-200 my-8">
      <table class="min-w-full bg-white text-center">
        <thead class="bg-jti-blue text-white uppercase">
          <tr>
            <th class="w-40"></th>
            <th class="py-3 px-4">
              Sala 1: GII
            </th>
            <th class="py-3 px-4">
              Sala 2: GIQI
            </th>
            <th class="py-3 px-4">
              Sala 3: GIEIA
            </th>
            <th class="py-3 px-4">
              Sala 4: GIM
            </th>
          </tr>
        </thead>
        <tbody class="text-gray-700">
          <tr>
            <td class="py-3 px-4 font-bold">15:00 - 16:00</td>
            <td class="py-3 px-4"><b>Titulo</b></br>Ponencias</td>
            <td class="py-3 px-4"><b>Titulo</b></br>Ponencias</td>
            <td class="py-3 px-4"><b>Titulo</b></br>Ponencias</td>
            <td class="py-3 px-4"><b>Titulo</b></br>Ponencias</td>
          </tr>
          <tr class="bg-gray-100">
            <td class="py-3 px-4 font-bold">16:00 - 17:00</td>
            <td class="py-3 px-4"><b>Titulo</b></br>Ponencias</td>
            <td class="py-3 px-4"><b>Titulo</b></br>Ponencias</td>
            <td class="py-3 px-4"><b>Titulo</b></br>Ponencias</td>
            <td class="py-3 px-4"><b>Titulo</b></br>Ponencias</td>
          </tr>

          <tr>
            <td class="py-3 px-4 font-bold">17:00 - 17:30</td>
            <td class="text-center font-bold" colspan="4">DESCANSO</td>
          </tr>

          <tr class="bg-gray-100">
            <td class="py-3 px-4 font-bold">17:30 - 18:30</td>
            <td class="py-3 px-4"><b>Titulo</b></br>Ponencias</td>
            <td class="py-3 px-4"><b>Titulo</b></br>Ponencias</td>
            <td class="py-3 px-4"><b>Titulo</b></br>Ponencias</td>
            <td class="py-3 px-4"><b>Titulo</b></br>Ponencias</td>
          </tr>

          <tr>
            <td class="py-3 px-4 font-bold">18:30 - 19:30</td>
            <td class="py-3 px-4"><b>Titulo</b></br>Ponencias</td>
            <td class="py-3 px-4"><b>Titulo</b></br>Ponencias</td>
            <td class="py-3 px-4"><b>Titulo</b></br>Ponencias</td>
            <td class="py-3 px-4"><b>Titulo</b></br>Ponencias</td>
          </tr>
        </tbody>
      </table>
    </div>
  </div>
</template>

<script>
export default {
  name: "Schedule",
  props: {
    title: {
      type: String,
      required: true
    },
    table: {
      type: Array,
      required: true
    },
  },
};
</script>

<style scoped>
  th, tr {
    font-family: 'Open Sans';
  }

  th {
    font-weight: bold;
  }
</style>
