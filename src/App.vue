<template>
  <div id="app">
    <MainPageHeader></MainPageHeader>
    <FootballPlayers :players="players"></FootballPlayers>
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
  data() {
    return {
      players: [
        {
          name: "Heung-Min Son",
          location: "Chuncheon, South Korea",
          position: "Striker",
          show: false,
        },
        {
          name: "Richarlison",
          location: "Nova Venecia, Brazil",
          position: "Striker",
          show: false,
        },
        {
          name: "James Maddison",
          location: "Coventry England",
          position: "Playmaker",
          show: false,
        },
        {
          name: "Guglielmo Vicario",
          location: "Udine, Italy",
          position: "Goalkeeper",
          show: false,
        },
        {
          name: "Cristian Romero",
          location: "Cordoba, Argentina",
          position: "Defender",
          show: false,
        },
        {
          name: "Dejan Kulusevski",
          location: "Stockholm, Sweden",
          position: "Left Winger",
          show: false,
        },
      ],
    };
  },
};
</script>

<style></style>
