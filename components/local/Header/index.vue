<template>
 <b-container class="bv-example-row my-5">
   <b-row align-h="center">
    <b-col cols="10" sm="10"  md="8" lg="6" class="content">
      <div class="">
        <p class="Toptext">
          منصة
          <sapn class="mainColor">clientanytime</sapn>
        </p>
        <p class="secFont">
          هي منصة تقدم و تتخصص في خدمة المجيب الالي(Bot) للواتس اب و التي تمكن الأفراد و أصحاب المتاجر اللإلكترونية من الإجابة علي عدد كبير من العملاء (العملاء المحتملين) أليا كالرد علي استفسارتهم
        </p>
        <div class="btns">
          <b-button size="sm" class="my-2 my-sm-2 mx-2 py-2 px-5 font-weight-bold" type="button" pill  variant="dark" v-b-tooltip.hover title="انقر لتصفح ال documentation لتعلم المزيد ...."> وثائق API</b-button>
          <b-button size="sm" class="my-2 my-sm-2 mx-2 py-2 px-5 font-weight-bold" type="button" pill  variant="outline-success" v-b-tooltip.hover title="فترة تجربية لمدة 5 أيام">
            <!-- <img :src="require(`~/assets/icon/Learn More icon.png`)" class="LearnIcon"/> -->
            تجربة مجانية
          </b-button>
        </div>
      </div>
    </b-col>
    <b-col cols="10" sm="10"  md="8" lg="6" class="d-flex justify-content-center">
      <img :src="require(`~/assets/img/WhatsApp2.jpeg`)" class="w-75" />
    </b-col>
  </b-row>
 </b-container>
</template>

<style scoped>
 .content{
   display: flex;
   justify-content: center;
   flex-direction: column;
 }
 .Toptext{
  font-size: 35px;
  font-weight: bolder;
 }

 .LearnIcon{
   width: 30px;
   margin-right: 5px;
 }
</style>
