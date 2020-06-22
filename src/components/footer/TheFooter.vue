<template>
  <footer>
  <div class="container-fluid">
    <div class="row px-2 py-4">
      <div class="col-md-3 pb-5">
        <img src="@/assets/logo.png" alt="logo">
      </div>
      <div class="col-md-3 pb-5">
        <h4>Accueil</h4>
        <p><a href="#">Catégorie</a></p>
        <p><a href="#">Les nouveautés</a></p>
        <p><a href="#">Les promotions</a></p>
      </div>

      <div class="col-md-3 pb-5">
        <h4>Nos service</h4>
        <p><a href="#">Livraison à domicile</a></p>
        <p><a href="#">Livraison standar</a></p>
        <p><a href="#">Livraison express</a></p>
      </div>

      <div class="col-md-3 pb-5">
        <h4>Contacter</h4>
        <p><a href="#">Services clients</a></p>
        <a href="#" class="pr-3 text-left items-left"><i class="fab fa-facebook-f"></i></a>
        <a href="#" class="pr-3 text-left items-left"><i class="fab fa-instagram"></i></a>
        <a href="#" class="pr-3 text-left items-left"><i class="fab fa-youtube"></i></a>
        <a href="#" class="text-left items-left"><i class="fab fa-whatsapp"></i></a>
      </div>

    </div>
  </div>
  <h4 class="phone bg-dark text-white p-2 m-0">
    <i class="fas fa-phone-alt "></i>
    06 25 36 21 25
  </h4>
 </footer>
</template>
<script>
export default {
  name: "TheFooter"
};
</script>

<style lang="scss" scoped>
.container-fluid{
    background: #333333;
    h4 {
      color: #fff;
      cursor: context-menu;
    }
      a{
      color: #fff;
      }
      .text-left {
        font-size: 30px !important;
      }
      img{
        width: 20vh;
      }
}
</style>
