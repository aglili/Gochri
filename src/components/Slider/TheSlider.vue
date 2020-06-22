<template>
  <div class="container-fluid">
    <div class="row">
      <div class="col">
    <h3>Fait vos courses en ligne</h3>
    <input type="submit" class="btn bg-white hover:white" name="text" value="Je me connect">
    <!-- <button class="btn btn-outline-success" type="button">Main button</button> -->
  </div>
    </div>
  </div>
</template>


<style lang="scss" scoped>
 $white: #fff;
 $orange: #f3973a;
 .container-fluid{
   background-image: url(../../assets/header.png);
   background-position: center;
   background-repeat: no-repeat;
   background-size: cover;
   width: 100%;
   height: 100vh;
   position: relative;
   overflow-x: hidden;
 }
 .row{
   text-align: center;
   position: absolute;
   top: 50%;
   left: 50%;
   transform: translate(-10%, -50%);
 }
  h3{
    font-size: 45px;
    color: $white;
  }
  .btn{
    color: $orange;
    font-weight: 600;
  }
  .btn:hover {
  color: $white;
  background-color: $orange !important;
 }
 @media (max-width: 995px) {
     h3 {
     font-size: 35px;
   }
   .container-fluid {
    height: 62vh;
  }
 }
 @media (max-width: 884px) {
   h3 {
       font-size: 30px;
   }
 }
 @media (max-width: 663px) {
   h3 {
       font-size: 25px;
   }
 }
 @media (max-width: 553px) {
   .row {
    text-align: center;
    position: absolute;
    top: 30%;
    left: 43%;
    transform: translate(-2%, 4%);
  }
 }
 @media (max-width: 493px) {
   .row {
    left: 31%;
  }
 }
 @media (max-width: 493px) {
   .row {
    left: 31%;
  }
  .container-fluid {
      width: 110%;
  }
 }
 @media (max-width: 263px) {
   .row {
    left: 10%;
  }
 }
</style>
