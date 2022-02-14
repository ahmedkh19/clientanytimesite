<template>
  <b-container class="my-5" id="OurService">
    <p class="mainFont">خدماتنا</p>
    <b-row align-h="center">
      <b-col cols="10" sm="10"  md="6" lg="3" class="px-5 my-3">
        <div class="b-rounded shadow h pt-4 pb-2 px-2 d-flex justify-content-center align-items-center flex-column">
          <img :src="require(`~/assets/icon/drag-and-drop 1.png`)" class="p-2 mb-2 border-bottom">
          <p class="thrFont">
            امكانية انشاء المجيب الالي من دون اي خبرة برمجية مسبقة!
            <br>
            عن طريق خاصية السحب و الافلات
          </p>
        </div>
      </b-col>
      <b-col cols="10" sm="10"  md="6" lg="3" class="px-5 my-3">
        <div class="b-rounded shadow h pt-4 pb-2 px-2 d-flex justify-content-center align-items-center flex-column">
          <img :src="require(`~/assets/icon/bot 1.png`)" class="p-2 mb-2 border-bottom">
          <p class="thrFont">
           مجيب الي ذكي صمم خصيصاً لراحتك و راحة عملائك
          </p>
        </div>
      </b-col>
      <b-col cols="10" sm="10"  md="6" lg="3" class="px-5 my-3">
        <div class="b-rounded shadow h pt-4 pb-2 px-2 d-flex justify-content-center align-items-center flex-column">
          <img :src="require(`~/assets/icon/api 1.png`)" class="p-2 mb-2 border-bottom">
          <p class="thrFont">
            خدمة الربط البرمجي API التي تمكنك من ارسال الصور و الرسائل النصية من موقعك
          </p>
        </div>
      </b-col>
      <b-col cols="10" sm="10"  md="6" lg="3" class="px-5 my-3">
        <div class="b-rounded shadow h pt-4 pb-2 px-2 d-flex justify-content-center align-items-center flex-column">
          <img :src="require(`~/assets/icon/shield 1.png`)" class="p-2 mb-2 border-bottom">
          <p class="thrFont">
            نوفر لك الحماية مع تشفير https رسالتك دائما في امان
          </p>
        </div>
      </b-col>
    </b-row>
    <b-row align-h="center">
      <b-col cols="10" sm="10"  md="6" lg="3" class="px-5 my-3">
        <div class="b-rounded shadow h pt-4 pb-2 px-2 d-flex justify-content-center align-items-center flex-column">
          <img :src="require(`~/assets/icon/quick 1.png`)" class="p-2 mb-2 border-bottom">
          <p class="thrFont">
            وداعا لتكرار الكتابة... مع نظام الردور السريعة والاختصارات
          </p>
        </div>
      </b-col>
      <b-col cols="10" sm="10"  md="6" lg="3" class="px-5 my-3">
        <div class="b-rounded shadow h pt-4 pb-2 px-2 d-flex justify-content-center align-items-center flex-column">
          <img :src="require(`~/assets/icon/videos 1.png`)" class="p-2 mb-2 border-bottom">
          <p class="thrFont">
           نظام الأقسام وهو اشبه بنظام المرور الذي يمكن فريقك المتخصص من التعامل مع رسائل أقسامهم فقط
          </p>
        </div>
      </b-col>
      <b-col cols="10" sm="10"  md="6" lg="3" class="px-5 my-3">
        <div class="b-rounded shadow h pt-4 pb-2 px-2 d-flex justify-content-center align-items-center flex-column">
          <img :src="require(`~/assets/icon/support-ticket 1.png`)" class="p-2 mb-2 border-bottom">
          <p class="thrFont">
            نظام التذاكر الذي يمكن فريق خدمة العملاء من القيام بعملهم بأريحية تامة
          </p>
        </div>
      </b-col>
      <b-col cols="10" sm="10"  md="6" lg="3" class="px-5 my-3">
        <div class="b-rounded shadow h pt-4 pb-2 px-2 d-flex justify-content-center align-items-center flex-column">
          <img :src="require(`~/assets/icon/technical-support 1.png`)" class="p-2 mb-2 border-bottom">
          <p class="thrFont">
            دعم فني علي مدار الساعة لاستقبال اسئلتكم والرد علي استفساراتكم
          </p>
        </div>
      </b-col>
    </b-row>
  </b-container>
</template>

<style scoped>
 .h{
   height: 250px;
 }
</style>
