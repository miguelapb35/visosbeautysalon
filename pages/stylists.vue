<template>
<div>
    <section class="is-medium is-bold">
        <div class="hero-body">
            <div class="container has-text-centered white">
                <h1 class="title title is-1 white">Visos Beauty Salon</h1>
                <h2 class="subtitle has-text-white">Hair cuts, color, wax & more </h2>
                <h3>15433A E. Hampden Av. Aurora, Co, 80013</h3>
            </div>
        </div>
    </section>
        <div class="container">
        <!-- START ARTICLE FEED -->
        <section class="articles">
            <div class="column">
                <!-- START ARTICLE -->
                <div class="card article">
                    <div class="card-content">
                        <div class="media">
                            <div class="media-content has-text-centered">
                                <p class="title article-title">Our Team of Stylists</p>
                            </div>
                        </div>
                        <div class="content article-body">
                            <div class="row">
                                <div class="columns has-text-centered">
                                    <div class="column">
                                        <div class="is-flex is-horizontal-center">
                                            <figure class="image is-128x128 ">
                                                <img class="is-rounded img-raised" src="../assets/img/stylist-bertha.JPG">
                                            </figure>
                                        </div>
                                        <div class="funcion">
                                            <h3 class="subtitle">Bertha</h3>
                                            <p>Cuts</p>
                                        </div>
                                    </div>
                                    <div class="column">
                                        <div class="is-flex is-horizontal-center">
                                            <figure class="image is-128x128 ">
                                                <img class="is-rounded img-raised" src="../assets/img/stylist-diana.jpeg">
                                            </figure>
                                        </div>
                                        <div class="funcion">
                                            <h3 class="subtitle">Diana</h3>
                                            <p>Color Expert</p>
                                        </div>
                                    </div>
                                </div>
                            </div>
                            <div class="row">
                                <div class="columns has-text-centered">
                                    <div class="column">
                                        <div class="is-flex is-horizontal-center">
                                            <figure class="image is-128x128 ">
                                                <img class="is-rounded img-raised" src="../assets/img/stylist-doris.jpeg">
                                            </figure>
                                        </div>
                                        <div class="funcion">
                                            <h3 class="subtitle">Doris</h3>
                                            <p>Color Expert</p>
                                        </div>
                                    </div>
                                    <div class="column">
                                        <div class="is-flex is-horizontal-center">
                                            <figure class="image is-128x128 ">
                                                <img class="is-rounded img-raised" src="../assets/img/stylist-mary.jpeg">
                                            </figure>
                                        </div>
                                        <div class="funcion">
                                            <h3 class="subtitle">Mary</h3>
                                            <p>Color Expert</p>
                                        </div>
                                    </div>
                                </div> 
                            </div>
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
    title: 'Visos Beauty Salon',
    meta: [
    {
        hid: 'description',
        name: 'description',
        content: 'Beauty Salon, 9:30 am -7 pm, Visos Beauty Salon, Aurora, 15433A E. Hampden Av. Aurora, Co, 80013, Colorado, 303 693 3089 , stylists, color experts, diana, doris, bertha, mary, haircuts, color, wax, haircuts for men, women, children, Hispanic oriented business, we welcome clients from all cultures and all ages'
    }
    ]
    }
}
}
</script>

<style scoped>
.hero-body
{
background-image: url(../assets/img/vue-mk-header.jpg);
background-position: center;
background-size: cover;
background-repeat: no-repeat;
height: 500px;
}
.funcion{
    margin: 1rem 0;
}
.img-raised{
    box-shadow: 0 5px 15px -8px rgba(0,0,0,.24), 0 8px 10px -5px rgba(0,0,0,.2);
}
.card article{
  border-radius: 6px;
  box-shadow: 0 16px 24px 2px rgba(0,0,0,.14), 0 6px 30px 5px rgba(0,0,0,.12), 0 8px 10px -5px rgba(0,0,0,.2);
}
.articles {
  margin: 5rem 0 0 0;
  margin-top: -200px;
}
.articles .content p {
    line-height: 1.9;
    margin: 15px 0;
}
.is-horizontal-center {
    justify-content: center;
}
.white{
    color: blanchedalmond;
}
.columns:nth-child(2)
{margin-top: -10rem;}
body {
background: #041221;
}
.card {overflow:hidden}
.card.large {
height: 600px;
-webkit-backface-visibility: hidden;
backface-visibility: initial;
border-radius: 5px;
}
.media-content {
overflow: hidden;
}
.title.no-padding {
margin-bottom: 0 !important;
}
#flow span {
display: block;
width: 200vw;
height: 200vw;
position: absolute;
top: -180vw;
left: -50vw;
border-radius: 90vw;
opacity: 0.6;
}
.flow-1 {
background: #3281ff;
-webkit-animation: rotating 20s linear infinite;
-moz-animation: rotating 20s linear infinite;
-ms-animation: rotating 20s linear infinite;
-o-animation: rotating 20s linear infinite;
animation: rotating 20s linear infinite;
}
.flow-2 {
background: #f442ee;
position: absolute;
-webkit-animation: rotating 15s linear infinite;
-moz-animation: rotating 15s linear infinite;
-ms-animation: rotating 15s linear infinite;
-o-animation: rotating 15s linear infinite;
animation: rotating 15s linear infinite;
}
.flow-3 {
background: #42eef4;
position: absolute;
-webkit-animation: rotating 7s linear infinite;
-moz-animation: rotating 7s linear infinite;
-ms-animation: rotating 7s linear infinite;
-o-animation: rotating 7s linear infinite;
animation: rotating 7s linear infinite;
}
@-webkit-keyframes rotating {
from {
-ms-transform: rotate(0deg);
-moz-transform: rotate(0deg);
-webkit-transform: rotate(0deg);
-o-transform: rotate(0deg);
transform: rotate(0deg);
}
to {
-ms-transform: rotate(360deg);
-moz-transform: rotate(360deg);
-webkit-transform: rotate(360deg);
-o-transform: rotate(360deg);
transform: rotate(360deg);
}
}
@keyframes rotating {
from {
-ms-transform: rotate(0deg);
-moz-transform: rotate(0deg);
-webkit-transform: rotate(0deg);
-o-transform: rotate(0deg);
transform: rotate(0deg);
}
to {
-ms-transform: rotate(360deg);
-moz-transform: rotate(360deg);
-webkit-transform: rotate(360deg);
-o-transform: rotate(360deg);
transform: rotate(360deg);
}
}
.rotating {
-webkit-animation: rotating 2s linear infinite;
-moz-animation: rotating 2s linear infinite;
-ms-animation: rotating 2s linear infinite;
-o-animation: rotating 2s linear infinite;
animation: rotating 2s linear infinite;
}
.footer{
background-color: #222831;
color: lemonchiffon;
}
.footer p, strong
{color: lemonchiffon}
.footer a:hover
{color: crimson;}
.fa
{color: lemonchiffon;
    margin: 10px}

::selection 
{background-color:#DEF4FF}
</style>
