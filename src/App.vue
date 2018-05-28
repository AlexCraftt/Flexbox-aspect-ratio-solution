<template>
  <div class="main">
    <div class="container">
      <div class="top">

      </div>
      <div class="first-grid">
        <img class="img1" src="src/assets/img/fxxxjhyyy.jpg" alt="">
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
    flex-direction: row;
    background: #ff9d00;
    align-self: flex-start;
    min-width: 100%;
    height: 70px;
  }

  .first-grid{
    display: flex;
    flex-direction: row;
    flex-wrap: wrap;
    justify-content: space-between;
    background: tomato;
    min-width: 100%;
    height: 350px;
  }

  img1 {
    flex-basis: 30%;
    flex-grow: 1;
  }


</style>
