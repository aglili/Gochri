<template>
  <div class="container">
    <h1> anna nb </h1>
  </div>
  <div>
    <product
    :v-for="selection in selections"
    :key="selection.id"
    :img="selection.img"
    :princImg="selection.princImg"
    :lien="selection.lien"
    :title="selection.title"
    />
  </div>
</template>

<script>
import selection from "@/components/Selection/selection.vue";
export default {
  components: {
    product
  },
  data: function() {
    return {
      selection: [
        {
          id= 1,
          img: "@/assets/fraise.png",
          title: "Faites",
        },
        {
          id= 2,
          img: "@/assets/fraise.png",
          title: "Faisdds",
        },
      ]
    }
  }
}
</script>
