<template>
    <!-- START NAV -->
    <nav class="navbar is-fixed-top">
        <div class="container">
            <div class="navbar-brand">
                <nuxt-link to="/" class="navbar-item is-active has-text-weight-bold"> <span class="visos">Visos Beauty Salon</span>  
                  <img  src="@/assets/img/Logo.png" class="logo">                    
                </nuxt-link>

                <span class="navbar-burger burger" data-target="navbarMenu">
                <span></span>
                <span></span>
                <span></span>
                </span>
            </div>
            <div id="navbarMenu" class="navbar-menu">
                <div class="navbar-end">
                    <nuxt-link to="stylists" class="navbar-item">Stylists</nuxt-link>
                    <nuxt-link to="about" class="navbar-item">About</nuxt-link>
                    <nuxt-link to="contact" class="navbar-item">Contact</nuxt-link>
                    <a href="https://www.facebook.com/pages/Visos-Beauty-Salon/133093463404279" target="_blank" class="navbar-item">
                      <i class="fab fa-facebook"></i>
                    </a>     
                </div>
            </div>
        </div>
    </nav>
    <!-- END NAV -->

</template>

<script>
export default {

}
if(process.client){
document.addEventListener('DOMContentLoaded', () => {

  // Get all "navbar-burger" elements
  const $navbarBurgers = Array.prototype.slice.call(document.querySelectorAll('.navbar-burger'), 0);

  // Check if there are any navbar burgers
  if ($navbarBurgers.length > 0) {

    // Add a click event on each of them
    $navbarBurgers.forEach( el => {
      el.addEventListener('click', () => {

        // Get the target from the "data-target" attribute
        const target = el.dataset.target;
        const $target = document.getElementById(target);

        // Toggle the "is-active" class on both the "navbar-burger" and the "navbar-menu"
        el.classList.toggle('is-active');
        $target.classList.toggle('is-active');

      });
    });
  }

});
}
</script>

<style>
.container{
  padding: 0 32px;
}
.logo{
  padding-left: 8px;
}
.visos{
  font-size: 2rem;
}
.navbar-item{
  font-weight: 600;
  font-size: 1.3rem;
}

a.navbar-item:visited {
  color: #000;
}
a.navbar-item:hover {
  color:blanchedalmond;
  background-color:  rgb(175, 93, 175);
}

a.navbar-item:active{
  color: purple;
}
a.navbar-item.is-active:hover{
  color: purple;
}

</style>
