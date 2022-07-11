<template>
  <div class="place">
    <div class="place-container">
      <div class="w-100 place-container--image">
        <img src="../assets/skaftogarden.jpg" alt="Skaftögården" />
      </div>
      <div class="place-container--text">
        <h2>Skaftögården</h2>
        <p class="p-margin">
          Bröllopet och festen sker på Skaftögården i Fiskebäckskil (1,5 timme
          norr om Göteborg).
        </p>
        <p class="p-margin p-place--adress">Skaftö, 451 78 Fiskebäckskil</p>
        <a
          href="https://www.google.com/maps/place/Skaft%C3%B6g%C3%A5rden/@58.2569239,11.4774405,17z/data=!3m1!4b1!4m5!3m4!1s0x4645a19a971b5e9b:0x59e8491cbb07a7f6!8m2!3d58.2569211!4d11.4796292"
          >Se på karta
          <img class="arrow" src="../assets/arrow-right-long-light.svg" />
        </a>
      </div>
    </div>
  </div>
</template>

<style scoped lang="scss">
.place {
  background-color: #02211b;
  &-container {
    display: flex;
    position: relative;

    &--image {
      img {
        filter: grayscale(100%);
        width: 100%;
        object-fit: cover;
        height: 80vh;
      }
    }

    &--text {
      background-color: #02211b;
      color: white;
      padding: 45px;
      padding-bottom: 55px;
      position: absolute;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -50%);
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;

      @media (min-width: 1024px) {
        width: 25%;
      }
    }
  }
}

h2 {
  margin-top: 0;
}

a {
  color: white;
  font-family: "Nunito", sans-serif;
  display: flex;
  align-items: center;
  text-decoration: none;
  padding: 10px 18px;
  border: 1px solid white;
  font-size: 14px;
  border-radius: 35px;
  width: fit-content;
  transition: all 0.2s ease-in-out;

  &:hover {
    transform: scale(1.1);
  }
}

.arrow {
  height: 15px;
  padding: 0 0 0 7px;
}
</style>
