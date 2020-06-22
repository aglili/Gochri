<template>
      <div class="col-md-4 col-sm-6 mb-4">
        <div class="card orange">
          <a :href="actualite.url">
          <img class="card-img-top" :src="actualite.img" :alt="actualite.alt" />
          <div class="card-body">
            <p class="card-text"> {{actualite.parag}} </p>
          </div>
          </a>
        </div>
      </div>
</template>

<script>
export default {
  props: ["actualite"]
};
</script>

<style lang="scss" scoped>
.col-md-4{

  img{
    width: 100%;
    height: 13vw;
    object-fit: cover;
  }
  .card{
    height: 21vw;
    font-size: 15px;
  }
  .card-body {
    padding: 1rem;
}
  a{
    text-decoration: none;
    color: #fff;
    cursor: pointer;
  }
  a:hover{
    color: #fff;
  }
  .orange{
    background: #F39637;
  }
  p {
    font-size: 25px;
  }
}

@media (max-width: 1198px) {
  p {
    font-size: 15px !important;
  }
}

@media (max-width: 880px) {
  .col-md-4 .card {
  height: 28vw;
  }
  .col-md-4 img {
    height: 18vw;
  }
}

@media (max-width: 780px) {
    .col-md-4 .card-body {
    padding: 10px;
 }
}


@media (max-width: 767px) {
  .col-md-4 .card {
  height: 35vw;
  }
  .col-md-4 img {
    height: 25vw;
  }
}


@media (max-width: 650px) {
  p {
    font-size: 13px;
  }
}

@media (max-width: 575px) {
  .col-md-4 .card {
    height: 52vw;
    width: 287px;
    margin: 0 auto;
  }
  .col-md-4 img {
    height: 35vw;
  }
  p {
      font-size: 15px;
  }
}
@media (max-width: 535px) {
  .col-md-4 .card {
    height: 52vw;
    width: 237px;
  }
}

@media (max-width: 365px) {
  .col-md-4 .card {
    height: 58vw;
    width: 209px;
  }
  .h1, h1 {
    font-size: 1.8rem !important;
}
}
</style>
