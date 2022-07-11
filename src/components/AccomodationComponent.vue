<template>
  <div class="accomodation" id="accomodation">
    <div class="w-70 accomodation-container">
      <div class="accomodation-image">
        <img src="../assets/boende.jpg" alt="Women with dresses" />
      </div>
      <div class="accomodation-text">
        <h2>Boende</h2>
        <p>
          I lokalen finns det flera rum med sängar (och kuddar och täcken),
          <u>men sängkläder måste ni ta med själva.</u>
        </p>
        <p class="accomodation-text--p">
          Om ni väljer att sova över, meddela detta vid OSA så ordnar vi en
          plats åt dig/er. Det finns dusch i lokalen, dock får ni ta med er
          handduk, duschtvål, etc.
        </p>
      </div>
    </div>
  </div>
</template>

<style scoped lang="scss">
.accomodation {
  background-color: #02211b;
  color: white;
  display: flex;
  align-items: center;
  justify-content: center;

  &-container {
    display: grid;
    grid-template-columns: 1fr;
    justify-content: center;
    grid-gap: 50px;

    @media (min-width: 1024px) {
      grid-template-columns: 1fr 1fr;
    }
  }

  h2 {
    margin-top: 0;
  }

  .w-50 {
    text-align: left;
  }

  &-text {
    text-align: left;
    order: 1;
    &--p {
      margin-top: 20px;
    }

    @media (min-width: 1024px) {
      order: 2;
    }
  }

  &-image {
    overflow: hidden;
    order: 2;

    img {
      height: 350px;
      filter: grayscale(100%);
      width: 100%;
      object-fit: cover;
    }

    @media (min-width: 1024px) {
      order: 1;
    }
  }
}
</style>
