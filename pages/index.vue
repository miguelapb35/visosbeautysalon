<template>
  <div>
    <section class="is-medium is-bold">
        <div class="hero-body">
            <div class="container has-text-centered white">
                <h1 class="title title is-1 white titulo-visos">Visos Beauty Salon</h1>
                <h2 class="subtitle has-text-white">Hair cuts, color, wax & more </h2>
                    <div class="container has-text-centered">                                    
                      <h3>15433A E. Hampden Av. Aurora, Co, 80013</h3>
                      <h2>open Monday - Saturday 10am - 6pm</h2>
                      <h2>Make your Appointment: 303 693 3089, 303 693 0422</h2>
                    </div>                 
            </div>
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
                            <div class="media-content title title is-3 has-text-centered">
                              Our Services
                            </div>
                        </div>
            
                        <div id="staggered-list-demo" class="has-text-centered">
                          <input v-model="query" class="input is-rounded is-primary is-small" placeholder="Type service here...">
                          <transition-group
                            name="staggered-fade"
                            tag="ul"
                            v-bind:css="false"
                            v-on:before-enter="beforeEnter"
                            v-on:enter="enter"
                            v-on:leave="leave"
                          >
                                <li class="lista"
                                  v-for="(item, index) in computedList"
                                  v-bind:key="item.Service"
                                  v-bind:data-index="index"
                                >{{ item.Service }} {{ item.Price }}</li>

                          </transition-group>             
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
          content: 'The best place for haircuts, Mens hair cut, Mens hair cut, Women hair cut, Women color, Women high light, Face Waxing of eye brows, Make up, Bikini, Legs, Eyelash, Eye brows, lip'
        }
      ]
    }
  },  
  components: {
    
  },
  data() {
    return {
      query: '',
      list: [
            { Service: 'Kids hair cut', Price: '$ 12 and up'  },
            { Service: 'Mens hair cut', Price: '$ 14 and up' },
            { Service: 'Women hair cut', Price: '$ 16 and up' },
            { Service: 'Women color', Price : '$ 58 and up' },
            { Service: 'Perms', Price : '$ 48 and up' },
            { Service: 'Women high light', Price: '$ 55 and up' },        
            { Service: 'Face Waxing of eye brows', Price: '$ 10' },        
            { Service: 'Lip', Price: '$ 8' },        
            { Service: 'Eye brows & lip', Price: '$ 15' },        
            { Service: 'Total face', Price: '$ 45' },        
            { Service: 'Body waxing : Armpits', Price: '$ 20 and up' },        
            { Service: 'Bikini', Price: '$ 20 and up' },        
            { Service: 'Legs', Price: '$ 50' },        
            { Service: 'Half Legs', Price: '$ 25' },        
            { Service: 'Feet', Price: '$ 15' },        
            { Service: 'Make up', Price: '$ 30' },        
            { Service: 'Eyelash', Price: '$ 15' },         
      ]
    };
  }, 
  methods: {
    beforeEnter: function (el) {
      el.style.opacity = 0
      el.style.height = 0
    },
    enter: function (el, done) {
      var delay = el.dataset.index * 150
      setTimeout(function () {
        Velocity(
          el,
          { opacity: 1, height: '1.6em' },
          { complete: done }
        )
      }, delay)
    },
    leave: function (el, done) {
      var delay = el.dataset.index * 150
      setTimeout(function () {
        Velocity(
          el,
          { opacity: 0, height: 0 },
          { complete: done }
        )
      }, delay)
    }
  },  
  computed: {
    computedList: function () {
      var vm = this
      return this.list.filter(function (item) {
        return item.Service.toLowerCase().indexOf(vm.query.toLowerCase()) !== -1
      })
    }
  }  

}
</script>

<style scoped>
html,body {
  font-family: 'Open Sans', sans-serif;
  font-size: 14px;
  background: #eee;
}

.navbar.is-white {
  background: #F0F2F4;
}
.navbar-brand .brand-text {
  font-size: 1.11rem;
  font-weight: bold;
}
.lista {
  font-size: 2rem;
  margin-top: 1rem;
}
.hero-body
{
background-image: url(../assets/img/vue-mk-header.jpg);
background-position: center;
background-size: cover;
background-repeat: no-repeat;
height: 500px; 

}
.white{
  color: blanchedalmond;
}
.card article{
  border-radius: 6px;
  box-shadow: 0 16px 24px 2px rgba(0,0,0,.14), 0 6px 30px 5px rgba(0,0,0,.12), 0 8px 10px -5px rgba(0,0,0,.2);
}
.articles {
  margin: 5rem 0;
  margin-top: -200px;
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
  /* margin-top: 3rem; */
}
.article, .promo-block {
  margin-top: 6rem;
}
div.column.is-8:first-child {
  padding-top: 0;
  margin-top: 0;
}
.article-title {
/*   font-size: 2rem;
  font-weight: lighter;
  line-height: 2; */
}
.article-subtitle {
  color: #909AA0;
  margin-bottom: 3rem;
}
.article-body {
  line-height: 1.4;
  margin: 0;
}
.promo-block .container {
  margin: 1rem 5rem;
}
.title{
  line-height: unset;
}
input{
  width: 50%;
}

/* media queries */
@media (max-width: 768px) {
.title{
  line-height: unset;
}
.lista {
  font-size: 1.5rem;
}
input{
  width: 50%;
}
}

@media (max-width: 500px) {
.title{
  line-height: unset;
}
.lista {
  font-size: 1rem;
}
input{
  width: 60%;
}
.titulo-visos{
  font-size: 2rem;
}
}

/* .container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.title {
  font-family: 'Quicksand', 'Source Sans Pro', -apple-system, BlinkMacSystemFont,
    'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
} */
</style>
