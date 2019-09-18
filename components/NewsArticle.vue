  <template>
    <article class="news_article">
      <figure class="news_image">
        <slot name="img"></slot>
      </figure>
      <div class="news_about_box">

        <h3 class="article_title">
          <slot name="title"></slot>
        </h3>
        <p class="date">
          <slot name="time"></slot>
        </p>
        <p class="article_about">
          <slot name="item"></slot>
        </p>
      </div>
    </article>
  </template>
  <style scoped>
  .news_article {
    display: flex;
    margin-top: 3em;
    transition: 0.3s;
  }

  .news_article:hover {
    opacity: 0.7;
  }

  .news_about_box {
    width: 49%;
  }

  .news_image {
    width: 41.66667%;
    text-align: center;
  }

  .news_image img {
    width: 90%;
  }

  .article_title {
    font-size: 1.8rem;
  }

  .date {
    margin-top: 0.5em;
    font-size: 1.2rem;
    color: #656c6e;
  }

  .article_about {
    font-size: 1.3rem;
    margin: 2em 0;
    color: #656c6e;
  }
  @media screen and (max-width:768px){
    .news_image {
      width: 44%;
    }

    .news_about_box {
      width: 60%;
      padding-left: 10px;

    }
  }
  @media screen and (max-width:500px){
    .news_article{
      display:block;
    }
    .news_image{
      width:100%;
    }
    .news_image img{
width:100%;
    }
    .news_about_box{
      width:100%;
      padding:0;
    }
    .article_title{
      width:100%;
      font-size:1.8rem;
      margin-top:1em;
      line-height:3rem;
  font-weight:800;
    }
    .article_about{
      display:none;
    }
    
  }
  </style>
