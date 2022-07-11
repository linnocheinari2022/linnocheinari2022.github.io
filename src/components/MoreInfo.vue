<template>
  <div class="moreinfo" id="moreinfo">
    <div class="moreinfo-container w-70">
      <h2>Övrig info</h2>
      <div class="moreinfo-container--text">
        <div class="moreinfo-dinner">
          <img src="../assets/fork-knife-light.svg" class="p-margin" />
          <p class="p-margin f-18"><strong>Middag och dryck</strong></p>
          <p>
            Vid eventuella allergier, meddela dessa snarast till Linn i samband
            med OSA. Dryck kommer att finnas på plats, både med alkohol och
            alkoholfritt.
          </p>
        </div>
        <div class="moreinfo-music">
          <img src="../assets/music-light.svg" class="p-margin" />
          <p class="p-margin f-18"><strong>Musik</strong></p>
          <p>
            Vi har skapat en delat Spotify spellista där ni kan lägga till låtar
            som ni vill rocka till under festen (till er som inte vet hur
            Spotify fungerar, fråga någon yngre i eran närhet, hehe).
          </p>
          <a
            href="https://open.spotify.com/playlist/0Xfm1oTLGPLABFZY2fSiwX?si=bfa325e61c7d4649&pt=cd6f8a2a318a85cde12ca8c44e80ee43"
            >Lägg till låtar här!</a
          >
        </div>
        <!-- </div>
      <div class="moreinfo-container--text"> -->
        <div class="moreinfo-children">
          <img src="../assets/baby-light.svg" class="p-margin" />
          <p class="p-margin f-18"><strong>Barn</strong></p>
          <p>
            Vi tycker mycket om barn, men denna dag firar vi enbart i vuxnas
            sällskap. Bebisar som ammas och inte kan lämnas med barnvakt är
            givetvis välkomna.
          </p>
        </div>
        <div class="moreinfo-present">
          <img src="../assets/gifts-light.svg" class="p-margin" />
          <p class="p-margin f-18"><strong>Bröllopspresent</strong></p>
          <p class="p-margin">
            Ni som kan eller vill får gärna bidra till våran bröllopsresa.
            Drömmen är Bora Bora, men vi får se hur långt vi kommer! Kontonummer
            kan vi dela ut vid OSA, annars kan ni swisha till Linn (0702 46 07
            29).
          </p>
          <p>
            Det viktigaste är att ni är där och firar denna dag tillsammans med
            oss!
          </p>
        </div>
      </div>
    </div>
  </div>
</template>

<script></script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.moreinfo {
  display: flex;
  align-items: center;
  justify-content: center;

  &-container {
    padding-bottom: 45px;

    @media (min-width: 1024px) {
      padding-bottom: 75px;
    }

    &--text {
      display: grid;
      grid-template-columns: 1fr;
      margin-top: 50px;
      grid-gap: 50px;

      @media (min-width: 1024px) {
        grid-template-columns: 1fr 1fr 1fr;
        margin-top: 70px;
      }
    }
  }

  &-dinner {
    margin-top: 25px;

    @media (min-width: 1024px) {
      margin-top: 0;
    }
  }

  &-music {
    display: flex;
    flex-direction: column;
    align-items: center;
    margin-top: 25px;

    @media (min-width: 1024px) {
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
      margin-top: 30px;

      &:hover {
        transform: scale(1.1);
      }
    }
  }

  &-children {
    margin-top: 25px;

    @media (min-width: 1024px) {
      margin-top: 0;
    }
  }

  &-present {
    margin-top: 25px;

    @media (min-width: 1024px) {
      grid-column: 1 / -1;
      margin-top: 30px;
    }

    @media (min-width: 1366px) {
      padding: 0 130px;
    }

    @media (min-width: 1920px) {
      padding: 0 250px;
    }
  }
}

h2 {
  margin-top: 10px;

  @media (min-width: 1920px) {
    margin-top: 0;
  }
}

img {
  height: 50px;
}
</style>
