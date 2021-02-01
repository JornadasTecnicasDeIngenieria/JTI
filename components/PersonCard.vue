<template>
  <div
    class="my-4 mx-2 md:m-8 flex flex-col bg-jti-black rounded-xl w-52 h-72 shadow-md"
  >
    <div
      class="w-38 h-38 rounded-full self-center bg-jti-blue mt-4 flex justify-center"
    >
      <img
        class="w-36 h-36 rounded-full self-center justify-self-center"
        :src="imageUrl"
      />
    </div>

    <div class="w-full flex my-1 text-white font-bold p-1">
      <span class="text-base text-center w-full">{{ information.title }}</span>
    </div>

    <div class="w-full flex my-1 text-white">
      <span class="w-full text-base text-center">{{ information.name }}</span>
    </div>

    <div class="flex text-white justify-center pt-1">
      <a :href="information.linkedin">
        <font-awesome-icon
          class="mx-1 text-2xl self-center"
          :icon="['fab', 'linkedin']"
        />
      </a>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    imageUrl: {
      type: String,
      required: true,
    },
    information: {
      type: Object,
      required: true,
    },
  },
};
</script>
