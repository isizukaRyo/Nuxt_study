<template>
<header>
<div class="header_box">
<figure class="header_title">Menu</figure>
<p class="nbs">&nbsp;</p>
<nav>
<ul class="header_list">
<li class="header_item">TOP </li>
<li class="header_item">PRODUCT</li>
<li class="header_item">ABOUT</li>
<li class="header_item">NEWS</li>
<li class="header_item">CONTACT</li>
</ul>
</nav>
</div>
</header>
</template>
<style scoped>
header{
    width:100%;
    height:670px;
    margin:0 auto;
    background-image:url("../static/images/road.jpg");
}
.header_box{
max-width:1024px;
margin:0 auto;
display:flex;
justify-content:space-between;
}
.header_list{
    height:100px;
    line-height:120px;
}
.header_item{
    display:inline-block;
    margin-right:2em;
    font-size:1.4rem;
    color:white;
}
.header_title{
    display:none;
}
@media screen and (max-width:768px){
    .nbs{
        display:none;
    }
    .header_box{
        background-color:white;
        height:45px;
    }
    .header_list{
        display:none;
    }
    .header_title{
        display:block;
        font-size:20px;
        line-height:45px;
        margin-left:5%;
    }

}
</style>