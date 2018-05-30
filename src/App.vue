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

<<<<<<< HEAD
  .main-screen {
    background: linear-gradient(#fb3, #58a);
=======
  .main {
>>>>>>> 12ca7e9f1147230d74404656bab65ceabb8db294
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
<<<<<<< HEAD
    background: #ccc;
    width: 100%;
    height: 100px;
    top: 0;
  }

  .search-icon-area {
    background: #ccc;
    width: 100px;
    height: 100%;
    position: relative;
    left: 100px;
  }

  .icon-search {
    color: linen;
    left: 10%;
    top: 10%;
    margin-right: -50%;
    position: relative;
=======
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
>>>>>>> 12ca7e9f1147230d74404656bab65ceabb8db294
  }


</style>
