<template>
  <b-container class="my-5" id="OurService">
    <p class="mainFont">أمثلة علي استخدام واتس لووب</p>

    <b-row align-h="center">
      <b-col cols="10" sm="10"  md="6" lg="3" class="px-5 my-3">
        <div class="b-rounded shadow h pt-4 pb-2 px-2 d-flex justify-content-center align-items-center flex-column">
          <img :src="require(`~/assets/icon/call-center.png`)" class="p-2 mb-2 border-bottom">
          <h6 class="font-weight-bold mainColor">خدمة العملاء</h6>
          <p class="thrFont">
            بالتواجد الدائم علي مدار اليوم يساعدك علي الرد علي الاستفسارات العملاء بشكل فوري
          </p>
        </div>
      </b-col>
      <b-col cols="10" sm="10"  md="6" lg="3" class="px-5 my-3">
        <div class="b-rounded shadow h pt-4 pb-2 px-2 d-flex justify-content-center align-items-center flex-column">
          <img :src="require(`~/assets/icon/face-recognition.png`)" class="p-2 mb-2 border-bottom">
          <h6 class="font-weight-bold mainColor">أنظمة الحجوزات</h6>
          <p class="thrFont">
            يمكنك استخدامه في حجز المواعيد و تأكيدها و متابعتها و تقيمها بعد الأنتهاء
          </p>
        </div>
      </b-col>
      <b-col cols="10" sm="10"  md="6" lg="3" class="px-5 my-3">
        <div class="b-rounded shadow h pt-4 pb-2 px-2 d-flex justify-content-center align-items-center flex-column">
          <img :src="require(`~/assets/icon/digital-campaign.png`)" class="p-2 mb-2 border-bottom">
          <h6 class="font-weight-bold mainColor">التسويق الألكتروني</h6>
          <p class="thrFont">
            اعرض صور منتجاتك و أسعارها مع إمكانية طلبها من خلال موقعك مباشرة
          </p>
        </div>
      </b-col>
      <b-col cols="10" sm="10"  md="6" lg="3" class="px-5 my-3">
        <div class="b-rounded shadow h pt-4 pb-2 px-2 d-flex justify-content-center align-items-center flex-column">
          <img :src="require(`~/assets/icon/notification-bell.png`)" class="p-2 mb-2 border-bottom">
          <h6 class="font-weight-bold mainColor">التنبيهات التفاعلية</h6>
          <p class="thrFont">
            ارسل تنبيهات بحالة التسجيل أو طلب المنتجات و شحنها تلقائيا حال تسجيلها في النظام
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
