<template>
  <div class="content">
    <div
      v-for="(player, index) in players"
      :key="index"
      class="player"
      @click="player.show = !player.show"
    >
      <p class="player_name">{{ player.name }}</p>
      <p>{{ player.location }}</p>
      <p v-show="player.show" class="player_position">{{ player.position }}</p>
    </div>
  </div>
</template>

<script>
export default {
  props: ["players"],
  data() {
    return {};
  },
};
</script>

<style>
.content {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
  margin: 100px 50px;
  gap: 20px;
}

.player {
  height: 150px;
  border: solid;
  border-width: 1px;
  display: flex;
  flex-direction: column;
  text-align: center;
  border-radius: 20px;
  background: grey;
  color: white;
}

.player_name {
  font-size: 20px;
}

p {
  margin-bottom: 10px;
}

.player_position {
  font-weight: bolder;
}
</style>
