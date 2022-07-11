<template>
  <nav>
    <router-link to="#hero">Home</router-link> |
    <router-link to="#whenandwhere">Vigsel och firande</router-link> |
    <router-link to="#accomodation">Boende</router-link> |
    <router-link to="#dresscode">Klädsel</router-link> |
    <router-link to="#moreinfo">Övrig info</router-link> |
    <router-link to="#rsvp">OSA</router-link>
  </nav>
  <router-view />
</template>

<style lang="scss">
#app {
  font-family: "EB Garamond", serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
}

body {
  margin: 0;
  position: relative;
  background-color: #02211b;
}

nav {
  padding: 30px;
  background-color: #02211b;
  color: white;
  position: fixed;
  width: 100%;
  z-index: 10;
  display: none;

  @media (min-width: 1024px) {
    display: block;
  }

  a {
    color: #ffffff;
    text-decoration: none;
    margin: 0 25px;
    width: fit-content;

    // &.router-link-exact-active {
    //   //   color: #42b983;
    //   //   text-decoration: underline;
    //   border-bottom: 1px solid white;
    // }
  }
}

h1,
h2,
h3,
h4,
h5,
h6 {
  font-weight: 600;
}

h2 {
  font-size: 32px;
  color: #e8dbc1;
}

p {
  font-family: "Nunito", sans-serif;
  margin: 0;
  line-height: 25px;
  color: white;
}

.p-margin {
  margin-bottom: 24px;
}

.f-18 {
  font-size: 18px;
}

.w-100 {
  width: 100%;
}

.w-70 {
  width: 100%;
  padding: 55px 30px;
  padding-bottom: 0;

  @media (min-width: 1024px) {
    width: 70%;
    padding: 90px 30px;
    padding-bottom: 0;
  }
}

.w-50 {
  width: 100%;

  @media (min-width: 1366px) {
    width: 50%;
  }
}

.w-30 {
  width: 30%;
}

@import url("https://fonts.googleapis.com/css2?family=Cabin:wght@400;500;600&family=EB+Garamond:ital,wght@0,400;0,500;0,600;0,700;0,800;1,400;1,500;1,600;1,700;1,800&family=Great+Vibes&family=Lato:wght@100;300;400;700&family=Nunito:wght@200;300;400;500;600;800;900&family=Playfair+Display:ital,wght@0,400;0,500;0,600;0,700;0,800;1,400;1,500;1,600;1,700&family=Raleway:wght@300;400;500;600;700;900&family=Roboto:wght@300;400;500;700&display=swap");
</style>
