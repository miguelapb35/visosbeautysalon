<template>
<div>
    <section class="hero is-medium is-bold">
        <div class="hero-body-about">

        </div>
    </section>
            <div class="container">
        <!-- START ARTICLE FEED -->
        <section class="articles">
            <div class="column is-10 is-offset-1">
                <!-- START ARTICLE -->
                <div class="card article">
                    <div class="card-content">
                        <div class="media">
                            <div class="media-content has-text-centered">
                                    <h1 class="title "> Welcome to Visos Beauty Salon</h1>
                                    <h2 class="subtitle">15433A E. Hampden Av. Aurora, Co, 80013</h2>
                            </div>
                        </div>
                        <div class="content article-body">
                            Visos Beauty Salon strives to work in making a better version of you! Here at Visos we believe that your hair tells a story. As an important part of your image, your hair projects your identity, your beliefs and moods. We are committed on helping you discover the best version of you by providing you with the talent and technique from our expert stylists, who keep up with the latest trends and give you individual attention. As a Hispanic oriented business, we welcome clients from all cultures and all ages, creating a diverse atmosphere for which we are very proud off.
                        </div>
                    </div>
                </div>
                <!-- END ARTICLE -->
              </div>
        </section>
        <!-- END ARTICLE FEED -->
        </div>
</div>
</template>

<script>
export default {
  head() {
    return {
      title: 'About Visos Beauty Salon',
      meta: [
        {
          hid: 'description',
          name: 'description',
          content: 'Beauty Salon, Visos Beauty Salon, Aurora, 15433A E. Hampden Av. Aurora, Co, 80013, Colorado, 303 693 3089 ,The best place for haircuts, color, wax, haircuts for men, women, children, As a Hispanic oriented business, we welcome clients from all cultures and all ages, creating a diverse atmosphere for which we are very proud off'
        }
      ]
    }
  }
}
</script>

<style>
.hero-body-about
{
background-image: url(../assets/img/visos-salon2.jpeg);
background-position: center;
background-size: cover;
background-repeat: no-repeat;
height: 500px;
}
.articles {
  margin: 5rem 0;
  margin-top: -200px;
}
.card article{
  border-radius: 6px;
  box-shadow: 0 16px 24px 2px rgba(0,0,0,.14), 0 6px 30px 5px rgba(0,0,0,.12), 0 8px 10px -5px rgba(0,0,0,.2);
}
.articles .content p {
    line-height: 1.9;
    margin: 15px 0;
}
.author-image {
    position: absolute;
    top: -30px;
    left: 50%;
    width: 60px;
    height: 60px;
    margin-left: -30px;
    border: 3px solid #ccc;
    border-radius: 50%;
}
.media-center {
  display: block;
  margin-bottom: 1rem;
}

.article, .promo-block {
  margin-top: 6rem;
}
div.column.is-8:first-child {
  padding-top: 0;
  margin-top: 0;
}
.article-title {
  font-size: 2rem;
  font-weight: lighter;
  line-height: 2;
}
.article-subtitle {
  color: #909AA0;
  margin-bottom: 3rem;
}
.article-body {
  line-height: 1.4;
/*   margin: 0 6rem; */
  padding-bottom: 50px;
}
.promo-block .container {
  margin: 1rem 5rem;
}
/* .title{
  line-height: unset;
} */


@media screen and (max-width: 768px) {

}
</style>
