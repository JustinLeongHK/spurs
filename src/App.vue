<template>
  <div id="app">
    <MainPageHeader></MainPageHeader>
    <FootballPlayers></FootballPlayers>
  </div>
</template>

<script>
import MainPageHeader from "./components/MainPageHeader.vue";
import FootballPlayers from "./components/FootballPlayers.vue";

export default {
  name: "App",
  components: {
    MainPageHeader,
    FootballPlayers,
  },
};
</script>

<style></style>
