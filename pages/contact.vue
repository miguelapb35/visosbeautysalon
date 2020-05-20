<template>
<div>
    <section class="hero is-medium is-bold">
        <div class="hero-body">

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
                                <h1 class="title article-title">For Appointments</h1>
                                <p class="has-text-centered">please call</p>
                                <div class="container has-text-centered">                                    
                                    <h2 class="subtitle">303 693 3089</h2>
                                    <h2 class="subtitle">303 693 0422</h2>
                                    <h2 class="subtitle last-subt">15433A E. Hampden Av. Aurora, Co, 80013</h2>
                                    <h1 class="title hast-text-centered">Hours of operation</h1>
                                </div> 
                            </div>
                        </div>
                        <div class="content article-body">
                            
                            <table class="table is-hoverable is-striped">
                            <thead>
                              <tr>
                                <td>Day</td>
                                <td>Hour</td>
                              </tr>
                            </thead>

                            <tbody>
                              <tr>
                                <th>Monday</th>
                                <td>10:00 am - 6 pm</td>
                              </tr>
                              <tr>
                                <th>Tuesday</th>
                                <td>10:00 am - 6 pm</td>
                              </tr>
                              <tr>
                                <th>Wednesday</th>
                                <td>10:00 am - 6 pm</td>
                              </tr>
                              <tr>
                                <th>Thursday</th>
                                <td>10:00 am - 6 pm</td>
                              </tr>
                              <tr>
                                <th>Friday</th>
                                <td>10:00 am - 6 pm</td>
                              </tr>
                              <tr>
                                <th>Saturday</th>
                                <td>10:00 am - 6 pm</td>
                              </tr>
                              <tr>
                                <th>Sunday</th>
                                <td>Closed</td>
                              </tr> 
                            </tbody>
                          </table>
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
      title: 'Contact Visos Beauty Salon',
      meta: [
        {
          hid: 'description',
          name: 'description',
          content: 'Beauty Salon, 9:30 am -7 pm, Visos Beauty Salon, Aurora, 15433A E. Hampden Av. Aurora, Co, 80013, Colorado, 303 693 3089 , haircuts, color, wax, haircuts for men, women, children, Hispanic oriented business, we welcome clients from all cultures and all ages'
        }
      ]
    }
  }
}
</script>

<style>
.hero-body
{
background-image: url(../assets/img/visos-salon.jpeg);
background-position: center;
background-size: cover;
background-repeat: no-repeat;
height: 500px;
}
.subtitle{
  font-weight: 600;
  font-size: 1.2rem;
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
.media-content {
  margin-top: 1rem;
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

@media screen and (max-width: 768px) {
    .media-content{
        height: auto;
        overflow: none;
    }
}
@media screen and (max-width: 500px) {
.last-subt{
  padding-bottom: 20px;
}
}
</style>
