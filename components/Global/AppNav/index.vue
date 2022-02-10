<template>
  <b-container>
     <b-navbar toggleable="lg"  class="nav" >
      <b-navbar-brand href="#">
        <img :src="require(`~/assets/logo/logo.png`)" class="logo"/>
      </b-navbar-brand>

      <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

      <b-collapse id="nav-collapse" is-nav>
        <b-navbar-nav class="mx-auto">
          <NuxtLink  to="/" tag="li" exact class="nav-link">الرئيسية</NuxtLink >
          <NuxtLink to="/2" tag="li" class="nav-link">من نحن</NuxtLink>
          <NuxtLink to="/2" tag="li" class="nav-link">العملاء</NuxtLink>
          <NuxtLink to="/2" tag="li" class="nav-link">مواقع ذات صلة</NuxtLink>
          <NuxtLink to="/CallUs" tag="li" class="nav-link">اتصل بنا</NuxtLink >
        </b-navbar-nav>

        <!-- Right aligned nav items -->
        <b-navbar-nav class="mr-auto">

          <b-button size="sm" class="my-2 my-sm-2 mx-2 py-2 px-3" type="button" pill  variant="dark">انشاء حساب</b-button>
          <b-button size="sm" class="my-2 my-sm-2 mx-2 py-2 px-3" type="button" pill  variant="outline-success" >تسجيل دخول</b-button>


        </b-navbar-nav>
      </b-collapse>
     </b-navbar>
  </b-container>
</template>

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
