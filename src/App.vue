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
    background: #fde152;
    position: absolute;
    top: 0;
    bottom: 0;
    left: 0;
    right: 0;
    min-width: 760px;
  }

  .top {
    background: #ff9d00;
    width: 100%;
    height: 100px;
    top: 0;
  }

  .search-icon-area {
    background: #ff7b00da;
    width: 100px;
    height: 100%;
    position: relative;
    left: 100px;
  }

  .icon-search {
    color: #ff5100;
    left: 10%;
    top: 10%;
    margin-right: -50%;
    position: relative;
  }
</style>
