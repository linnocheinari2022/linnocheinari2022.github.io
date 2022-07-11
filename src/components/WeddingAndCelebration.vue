<template>
  <div class="wedding-and-celebration" id="whenandwhere">
    <h2>Vigsel och firande</h2>
    <div class="wedding-and-celebration--content w-70">
      <div class="wedding">
        <img src="../assets/rings-wedding-light.svg" class="p-margin" />
        <p class="p-margin f-18"><strong>Vigsel</strong></p>
        <p class="p-margin">Kl 16.00</p>
      </div>
      <div class="mingle">
        <img src="../assets/champagne-glasses-light.svg" class="p-margin" />
        <p class="p-margin f-18"><strong>Mingel</strong></p>
        <p class="p-margin">Efter vigseln</p>
      </div>
      <div class="dinner">
        <img src="../assets/plate-utensils-light.svg" class="p-margin" />
        <p class="p-margin f-18"><strong>Middag</strong></p>
        <p class="p-margin">Kl 18.00</p>
      </div>
      <div class="party">
        <img src="../assets/party-horn-light.svg" class="p-margin" />
        <p class="p-margin f-18"><strong>Fest!</strong></p>
        <p class="p-margin party--p">
          Efter middag
          <img class="arrow" src="../assets/arrow-right-long-light.svg" /> Sent
        </p>
      </div>
    </div>
  </div>
</template>

<style scoped lang="scss">
.wedding-and-celebration {
  background-color: #02211b;
  padding: 55px;
  padding-bottom: 65px;
  color: white;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;

  &--content {
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    flex-direction: row;
    justify-content: space-between;
    margin-top: 30px;
    margin-bottom: 20px;
    padding: 0;
    grid-gap: 60px;

    @media (min-width: 1024px) {
      grid-template-columns: repeat(4, 1fr);
      margin-top: 40px;
    }
  }
}

img {
  height: 50px;
}

.arrow {
  height: 15px;
  padding: 0 0 0 7px;
}

h2 {
  margin-bottom: 50px;
  margin-top: 10px;

  @media (min-width: 1024px) {
    margin-top: unset;
  }
}

.party {
  &--p {
    display: flex;
    align-items: center;
    justify-content: center;
  }

  .arrow {
    padding: 0 7px;
  }
}

.p-place {
  margin-bottom: 8px;

  &--adress {
    margin-bottom: 20px;
  }
}
</style>
