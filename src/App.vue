<template>
  <div class="main-screen">
    <div class="top">
      <div class="search-icon-area">
          <i class="fa fa-search icon-search fa-6x"></i>
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

  .main-screen {
    background: linear-gradient(#fb3, #58a);
    position: absolute;
    top: 0;
    bottom: 0;
    left: 0;
    right: 0;
    min-width: 760px;
  }

  .top {
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
  }
</style>
