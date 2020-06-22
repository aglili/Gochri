<template>
  <div class="d-flex mb-3">
    <div class="anna">
      <div class="card col" style="width: 12rem;">
      <div class="card-body">
        <a :href="promotion.url">
          <img class="card-title" :src="promotion.img" />
        </a>
      </div>
    </div>
    <h3 class="mt-2"> {{promotion.name}}</h3>
    <b> {{promotion.price}}DH </b>
  </div>
</div>

</template>
<script>
export default{
  props: ['promotion']
}
</script>
<style lang="scss" scoped>
$orange: #f3973a;


h3 {
  font-size: 1rem;
}
b{
  color: $orange;
  cursor: context-menu;
}

img{
  width: 100px;
  height: 20vh;
  object-fit: contain;
}
</style>
