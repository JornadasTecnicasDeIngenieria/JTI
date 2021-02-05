<template>
  <div class="wrapper py-4">
    <h3 class="p-4 text-jti-purple text-center lg:text-left">
      {{ this.title }}
    </h3>
    <div class="bg-jti-blue w-full h-1 rounded-full"></div>

    <div ref="organizations" class="w-full flex justify-around flex-wrap">
      <!-- <div v-for="item in companies">
        <img class="h-24 m-4" :src="item.image" :alt="item.name" />
      </div>
      <div class="bg-jti-blue w-full h-05 rounded-full mb-6"></div>
      <div v-for="item in companies">
        <img class="h-24 m-4" :src="item.image" :alt="item.name" />
      </div> -->
    </div>
    <div class="bg-jti-blue w-full h-1 rounded-full"></div>
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
  mounted() {
    let parent = document.createElement("div");
    parent.classList.add("flex", "flex-wrap", "justify-around");

    // Puts three organizations logos per row, separated by a blue line
    for (let index = 0; index < this.companies.length; index++) {
      let image = document.createElement("img");
      image.classList.add("h-24", "m-4");
      image.src = this.companies[index].image;
      image.alt = this.companies[index].alt;
      parent.appendChild(image);

      if (index === this.companies.length - 1) {
        this.$refs.organizations.appendChild(parent);
      } else if ((index + 1) % 3 === 0) {
        this.$refs.organizations.appendChild(parent);
        parent = document.createElement("div");
        parent.classList.add("flex", "flex-wrap", "justify-around");
        let line = document.createElement("div");
        line.classList.add("h-05", "bg-jti-blue", "w-full");
        this.$refs.organizations.appendChild(line);
      }
    }
  },
};
</script>
