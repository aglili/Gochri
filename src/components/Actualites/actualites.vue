<template>
  <div class="container">
    <h1>Nos actualités</h1>
    <div class="row">
      <actualite
      v-for="actualite in actualites"
      :key="actualite.id"
      :actualite="actualite" />
    </div>
  </div>
</template>

<script>
import actualite from "@/components/Actualites/actualite.vue";
export default {
  components: {
    actualite
  },
  data: () => {
    return {
      actualites: [
        {
        id: 1,
        img: "images/Jus_bio.jpg",
        alt: "Card image cap",
        parag: "Faites le plein d'énergie",
        lien: "#"
        },
        {
        id: 2,
        img: "images/image.jpg",
        alt: "Card image cap",
        parag: "Le plaisir d'une petite pause de gourmandise",
        lien: "#"
        },
        {
        id: 3,
        img: "images/chocolat.jpg",
        alt: "Card image cap",
        parag: "Pour les enfants",
        lien: "#"
        },
        {
        id: 4,
        img: "images/viande.jpg",
        alt: "Card image cap",
        parag: "Un régal pour tous",
        lien: "#"
        },
        {
        id: 5,
        img: "images/fromage.png",
        alt: "Card image cap",
        parag: "A consommer avec passion",
        lien: "#"
        },
        {
        id: 6,
        img: "images/bio.jpg",
        alt: "Card image cap",
        parag: "100% BIO",
        lien: "#"
        },
      ]
    };
  }
};
</script>
