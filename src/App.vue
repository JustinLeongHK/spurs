<template>
  <div id="app">
    <MainPageHeader></MainPageHeader>
    <FootballPlayers></FootballPlayers>
    <page-footer></page-footer>
  </div>
</template>

<script>
import MainPageHeader from "./components/MainPageHeader.vue";
import FootballPlayers from "./components/FootballPlayers.vue";
import PageFooter from "./components/PageFooter.vue";

export default {
  name: "App",
  components: {
    MainPageHeader,
    FootballPlayers,
    PageFooter,
  },
};
</script>

<style></style>
