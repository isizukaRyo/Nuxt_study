<template>
<footer>
<ul class="footer_list">
<li class="footer_item">
<p class="copyright">Copyright © 2019 PAS-POL -旅のモノづくりブランド-｜TABIPPO All rights reserved.</p>
</li>
</ul>

</footer>
</template>

<style scoped>
footer{
    width:100%;
    height:154px;
    margin:0 auto;
    display:flex;
    background-color: #656c6e;
}
.footer_list{
      max-width:1024px;
    width:100%;
    margin:0 auto;
    list-style:none;
}
.footer_item{
      text-align:right;
      color:white;
}
.copyright{
  width:80%;
  margin:0 auto;
  line-height:2em;
  margin-top:7em;
}

@media screen and (max-width:600px){
  .copyright{
    text-align:center;
  }
}
</style>