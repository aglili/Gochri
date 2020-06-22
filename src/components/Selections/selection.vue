<template>
  <div class="col-12 col-sm-6 col-md-4 col-lg-3 mb-4">
    <div class="card">
      <img :src="selection.favorite" alt="listes" class="icon" />
        <div class="card-body">
          <img class="card-title" :src="selection.img" />
          <h6 class="card-subtitle mb-2 text-muted"> {{selection.name}} </h6>
          <p class="card-text line text-right mb-0"> {{selection.price.bf}}DH </p>
          <p class="card-text text-right mb-0"> {{selection.price.af}}DH </p>
          <a class="card-link"><img :src="selection.panier" alt="panier" class="panier"></a>
        </div>
    </div>
  </div>
</template>

<script>
export default{
  props: ["selection"],
}
</script>

<style lang="scss" scoped>
$orange: #f3973a;
h6{
    color: #4d4d4d !important;
}
p{
  font-size: 18px;
  color: $orange;
  cursor: context-menu;
}
.mb-4:last-child, .my-4:last-child {
  display: none;
}
.card-link{
  width: 100px;
  cursor: pointer;
}
.icon{
  position: absolute;
  right: 13px;
  top: 10px;
  width: 47px;
  cursor: pointer;
}
.panier{
  position: absolute;
  left: 22px;
  width: 30px;
  bottom: 21px;
  background: $orange;
  padding: 5px;
  border-radius: 10px;
  width: 32px;
}
.card-title{
  width: 25vh;
  height: 25vh;
  object-fit: contain;
}
.line{
  text-decoration: line-through;
}
.user {
  background: #fff;
  border: 2 solid $orange;
  width: 100%;
  height: 28vh;
  z-index: 100000;
  position: absolute;
  top: 160px;
  left: 0px;
  display: none;
}
span {
  cursor: pointer;
  position: absolute;
  right: 0;
  font-size: 18px;
  background: red;
  padding: 1px 12px;
  color: white;
  border-radius: 5px;
}
.card-img-top {
  margin-left: 85px;
  width: 9rem;
}


 @media (max-width: 991px) {
   .mb-4:last-child, .my-4:last-child {
     display: block;
   }
}
 @media (max-width: 767px) {
   .mb-4:last-child, .my-4:last-child {
     display: none;
   }
}
</style>
