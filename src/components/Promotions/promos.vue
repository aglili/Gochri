<template>
  <div class="container p-4 bg-light">
    <h1> Promotions d'Aujourd'hui</h1>
    <div class="row">
        <promotion
        v-for="promotion in promotions"
        :key="promotion.id"
        :promotion="promotion" />
    </div>
  </div>
</template>
<script>
import promotion from "@/components/Promotions/promotion.vue";
export default {
  components: {
    promotion
  },
  data: () => {
    return {
      promotions: [
        {
          id: 1,
          img: "images/valencia.jpg",
          url: "#",
          name: "Jus Valencia 1L",
          price: 12
        },
        {
          id: 2,
          img: "images/café2.jpg",
          url: "#",
          name: "Nescafé caffé",
          price: 50
        },
        {
          id: 3,
          img: "images/eau.jpg",
          url: "#",
          name: "Pack Sidi ali Eau",
          price: 25
        },
        {
          id: 4,
          img: "images/Panzani.png",
          url: "#",
          name: "Les pattes panzani 1Kg",
          price: 30
        },
        {
          id: 5,
          img: "images/nutella.jpg",
          url: "#",
          name: "Nutelle 750g",
          price: 85
        },
        {
          id: 6,
          img: "images/danone.webp",
          url: "#",
          name: "Yaourt nature DANONE",
          price: 18
        },
        {
          id: 7,
          img: "images/huile t.jpg",
          url: "#",
          name: "Huile de table 1L",
          price: 13
        },
        {
          id: 8,
          img: "images/kiri.png",
          url: "#",
          name: "Fromage Kiri de 432g",
          price: 30
        },
        {
          id: 9,
          img: "images/sucr.jpg",
          url: "#",
          name: "Sucre en poudre 1Kg",
          price: 13
        },
        {
          id: 10,
          img: "images/charcutrie.jpg",
          url: "#",
          name: "charcutrie Koutoubia 250g",
          price: 30
        }

      ]
    }
  }
}
</script>
<style style="scss" scoped>
.row {
  justify-content: space-around;
}
@media (max-width: 600px) {
  h1 {
      font-size: 35px !important;
  }
}
</style>
