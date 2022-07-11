<template>
  <div class="hero" id="hero">
    <div class="parallax">
      <p class="f-18">Välkommen till vigseln mellan</p>
      <h1 class="hero-desktop-header">Linn & Einari</h1>
      <div class="hero-mobile-header">
        <h1 class="header-1">Linn</h1>
        <h2>&</h2>
        <h1>Einari</h1>
      </div>
      <p class="f-18">3 september 2022</p>
      <img class="arrow" src="../assets/arrow-right-long-light.svg" />
    </div>
  </div>
</template>

<style scoped lang="scss">
h1 {
  font-size: 110px;
  margin: 0px;
  font-weight: 500;

  @media (min-width: 1024px) {
    margin: 20px;
    font-size: 115px;
  }
}

h2 {
  color: white;
  margin: 0;
  font-size: 55px;

  @media (min-width: 1024px) {
    margin: 20px;
  }
}

.hero {
  color: white;

  &-desktop-header {
    display: none;

    @media (min-width: 1024px) {
      display: block;
    }
  }

  &-mobile-header {
    line-height: 1;
    margin: 45px;

    .header-1 {
      margin-bottom: 20px;
    }

    @media (min-width: 1024px) {
      display: none;
    }
  }
}

.arrow {
  transform: rotate(90deg);
  margin-top: 50px;
  height: 28px;

  @media (min-width: 1024px) {
    display: none;
  }
}

.parallax {
  padding-bottom: 40px;
  padding-top: 50px;
  width: 100%;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  background-image: url("../assets/forest.jpg");
  min-height: 550px;
  background-attachment: fixed;
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;

  @media (min-width: 1024px) {
    padding-top: 75px;
    padding-bottom: 0px;
  }
}
</style>
