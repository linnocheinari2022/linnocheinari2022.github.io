<template>
  <div class="dresscode" id="dresscode">
    <div class="dresscode-container w-70">
      <div class="dresscode-text">
        <div class="dresscode-text--container">
          <h2>Klädsel</h2>
          <p>
            Klädsel är avslappnat, tänk... midsommar. T.ex. nån snygg skorta och
            chinos, eller nån fin sommarklänning. (Vi vill att ni ska vara
            bekväma) Nånting sommrigt!
          </p>
        </div>
      </div>
      <div class="dresscode-images">
        <img src="../assets/dresscode.png" alt="Dresscode" />
        <img src="../assets/women.jpg" alt="Women with dresses" />
        <img src="../assets/men.jpg" alt="Mens clothing" />
        <img src="../assets/women2.jpg" alt="Women with dresses" />
        <img src="../assets/men2.jpg" alt="Mens clothing" />
      </div>
      <div class="dresscode-image-slider">
        <ImageSlider />
      </div>
    </div>
  </div>
</template>

<script>
import ImageSlider from "./ImageSlider.vue";
import { defineComponent } from "vue";

export default defineComponent({
  components: {
    ImageSlider,
  },
});
</script>

<style scoped lang="scss">
.dresscode {
  display: flex;
  align-items: center;
  justify-content: center;

  &-text {
    display: grid;
    grid-template-columns: 1fr;
    margin-bottom: 50px;

    @media (min-width: 1024px) {
      grid-template-columns: 1fr 1fr;
    }
  }

  &-images {
    grid-template-columns: 1fr 1fr 1fr 1fr 1fr;
    grid-gap: 30px;
    display: none;

    @media (min-width: 1024px) {
      display: grid;
    }
  }

  &-image-slider {
    @media (min-width: 1024px) {
      display: none;
    }
  }
}

h2 {
  text-align: left;
  margin-top: 0;
}

p {
  text-align: left;
}

img {
  height: 330px;
  width: 100%;
  object-fit: cover;
  -webkit-transition: all 0.5s ease-in-out;
  -moz-transition: all 0.5s ease-in-out;
  -o-transition: all 0.5s ease-in-out;
  transition: all 0.5s ease-in-out;
  filter: grayscale(100%);

  &:hover {
    transform: scale(1.3);
    cursor: pointer;
    filter: grayscale(0%);
    z-index: 4;
  }
}
</style>
