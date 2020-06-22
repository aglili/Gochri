<template>
    <div class="d-flex">
      <div class="col ml-1 pb-4">
        <div class="card">
        <a class="text-dark" :href="rayon.url">
         <img alt="fruits" :src="rayon.img" />
        <p> {{rayon.parag}} </p>
        </a>
        </div>
      </div>
    </div>
</template>

<script>
export default {
  props: ["rayon"]
};
</script>

<style lang="scss" scoped>
$orange: #f3973a;
$white: #fff;
$black: #2c3e50;

  .row{

    .card {
      width: 11rem;
    }
  img{
    height: 17vh;
    object-fit: cover;
    padding: 10px;
  }
  a{
    font-size: 12px;
    cursor: poinetr;
  }
  a:hover {
    text-decoration: none;
  }
  .card:hover {
    cursor: pointer;
  }
}
</style>
