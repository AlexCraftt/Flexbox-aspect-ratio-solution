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
</style>

<style scoped>
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
    background: #FFFD73;
    flex: 1 1 100%;
    width: 60%;
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
}

.item1{
    background: #73C9FF;
}

.item2{
    background: tomato;
}

.item3{
    background: #7373FF;
}

.item4{
    background: #73C9FF;
}

.item5{
    background: greenyellow;
}

.item6{
    background: lightcoral;
}

@media screen and (max-width: 780px){
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

@media screen and (max-width: 560px){
    .row .rel__offset{
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


