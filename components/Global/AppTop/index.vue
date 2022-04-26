<template>
  <b-container>
     <b-navbar toggleable="lg"  class="nav" >
      <b-navbar-brand href="#">
        <!-- <NuxtLink exact to="/" > -->
         <img :src="require(`~/assets/logo/logo.png`)" class="logo"/>
        <!-- </NuxtLink> -->
      </b-navbar-brand>

      <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

      <b-collapse id="nav-collapse" is-nav>
        <b-navbar-nav class="mx-auto">
          <NuxtLink  to="/" tag="li" exact class="nav-link">الرئيسية</NuxtLink >
          <NuxtLink to="/#OurView" class="nav-link"> رؤيتنا</NuxtLink>
          <NuxtLink to="/#OurService" class="nav-link">خدمتنا</NuxtLink>
          <NuxtLink to="/#Cards" class="nav-link">الباقات</NuxtLink>
          <NuxtLink to="/#CallUs" class="nav-link">اتصل بنا</NuxtLink>
        </b-navbar-nav>

        <!-- Right aligned nav items -->
        <b-navbar-nav class="mr-auto">
          <NuxtLink  to="/signup">
            <b-button size="sm" class="my-2 my-sm-2 mx-2 py-2 px-3" type="button" pill  variant="dark">انشاء حساب</b-button>
          </NuxtLink >
          <b-button size="sm" class="my-2 my-sm-2 mx-2 py-2 px-3" type="button" pill  variant="outline-success" >تسجيل دخول</b-button>


        </b-navbar-nav>
      </b-collapse>
     </b-navbar>
  </b-container>
</template>

<script>
// import vueSmoothScroll from 'vue-smooth-scroll'
// Vue.use(vueSmoothScroll)
</script>


<style scoped>
 .nav{
  border-bottom: 2px solid var(--mainColor);
 }
 .logo{
  width: 120px;
  height: 40px;
 }
 .nav-link{
  color: var(--DarkSecColor) !important;
  cursor: pointer;
 }
 .nav-link:hover{
  color: var(--DarkGrayColor) !important;
 }
 .nuxt-link-active{
   color: var(--mainColor) !important;
 }
</style>
