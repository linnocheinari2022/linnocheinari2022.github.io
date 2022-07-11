<template>
  <div class="home">
    <Hero />
    <WeddingAndCelebration />
    <PlaceComponent />
    <AccomodationComponent />
    <DressCode />
    <MoreInfo />
    <RsvpComponent />
    <OlliImg />
  </div>
</template>

<script>
import Hero from "@/components/HeroComponent.vue";
import WeddingAndCelebration from "@/components/WeddingAndCelebration.vue";
import PlaceComponent from "@/components/PlaceComponent.vue";
import AccomodationComponent from "@/components/AccomodationComponent.vue";
import DressCode from "@/components/DressCode.vue";
import MoreInfo from "@/components/MoreInfo.vue";
import RsvpComponent from "@/components/RsvpComponent.vue";
import OlliImg from "@/components/OlliImg.vue";

export default {
  name: "HomeView",
  components: {
    Hero,
    WeddingAndCelebration,
    PlaceComponent,
    AccomodationComponent,
    DressCode,
    MoreInfo,
    RsvpComponent,
    OlliImg,
  },
};
</script>
