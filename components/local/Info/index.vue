<template>
 <b-container class="bv-example-row my-5">
   <b-row align-h="center">
    <b-col cols="10" sm="10"  md="8" lg="6" class="content">
      <div class="">
       <h6 class="font-weight-bold mainColor"> واتساب شات بوت</h6>
        <h3>
          أتمتة محادثات العملاء علي مدار الساعة طوال أيام الأسبوع باستخدام الشات بوت
        </h3>
        <p>
          نصمم معك شاب بوت يتناسب مع مستوي الأتمتة التي تحتاجها أعمالك يمكننا التعامل مع جميع احتياجات أتمتة المحادثات بدءاً من رسائل الترحيب الألية و الرد علي الأسئلة الشائعة عن طريف الذكاء الأصطناعي وصولاً لتقديم خدمة ذاتية متكاملة للعملاء
        </p>

        <div class="btns">
          <b-button size="sm" class="my-2 my-sm-2 mx-2 py-2 px-5 font-weight-bold" type="button" pill  variant="outline-success" v-b-tooltip.hover title="فترة تجربية لمدة 5 أيام">
            تجربة مجانية
          </b-button>
        </div>
      </div>
    </b-col>
    <b-col cols="10" sm="10"  md="8" lg="6" class="d-flex justify-content-center">
      <img :src="require(`~/assets/img/chatPhone3.png`)" class="w-25" />
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
