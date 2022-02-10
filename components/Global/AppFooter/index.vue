<template>
  <div>
    <b-container class="topBorder mt-5 py-4">
      <b-row align-h="center">
        <b-col cols="10" sm="10"  md="6" lg="6" class="mt-5">
          <div class="d-flex justify-content-center align-center-center">
            <img :src="require(`~/assets/logo/logo.png`)" class="footerLogo">
          </div>
        </b-col>
        <b-col cols="12" sm="12"  md="6" lg="6" class="mt-5">
          <div class="d-flex justify-content-md-start justify-content-center">
            <div class="d-flex justify-content-start align-items-center">
              <img :src="require(`~/assets/icon/Shape.png`)" class="">
              <p class="mr-3 mb-0">السعودية</p>
            </div>
            <div class="d-flex justify-content-start align-items-center mr-5">
              <img :src="require(`~/assets/icon/Path.png`)" class="">
              <p class="mr-3 mb-0">364767567+</p>
            </div>
          </div>
          <div class="d-flex justify-content-md-start justify-content-center mt-4">
            <img :src="require(`~/assets/icon/RSS.png`)" class="footerIcon">
            <img :src="require(`~/assets/icon/Facebook.png`)" class="footerIcon">
            <img :src="require(`~/assets/icon/instagram black.1.png`)" class="footerIcon">
            <img :src="require(`~/assets/icon/linkedin black.1.png`)" class="footerIcon">
            <img :src="require(`~/assets/icon/Pinterest.png`)" class="footerIcon">
            <img :src="require(`~/assets/icon/Twitter.png`)" class="footerIcon">
            <img :src="require(`~/assets/icon/youtube color.1.png`)" class="footerIcon">

          </div>
        </b-col>
      </b-row>
    </b-container>
    <b-container>
      <div class="my-4">
        <b-navbar-nav class="d-flex justify-content-center flex-row mx-auto">
          <NuxtLink  to="/" tag="li" exact class="nav-link">الرئيسية</NuxtLink >
          <NuxtLink to="/3" tag="li" class="nav-link">من نحن</NuxtLink>
          <NuxtLink to="/3" tag="li" class="nav-link">العملاء</NuxtLink>
          <NuxtLink to="/3" tag="li" class="nav-link">مواقع ذات صلة</NuxtLink>
          <NuxtLink to="/CallUs" tag="li" class="nav-link">اتصل بنا</NuxtLink >
        </b-navbar-nav>
      </div>
      <div class="text-center my-4 DarkGrayColor">
        <p>جميع الحقوق محفوظة لمنصة &copy; clientanytime </p>
      </div>
    </b-container>
  </div>
</template>

<style scoped>
 .topBorder{
   border-top: 1px solid var(--mainColor);
   border-bottom: 2px solid var(--DarkGrayColor);
 }
 .footerLogo{
   width: 250px;
 }
 .footerIcon{
   width:20px;
   margin: 0 12px;
 }
  .nav-link{
  color: var(--DarkGrayColor) !important;
  cursor: pointer;
  margin: 0 8px;
 }
 .nav-link:hover{
  color: var(--DarkSecColor) !important;
 }
 .nuxt-link-active{
   color: var(--mainColor) !important;
 }
</style>
