<template>
  <div class="rsvp" id="rsvp">
    <div class="rsvp-container">
      <div class="rsvp-container--photo-grid">
        <img src="../assets/oss/1.jpg" alt="" />
        <img src="../assets/oss/2.jpg" alt="oss" />
        <img src="../assets/oss/3.jpg" alt="oss" />
        <img src="../assets/oss/4.jpg" alt="oss" />
        <img src="../assets/oss/5.jpg" alt="oss" />
        <img src="../assets/oss/6.png" alt="oss" />
        <img src="../assets/oss/7.jpg" alt="oss" />
        <img src="../assets/oss/9.jpg" alt="oss" />
        <img src="../assets/oss/10.jpg" alt="oss" />
        <img src="../assets/oss/11.jpg" alt="oss" />
        <img src="../assets/oss/12.jpg" alt="oss" />
        <img src="../assets/oss/13.jpg" alt="oss" />
        <img src="../assets/oss/14.jpg" alt="oss" />
        <img src="../assets/oss/15.png" alt="oss" />
        <img src="../assets/oss/16.jpg" alt="oss" />
        <img src="../assets/oss/17.jpg" alt="oss" />
        <img src="../assets/oss/18.jpg" alt="oss" />
        <img src="../assets/oss/19.jpg" alt="oss" />
        <img src="../assets/oss/20.jpg" alt="oss" />
        <img src="../assets/oss/21.jpg" alt="oss" />
        <img src="../assets/oss/22.jpg" alt="oss" />
        <img src="../assets/oss/26.jpg" alt="oss" />
        <img src="../assets/oss/27.jpg" alt="oss" />
        <img src="../assets/oss/28.jpg" alt="oss" />
        <img src="../assets/oss/29.jpg" alt="oss" />
        <img src="../assets/oss/30.jpg" alt="oss" />
        <img src="../assets/oss/32.jpg" alt="oss" />
        <img src="../assets/oss/33.jpg" alt="oss" />
        <img src="../assets/oss/34.jpg" alt="oss" />
        <img src="../assets/oss/36.jpg" alt="oss" />
        <img src="../assets/oss/37.jpg" alt="oss" />
        <img src="../assets/oss/38.jpg" alt="oss" />
        <img src="../assets/oss/39.jpg" alt="oss" />
        <img src="../assets/oss/40.jpg" alt="oss" />
        <img src="../assets/oss/41.jpg" alt="oss" />
        <img src="../assets/oss/42.jpg" alt="oss" />
      </div>
      <div class="rsvp-container--text">
        <h2>OSA</h2>
        <p class="p-margin">
          OSA till Linn så fort som möjligt, men senast 3 augusti (1 månad
          innan) antingen att:
        </p>
        <p class="p-margin-small desktop">
          <strong>Sms:a Linn</strong> - 0702 46 07 29
        </p>
        <p class="p-margin-small mobile">
          <span><strong>Sms:a Linn</strong> -</span>
          <span>0702 46 07 29</span>
        </p>
        <p class="p-margin-small">
          <strong>Skicka meddelande </strong>- på Facebook
        </p>
        <p><strong>Mejla</strong> - linn.tunberg@gmail.com</p>
      </div>
    </div>
  </div>
</template>

<style scoped lang="scss">
.rsvp {
  margin-top: 30px;
  display: flex;
  align-items: center;
  justify-content: center;

  &-container {
    position: relative;

    &--photo-grid {
      display: grid;
      grid-template-columns: repeat(4, 1fr);

      @media (min-width: 1024px) {
        grid-template-columns: repeat(9, 1fr);
      }
    }

    &--text {
      position: absolute;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -50%);
      background-color: #02211b;
      padding: 45px;
      padding-bottom: 55px;

      @media (min-width: 1024px) {
        width: 25%;
      }
    }
  }
}

.mobile {
  display: flex;
  flex-direction: column;
  @media (min-width: 1024px) {
    display: none;
  }
}

.desktop {
  display: none;

  @media (min-width: 1024px) {
    display: block;
  }
}

h2 {
  margin-top: 0;
}

img {
  width: 100%;
  height: 100%;
  object-fit: cover;
  filter: grayscale(100%);
}

.p-margin-small {
  margin-bottom: 20px;

  @media (min-width: 1024px) {
    margin-bottom: 10px;
  }
}
</style>
