<template>
  <div class="main-screen">
    <div class="top">

    </div>
  </div>
</template>

<script>
export default {
  name: 'app'
}
</script>

<style scoped>

  .main-screen {
    display: flex;
    background: linear-gradient(goldenrod, greenyellow);
    position: absolute;
    min-width: 760px;
    min-height: 400px;
   }

  .top {
    background: linear-gradient(seagreen, springgreen);
    width: 100%;
    height: 100px;
    top: 0;
    min-height: 70px;
  }
</style>
