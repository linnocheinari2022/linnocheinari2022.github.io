<template>
  <Splide :options="{ rewind: true }" aria-label="Kläder - dress code">
    <SplideSlide>
      <img src="../assets/dresscode.png" alt="Dresscode" />
    </SplideSlide>
    <SplideSlide>
      <img src="../assets/women.jpg" alt="Women with dresses" />
    </SplideSlide>
    <SplideSlide>
      <img src="../assets/men.jpg" alt="Mens clothing" />
    </SplideSlide>
    <SplideSlide>
      <img src="../assets/women2.jpg" alt="Women with dresses" />
    </SplideSlide>
    <SplideSlide>
      <img src="../assets/men2.jpg" alt="Mens clothing" />
    </SplideSlide>
  </Splide>
</template>

<script>
import { Splide, SplideSlide } from "@splidejs/vue-splide";
import { defineComponent } from "vue";
import "@splidejs/vue-splide/css";

export default defineComponent({
  components: {
    Splide,
    SplideSlide,
  },
  setup() {
    const options = {
      rewind: true,
      gap: "1rem",
    };

    return { options };
  },
});
</script>

<style scoped lang="scss">
img {
  height: 450px;
  object-fit: cover;
  width: 100%;

  @media (min-width: 1024px) {
    height: 500px;
  }
}
</style>
