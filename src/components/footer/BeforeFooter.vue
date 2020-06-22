<template>
  <div class="container-fluid bg-light">
    <div class="row text-center items-center py-3">
      <div class="col-6 mb col-md-3">
        <img src="@/assets/img1.png" alt="casque">
        <h2 class="titre pt-2">Un service client <br/>toujour disponible</h2>
      </div>

      <div class="col-6 mb col-md-3">
        <img src="@/assets/img2.png" alt="camion">
        <h2 class="titre pt-2">Un service livraison<br/>plus étendu</h2>
      </div>

      <div class="col-6 col-md-3">
        <img src="@/assets/img3.png" alt="drive">
        <h2 class="titre pt-2">Un drive axé sur <br/> la fraicheur et la qualité</h2>
      </div>

      <div class="col-6 col-md-3">
        <img class="pt-3" src="@/assets/img4.png" alt="paiment">
        <h2 class="titre pt-2">Un paiment sécurisé <br/>pour vos transactions</h2>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "BeforeFooter"
};
</script>

<style lang="scss" scoped>

    img{
      width: 10vh;
      text-align: center;
    }
    h2{
      font-size: 12px;
      color: #4d4d4d;
    }

    @media (max-width: 767px) {
      .mb {
        margin-bottom: 1.5rem;
      }
      .container-fluid {
        background: #fff !important;
      }
   }
</style>
