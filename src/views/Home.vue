 <template>
  <div class="home">
    <Menu />
    <TheSlider />
    <AfterSlider />
    <actualites />
    <rayons />
    <selections />
    <promos />
    <BeforeFooter />
    <TheFooter />
  </div>
</template>

<script>
// @ is an alias to /src
import Menu from "@/components/menu/Menu.vue";
import TheSlider from "@/components/Slider/TheSlider.vue";
import AfterSlider from "@/components/Slider/AfterSlider.vue";
import actualites from "@/components/Actualites/actualites.vue";
import rayons from "@/components/Rayons/rayons.vue";
import selections from "@/components/Selections/selections.vue";
import promos from "@/components/Promotions/promos.vue";
import BeforeFooter from "@/components/footer/BeforeFooter.vue";
import TheFooter from "@/components/footer/TheFooter.vue";

export default {
  name: "Home",
  components: {
    Menu,
    TheSlider,
    AfterSlider,
    actualites,
    rayons,
    selections,
    promos,
    BeforeFooter,
TheFooter  }
};
</script>
