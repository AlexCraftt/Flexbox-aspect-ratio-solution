<template>
  <!DOCTYPE html>
  <html lang="en">
    <head>
      <meta charset="UTF-8">
      <meta name="viewport" content="width=device-width, initial-scale=1.0">
      <meta http-equiv="X-UA-Compatible" content="ie=edge">
      <title>Адаптивная верстка</title>
    </head>
    <body>
      <section>
        <div class="wrapper">
          <div class="row rel">
            <div class="rel__offset"></div>
            <div class="rel__content">
              <div class="big">0</div>
              <div class="product product1">
                <div class="item item1">1</div>
                <div class="item item2">2</div>
                <div class="item item3">3</div>
              </div>
              <div class="product product2">
                <div class="item item4">4</div>
                <div class="item item5">5</div>
                <div class="item item6">6</div>
              </div>
            </div>

          </div>
        </div>
      </section>
    </body>
  </html>
</template>

<script>
export default {
  name: 'app'
}

</script>

<style>
html, body {
    background: cornsilk;
    margin: 0;
}

.rel{
    position: relative;
}

.rel__offset{
    height: 0;
}

.rel__offset-1-1{
    padding-top: 100%;
}

.rel__offset-16-9{
    padding-top: 56.25%;
}

.rel__offset-3-2{
    padding-top: 67%;
}

.rel__content{
    position: absolute;
    width: 100%;
    height: 100%;
    top: 0;
    left: 0;
    display: flex;
    flex-wrap: wrap;
    flex-direction: column;
}

.wrapper{
    /* max-width: 1280px; */
    width: auto;
    margin: 0 auto;
    /* padding: 0 30px; */
}

.row{
    border: 1px solid #f90;
}

.row .rel__offset{
    padding-top: 56.25%;
}

.big{
    background: #f4d058;
    flex: 1 1 100%;
    width: 60%;
    align-items: center;
}

.product{
    flex: 1 1 100%;
    width: 20%;
    display: flex;
    flex-direction: column;
}

.product1{
    order: -1;
}

.item{
    flex: 1 1 20%;
    height: calc(50% - 30px);
    background-size: cover;
    display: flex;
    align-items: center;
    justify-content: center;
}

.item1{
    background-image: url(assets/img/001.jpg);
}

.item2{
    background-image: url(assets/img/002.jpg);
}

.item3{
    background-image: url(assets/img/003.jpg);
}

.item4{
    background-image: url(assets/img/004.jpg);
}

.item5{
    background-image: url(assets/img/005.jpg);
}

.item6{
    background-image: url(assets/img/006.jpg);
}

@media screen and (max-width: 992px){
    .row .rel__offset{
        padding-top: 100%;
    }
    
    .big{
        width: 80%;
    }
    
    .product{
        flex: 1 1 20%;
    }
    
    .product1{
        order: 0;
    }
}

@media screen and (max-width: 600px){
    .row .rel__offset {
        display: none;
    }

    .rel__content{
        flex-wrap: nowrap;
        position: static;
    }

    .big, .product{
        width: auto;
    }
}
</style>


