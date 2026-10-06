<script setup>
import Navbar from './components/Navbar.vue';
import Footbar from './components/Footbar.vue';
import GameButton from './components/GameButton.vue';
</script>

<template>
  <Navbar></Navbar>
  <main>

    <div class="game-grid-container">
      <GameButton class="game-grid-item"/>
      <GameButton class="game-grid-item"/>
      <GameButton class="game-grid-item"/>
      <GameButton class="game-grid-item"/>
      <GameButton class="game-grid-item"/>
      <GameButton class="game-grid-item"/>
      <GameButton class="game-grid-item"/>
      <GameButton class="game-grid-item"/>
      <GameButton class="game-grid-item"/>
      <GameButton class="game-grid-item"/>
      <GameButton class="game-grid-item"/>
      <GameButton class="game-grid-item"/>
    </div>

    <div style="margin-top: auto;">
      <Footbar></Footbar>
    </div>
  </main>
</template>


<style>
main {
  display: flex;
  flex: 1;
  flex-direction: column;
  min-width: 0;
  min-height: 0;
  overflow-y: auto;
}

.game-grid-container {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
  margin-top: 18px;
  gap: 12px;
}

.game-grid-item {
  text-align: center;
}

</style>