<template>

    <li class="product_item">
      <figure class="product_image">
        <slot name="img"></slot>
      </figure>
      <p class="book_title">
        <slot name="item"></slot>
      </p>
    </li>
</template>

<style scoped>
.product_item{  
list-style:none;
  margin-bottom:5em;
  width:30%;
}
.product_image{
  width:80%;
}
.product_image img{
width:100%;
}
.book_title{
  font-size:17px;
  padding:0 30px;
  line-height:3rem;
  font-weight:bold;
  letter-spacing:4px;
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
    .product_item{
        display:block;
    }
    .product_image{
  width:100%;
  text-align:center;
}
  .product_image img{
    width:90%;
}
.book_title{
    width:80%;
    margin: 0;
    padding: 0 10%;
    font-size: 18px;
}
}

</style>
