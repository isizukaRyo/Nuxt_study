<template>
  <Main>
    <section class="slogan">
    <div class="slogan_box">
    <div class="item_box">
      <h1>旅に出よう</h1>
      <p class="slogan_item">僕たちが作りたいのは<br>持っているだけで旅に出たくなるモノ。<br>持っているだけでわくわくするモノ。</p>
      <p class="slogan_item">それは新しい時代の “パスポート”<br>僕たちが作るものは、<br>そんな、存在でありたい。</p>
      <p class="slogan_item">そして、人と人が繋がる<br>こんな時代だからこそ、<br>僕たちは、みんなでひとつのモノを<br>作ることを追求したい。</p>
      <figure></figure>
      <p class="slogan_item"> それは、自分と世界を繋げる<br>旅のモノづくりブランド<br></p>
      </div>
       </div>
    </section>
 <Product/>

    <News>
    <template><slot name="title"></slot></template>
    <template><slot name="time"></slot></template>
    <template><slot name="item"></slot></template>
    </News>

        <ul class="share_list">
        <li class="top">^</li>
          <li class="share_item face">Share on Facebook</li>
          <li class="share_item twitter">Share on Twitter</li>
          <li class="share_item hatena">Hatena Bookmark</li>
          <li class="share_item line">Send to LINE</li>
        </ul>

        <ul class="bottom_list">
          <li class="bottom_item">TOP</li>
          <li class="bottom_item">PRODUCT</li>
          <li class="bottom_item">ABOUT</li>
          <li class="bottom_item">NEWS</li>
          <li class="bottom_item">CONTACT</li>
        </ul>
   
  </Main>
</template>
<script>
  import Product from '~/components/Product.vue'
   import News from '~/components/News.vue'
  export default {
    components: {
      Product,
      News
    }
  }

</script>

<style scoped>
.slogan{
    width:100%;
    margin:0 auto;
    background-color: #f6f6f6;
}
.slogan_box{
    max-width: 370px;
    margin:0 auto;
    padding-bottom:5em;
}

h1{
    font-size:4.4rem;
    text-align:center;
    padding-top:2.5em;
    margin-bottom:1em;
    font-weight:100;
}
.slogan_item{
    text-align:justify;
    margin:0 auto;
    font-size:2rem;
    margin-bottom:2em;
}

.share_list{
    width:100%;
    margin:0 auto;
    text-align:center;
    padding:35px 0;
    position:relative;
    display:flex;
    justify-content:center;
    flex-wrap:wrap;
}
.share_item{
    list-style:none;
    font-size:1.4rem;
    width: 162px;
    height: 46px;
    line-height: 48px;
    border:solid 1px;
    transition:0.3s;
}
.top{
    position:absolute;
    top:-20px;
    left:48%;
    list-style:none;
    font-size:30px;
    background-color:white;
    width:50px;
    height:50px;
    border-radius:50px;
    color: #656c6e;
    cursor:pointer;
   transition:0.3s;
    
}
.top:hover{
    transform: translateY(-5px);
}
.face:hover{
    color:white;
    background-color:#4871a9;
}
.face{
    color: #4871a9;
    border-color: #4871a9;
    
}
.twitter{
    color: #70bdd3;
    border-color: #70bdd3;
    margin:0 2em;
}
.twitter:hover{
    color:white;
    background-color:#70bdd3;
}
.hatena{
    color: #2f9bcd;
    border-color: #2f9bcd;
}
.hatena:hover{
    color:white;
    background-color:#2f9bcd;
}
.bottom_list{
    width:100%;
    margin:0 auto;
    text-align:center;
    background-color: #939899;
    padding:30px 0;
}
.bottom_item{
display:inline-block;
font-size:1.4rem;
color:white;
padding:0 20px;
cursor:pointer;

}
.line{ 
    color: #8ec09d;
    border-color: #8ec09d;
    margin:0 2em;
    display:none;
}
.item_box{
    width:100%;
}
@media screen and (max-width:700px){
    h1{
        text-align:justify;
    }
    .slogan_box{
        margin-left:8em;
    }
}
@media screen and (max-width:600px){
    .share_list{
        width:90%;
        justify-content:space-evenly;
    }
    .share_item{
        width:45%;
    }
    .top{
        left:45%;
    }
    .twitter{
        margin:0;
        margin-bottom:0.5em;
    }
.line{
    display:block;
    margin:0;
}
.bottom_list{
    padding:0;
}
.bottom_item{
    width:100%;
    padding:16px 0;
    border-bottom:solid 1px white;
}
.bottom_item:nth-child(5){
    border:none;
}
}
@media screen and (max-width:500px){
    h1{
        font-size:3.6rem;
    }
    .slogan_box{
        margin-left:2em;
    }
    .slogan_item{
        font-size:1.5rem;
    }
    .share_item{
        font-size:1.3rem;
    }
}

</style>
