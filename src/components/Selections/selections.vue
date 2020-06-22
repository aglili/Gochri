<template>
  <div class="container">
  <h1> La sélection du moment </h1>
    <div class="row">
        <selection
        v-for="selection in selections"
        :key="selection.id"
        :selection="selection" />
    </div>
  </div>
</template>
<script>
import selection from "@/components/Selections/selection.vue";
export default {
  components: {
    selection
  },
  data: () => {
    return {
      selections: [
        {
          id: 1,
          name: "Frais 1Kg",
          img: "images/fraise.png",
          panier: "images/panie.png",
          favorite: "images/liste.png",
          haj: "jhdjf",
          price: {
            bf: 15.00,
            af: 10.00,
          },
        },
        {
          id: 2,
          name: "Fromage Kiri 24 p",
          price: {
            bf: 15.00,
            af: 10.00,
          },
          img: "images/kiri.png",
          panier: "images/panie.png",
          favorite: "images/liste.png",
          haj: "anna"
        },
        {
          id: 3,
          name: "Lait jaouda 1L",
          price: {
            bf: 6.00,
            af: 5.00,
          },
          img: "images/lait.png",
          panier: "images/panie.png",
          favorite: "images/liste.png",
          haj: "dregt"
        },
        {
          id: 4,
          name: "Panzani 500g",
          price: {
            bf: 30.00,
            af: 25.00,
          },
          img: "images/Panzani.png",
          panier: "images/panie.png",
          favorite: "images/liste.png"
        },
        {
          id: 5,
          name: "Poudre Chocolat 500g",
          price: {
            bf: 80.00,
            af: 60.00,
          },
          img: "images/nesquik.jpg",
          panier: "images/panie.png",
          favorite: "images/liste.png"
        },
        {
          id: 6,
          name: "Amande Affilées 250g",
          price: {
            bf: 50.00,
            af: 40.00,
          },
          img: "images/amande effiés.jpg",
          panier: "images/panie.png",
          favorite: "images/liste.png"
        },
        {
          id: 7,
          name: "Oreo bisuit",
          price: {
            bf: 15.00,
            af: 12.00,
          },
          img: "images/oreo.jpg",
          panier: "images/panie.png",
          favorite: "images/liste.png"
        },
        {
          id: 8,
          name: "Pépites chocolat 250 g",
          price: {
            bf: 30.00,
            af: 25.00,
          },
          img: "images/pépites chocolat.png",
          panier: "images/panie.png",
          favorite: "images/liste.png"
        },
        {
          id: 9,
          name: "Sucre en poudre 1Kg",
          price: {
            bf: 20.00,
            af: 15.00,
          },
          img: "images/sucr.jpg",
          panier: "images/panie.png",
          favorite: "images/liste.png"
        }
      ]
    }
  }
}
</script>
