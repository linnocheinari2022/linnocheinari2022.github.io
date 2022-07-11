<template>
  <img src="../assets/olli.png" />
</template>

<script>
export default {
  name: "OlliImg",
};
</script>

<style scoped lang="scss">
img {
  height: 170px;
  position: fixed;
  left: 0;
  bottom: -55px;
  z-index: 1;

  //   &:hover {
  //     animation: grow 5s ease-in-out forwards;
  //     -webkit-animation: grow 5s ease-in-out forwards;
  //     cursor: pointer;
  //   }
}

// @keyframes grow {
//   0% {
//     transform: scale(1);
//     -webkit-transform: scale(1);
//   }
//   100% {
//     transform: scale(5);
//     -webkit-transform: scale(5);
//   }
// }
</style>
