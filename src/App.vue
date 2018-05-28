<template>
  <div class="main">
    <div class="container">
      <div class="top">

      </div>
    </div>
    
  </div>
</template>

<script>
export default {
  name: 'app'
}
</script>

<style scoped>

  .main {
    position: absolute;
    top: 0;
    bottom: 0;
    left: 0;
    right: 0;
    background: #fde152;
  }

  .container{
    display: flex;
    flex-direction: column;
    flex-wrap: wrap;
    min-width: 100%;
  }

  .top {
    display: flex;
    background: #ff9d00;
    align-self: flex-start;
    min-width: 100%;
    height: 70px;
    top: 0;
  }
</style>
