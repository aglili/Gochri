<template>
  <div class="container bg-light">
    <div class="row">
      <div class="col-md-4 pb-2">
        <img alt="computer" src="@/assets/pc.png" />
        <p>Je sélectionne mes produit</p>
      </div>
      <div class="col-md-4 pb-2">
        <img alt="panier" src="@/assets/panier.png" class="panier" />
        <p>Je valide ma commande</p>
      </div>
      <div class="col-md-4 pb-2">
        <img alt="home" src="@/assets/home.png" class="home" />
        <p>Je récupére mes courses</p>
      </div>
    </div>
  </div>
</template>
<script></script>

<style lang="scss" scoped>
$orange: #f3973a;

.container {
  border-radius: 15px;
  margin-top: 3%;
  padding-top: 1rem;

  .row {
    align-items: center;
    .panier {
      width: 17%;
    }
    img {
      width: 15%;
    }
    p {
      color: $orange;
      font-size: 14px;
    }
  }
}
</style>
