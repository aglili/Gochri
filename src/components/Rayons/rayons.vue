<template>
  <div class="container pl-0">
    <h1 class="pt-4 text-light">Nos rayons les plus visité</h1>
    <div class="row">
    <rayon
    v-for="rayon in rayons"
    :key="rayon.id"
    :rayon="rayon" />
    </div>
  </div>
</template>

<script>
import rayon from "@/components/Rayons/rayon.vue";
export default {
  components: {
    rayon
  },
  data: function() {
    return {
      rayons: [
        {
          id: 1,
          img: "images/fruits.png",
          parag: "Fruits et légumes",
          url: "#"
        },
        {
          id: 2,
          img: "images/pains.png",
          parag: "Pains",
          url: "#"
        },
        {
          id: 3,
          img: "images/épicerir.png",
          parag: "Epicerie salée",
          url: "#"
        },
        {
          id: 4,
          img: "images/viande1.png",
          parag: "Viandes et poissons",
          url: "#"
        },
        {
          id: 5,
          img: "images/Buttonplus.svg",
          parag: "tous les rayons",
          url: "#"
        },
      ]
    };
  }
}
</script>
<style lang="scss" scoped>
$orange: #f3973a;
.container{
  background: $orange;
  border-radius: 10px;
}
.row{
  justify-content: center;
}

@media (max-width: 600px) {
  h1 {
      font-size: 35px !important;
  }
}
</style>
