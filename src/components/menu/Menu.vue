/* eslint-disable */
<template>
  <nav class="navbar navbar-expand-lg navbar-light">
    <NavbarMenu />

<!-- logo -->
    <a class="navbar-brand" href="#">
      <img alt="logo" src="@/assets/logo.png" class="logo" />
    </a>

<!-- search -->
  <div class="collapse navbar-collapse" id="navbarSupportedContent">
    <form class="form-inline my-2">
      <input class="form-control search mr-sm-0" type="search" placeholder="Recherche..." aria-label="Search">
          <div class="text-center">
              <i class="fas fa-search mr-1"></i>
          </div>
    </form>
  </div>

<!-- user -->
  <ul class="navbar-nav">
    <router-link to="/" tag="li" class="nav-item active" exact>
      <a class="nav-link" @click="user">
        <img alt="compte" class="icon1" src="@/assets/user.png" />
        <br/> Compte </a>

<!-- modal for user -->
  <form class="user" autocomplete="on">
      <span class="sign" @click="sign"><i class="fas fa-times"></i></span>
    <div class="form-group mt-3">
      <h3>Accéder à votre compte</h3>
      <p>Connectez-vous pour retrouver tous vos services</p>
     <input type="email" class="form-control user-modal" id="exampleInputEmail1" aria-describedby="emailHelp" placeholder="Adresse e-mail">
    </div>
    <div class="form-group">
     <input type="password" class="form-control user-modal" id="exampleInputPassword1" placeholder="Mot de Passe" autocomplete="oof" required>
    </div>
    <div class="connect">
    <p>Se Connecter avec :</p>
    <a href= "#"><img src="@/assets/facebook1.png" alt="facebook" class="facebook"></a>
    <a href= "#"><img src="@/assets/google.png" alt="google" class="google"></a>
    </div>
    <button type="submit" class="btn my-2">Connecter</button>
  <div class="form">
    <div class="form">
    <a href="#">J’ai oublié mon mot de passe</a>
    </div>
  <h5>Vous n’avez pas encore un compte ?</h5>
  <a href="#">Créer mon compte</a>
  </div>
  </form>
    </router-link>

<!-- favorite product -->
    <router-link to="#" tag="li" class="nav-item active">
      <a class="nav-link">
        <img alt="listes" class="icon2" src="@/assets/liste.png" /><br/>
        Listes
      </a>
    </router-link>

<!-- panier -->
    <router-link to="#" tag="li" class="nav-item active">
      <a class="nav-link">
        <img alt="panier" class="icon3" src="@/assets/basket.png" /><br/>
        Panier
      </a>
    </router-link>
  </ul>

</nav>
</template>

<script>
import NavbarMenu from "@/components/menu/NavbarIcon/NavbarMenu.vue";
export default {
  name: "Menu",
  components: {
    NavbarMenu
  },
  methods: {
   user: function() {
    let element = document.querySelector('.user');
    element.style.display="block";
  },

   sign: function() {
    let sign = document.querySelector('.user');
    sign.style.display="none";
  },
 }
};
</script>

<style lang="scss" scoped>
$white: #fff;
$orange: #f3973a;
nav{
  width: 100%;
  background: $white;
}
.logo{
  width: 90px;
  align-items: center;
}
li{
  font-size: 12px;

  .icon1,
  .icon2{
    width: 40px;
  }
  .icon3{
    width: 28px;
  }
}

.search {
  width: 415px !important;
  border-color: $orange;
  border-radius: 19px 0 0 19px;
}

.search:focus,
input {
  border-color: $orange;
  box-shadow: none!important;
}
.text-center{
  background: $orange;
  padding: 7px 12px;
  color: #fff;
  border-radius: 0 19px 19px 0;
}
.fa-search{
  font-size: 17px;
}
.menu{
    cursor: pointer;
}
.navbar-brand{
  margin-right: 20%;
}
.collapse:not(.show) {
    display: block !important;
}
.user {
  border-radius: 13px;
  background: $white;
  padding: 30px;
  width: 22rem;
  position: absolute;
  z-index: 10000;
  right: 7px;
  top: 76px;
  border-color: $orange;
  border: 1px solid $orange;
  display: none;
  position: fixed;
}
.sign {
  background: $orange;
  color: $white;
  font-size: 20px;
  position: absolute;
  top: 3px;
  right: 5px;
  cursor: pointer;
  padding: 1px 8px;
  border-radius: 7px;
}
.fa-times {
  transition: .2s;
}
.fa-times:hover {
  transform: rotate(88deg);
}
.user-modal{
  border-radius: 1rem;
}
h3 {
  color: $orange;
  font-size: 18pt;
  font-weight: bold;
}
h5 {
  color: $orange;
  font-size: 12pt;
  font-weight: bold;
  padding-top: 38px;
}
p {
  padding-bottom: 7px;
}
.connect {
  padding-bottom: 1rem;
}
.connect img {
  height: 43px;
  width: 34px;
  object-fit: contain;
}
.connect .facebook {
  width: 20px;
  margin-right: 10px;
}
.google {
  width: 34px;
  margin-left: 10px;
}
.form a {
  color: $orange;
  padding: 15px;
}
.btn {
  background: $orange;
  color: $white;
  border-radius: 17px;
}
.btn:hover {
  background: $white;
  border-color: $orange;
  color: $orange;
}


// media queries

@media (max-width: 1180px) {
  .navbar-brand {
    margin-right: 15%;
}
}


@media (max-width: 1001px) {
  .navbar-brand {
    margin-right: 10%;
}
}


@media (max-width: 991px) {
  .navbar-nav {
    right: 71px;
    position: absolute;
    display: -webkit-inline-box;
    top: 2px;
  }
  .logo {
    position: absolute;
    left: 81px;
    top: 9px;
  }
  .mb-2, .my-2 {
    margin-left: 20%;
  }
  .mt-2, .my-2 {
    margin-top: 1.5rem !important;
  }
  li{
    padding-right: 14%;
  }
  li:last-child{
    padding-right: 0;
  }
  .search {
    width: 505px !important;
  }
}

// design search
@media (max-width: 930px) {
  .mb-2, .my-2 {
    margin-left: 18%;
  }
}


@media (max-width: 740px) {
  .mb-2, .my-2 {
    margin-left: 12%;
  }
}


@media (max-width: 680px) {
  .mb-2, .my-2 {
    margin-left: 8%;
  }
}


@media (max-width: 640px) {
  .mb-2, .my-2 {
    margin-left: 4%;
  }
}


@media (max-width: 610px) {
  .search {
    width: 465px !important;
  }
}


@media (max-width: 604px) {
  .search {
    width: 455px !important;
  }
}


@media (max-width: 560px) {
  .search {
    display: none;
  }
  .text-center {
    display: none;
  }
}


@media (max-width: 471px) {
  .mb-2, .my-2 {
    margin-left: 0%;
  }
}
@media (max-width: 493px) {
  .mb-2, .my-2 {
    margin-left: 0%;
  }
}


@media (max-width: 493px) {
  .mb-2, .my-2 {
    margin-left: 0%;
  }
.navbar-nav {
    right: 27px;
  }
}


@media (max-width: 487px) {
  .mb-2, .my-2 {
    margin-left: 0%;
  }
.navbar-nav {
    right: 27px;
  }
}

@media (max-width: 377px) {
  li {
      padding-right: 4%;
  }
}


@media (max-width: 360px) {
  .logo {
    left: 61px;
  }
  .navbar-nav {
    right: 0;
  }
}


@media (max-width: 292px) {
  .navbar-nav{
    display: none;
  }
}
</style>
