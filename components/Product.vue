<template>
  <section class="product">
    <div class="product_box">
      <h2 class="product_title">PRODUCT</h2>
      <ul class="more">
      <li class="more_inner">MORE</li>
      </ul>
      <ul class="product_list">
      
      <template>
      <ProductItem>
      <template slot="img"><img src="images/music_fes.png"></template>
      <template slot="item"> The World Festival Guide -海外の音楽フェス完全ガイド-</template>
      </ProductItem>
      </template>

      <template>
      <ProductItem>
       <template slot="img"> <img src="images/die_2000.png"></template>
      <template slot="item"> この世界で死ぬまでにしたいこと2000</template>
      </ProductItem>
      </template>
      
      <template>
      <ProductItem>
         <template slot="img"> <img src="images/calender.png"></template>
      <template slot="item">365日日本一周 絶景日めくりカレンダー</template>
      </ProductItem>
      </template>
      
      <template>
      <ProductItem>
      <template slot="img"><img src="images/passport.png"></template>
      <template slot="item"> PASSPORT NOTEBOOK series</template>
      </ProductItem>
      </template>

      <template>
      <ProductItem>
        <template slot="img"><img src="images/english.png"></template>
      <template slot="item">ひとり旅英会話<span class="hon">BOOK</span></template>
      </ProductItem>
      </template>

      <template>
      <ProductItem>      
      <template slot="img"><img src="images/post_card.jpeg"></template>
      <template slot="item">日本の絶景ポストカード　春編</template>
      </ProductItem>
      </template>
      </ul>
    </div>
  </section>
</template>
<script>
  import ProductItem from '~/components/ProductItem.vue'


    export default {
    components: {
     ProductItem
    }
  }
</script>
<style scoped>
.product{
  width:100%;
  margin:0 auto;
  padding-top:8em;
  
}
.product_list{
  display:flex;
  flex-wrap:wrap;
  justify-content:space-between;
}
.product_box{
  width:90%;
  max-width:940px;
  margin:0 auto;
  position:relative;
}
.more{
    font-size:1.4rem;
    position: absolute;
    top:0;
    right: 0;
    width: 162px;
    height: 46px;
    line-height: 46px;
    border: solid 1px;
    text-align: center;
    display:flex;
    justify-content:center;
  transition:0.3s;
  
  }
  .more:hover{
    background-color:black;
    color:white;
  }
  .more_inner{
    list-style:none;
    position:relative; 
  }
  .more_inner:before{
    content:">";
    position:absolute;
    right:-50px;
    top:-1px;
    font-size:16px;
  }

.product_title{
  font-size:3rem;
    margin-bottom:2.5em;
    font-weight: 100;
}
a{
  text-decoration:none;
  color:#13191b;
}
.hon{
  display:block;
}
@media screen and (max-width:768px){
  .product_list{
    display:block;
  }

  .product_item{
     width:100%;
     display:flex;
  list-style:none;
  margin-bottom:5em;
  }
  .book_title{
    width:100%;
    padding:0;
  }
.product_image{
  width:70%;
}
  .product_image img{
    width:80%;
}
.hon{
  display:inline;
}
}
@media screen and (max-width:500px){
  .product{
    padding-bottom:12em;
  }
  .more{
    top:auto;
    bottom:-100px;
   right:0;
   left:0;
   margin:auto;
  }
  .product_title{
    text-align:center;
  }
  .product_item{
    display:block;
  }
  .product_image{
  width:100%;
}
  .product_image img{
    width:100%;
}

  .more_inner:before{
    content:">";
    position:absolute;
    bottom:10px;
    font-size:16px;
  }
  .product_list{
    display:block;
  }
}

</style>
