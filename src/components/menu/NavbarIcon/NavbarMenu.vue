<template>
  <!-- icon navbar -->
    <div class="wrapper pr-4">
      <span @click="menu">
          <i class="fas fa-bars"></i>
      </span>
      <div id="sidebar">
        <ul class="list-unstyled components">
          <li class="active"
          v-for="product in products"
          :key="product.id">
          <a href="#">
            <img :src="product.img">
            <label>
            {{product.name}}
          </label>
          </a>
          </li>
        </ul>
      </div>
  </div>
</template>

<script>
export default {
  data: function() {
    return {
      products: [
        {
          id: 1,
          img:"images/fruits.png",
          name:"Fruits et légumes",
        },
        {
          id: 2,
          img:"images/pains.png",
          name:"Pains"
        },
        {
          id: 3,
          img:"images/épicerir.png",
          name:"Epicerie salée"
        },
        {
          id: 4,
          img:"images/viande1.png",
          name:"Viandes et poissons"
        },
        {
          id: 5,
          img:"images/chocolat.jpg",
          name:"chocolat"
        }
      ]
    }
  },
  methods: {
  menu: function() {
    document.getElementById('sidebar').classList.toggle('active');
}
}
}
</script>
<style lang="scss" scoped>
$white: #fff;
$orange: #f3973a;
$lightOrng: #f3973ae3;

.fa-bars{
  font-size: 20px;
  color: $orange;
  cursor: pointer;
  font-size: 32px;
}
.fa-bars:hover {
  color: #e88017;
}
#sidebar {
  width: 18rem;
  background: #fff;
  position: absolute;
  left: -288px;
  top: 76px;
  border-radius: 14px;
  border: 0.01px solid $orange;
  z-index: 100;
  transition: .2s;
}
#sidebar.active {
  left: 2px;
}


ul {
  margin-bottom: 0rem;
}
li {
  padding: 13px;
  text-align: center;
  border-bottom: 1px solid #88858552;
  list-style: none;
  height: 13vh;
}
li:last-child {
  border-bottom: none;
}
li:hover {
  background: #f3973ab8;
  cursor: pointer;
}
li:first-child:hover {
  border-radius: 14px 14px 0 0;
}
li:last-child:hover {
  border-radius: 0px 0px 14px 14px;
}
a {
  color: #474749;
}
a:hover {
  color: #474749;
  text-decoration: none;
}
img {
  width: 66px;
  float: left;
  text-align: center;
}
span {
  text-align: center;
}
label {
  position: relative;
  top: 18px;
  font-size: 18px;
  cursor: pointer;
}


@media (max-width: 991px) {
  .sidebar {
  top: 56px;
  }
}
</style>
