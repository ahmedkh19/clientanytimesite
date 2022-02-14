<template>
  <b-container class="my-5" id="Cards">
    <p class="mainFont">الباقات</p>
    <b-row align-h="center">
      <b-col cols="12" sm="10"  md="6" lg="5" class="px-5 my-4">
        <div class="postion-relative b-rounded shadow p-3 pb-5">
          <p class="mainFont my-2">اسم الحزمة</p>
          <div class="my-5 d-flex justify-content-around">
            <div class="rounded shadow p-2">
              <p class="DarkGrayColor mb-0 font-weight-bold">3 أشهر</p>
              <p class="mainColor mb-0">المدة</p>
            </div>
            <div class="rounded shadow p-2">
              <p class="mainColor mb-0">الأسعار</p>
              <p class="DarkGrayColor mb-0 font-weight-bold">410 ريال</p>
            </div>
          </div>
          <div class="border-top pt-3">
            <div class="d-flex justify-content-between align-items-center my-3">
              <p class="m-0">تفعيل خدمة البط البرمجي API</p>
              <img :src="require(`~/assets/icon/right.png`)" class="icon">
            </div>
            <div class="d-flex justify-content-between align-items-center my-3">
              <p class="m-0">تفعيل خدمة المجيب الالي API</p>
              <img :src="require(`~/assets/icon/right.png`)" class="icon">
            </div>
            <div class="d-flex justify-content-between align-items-center my-3">
              <p class="m-0">تفعيل قسم التذاكر لخدمة العملاء</p>
              <img :src="require(`~/assets/icon/right.png`)" class="icon">
            </div>
            <div class="d-flex justify-content-between align-items-center my-3">
              <p class="m-0">تفعيل نظام الأقسام</p>
              <img :src="require(`~/assets/icon/right.png`)" class="icon">
            </div>
            <div class="d-flex justify-content-between align-items-center my-3">
              <p class="m-0">تفعيل ميزة الردود السريعة</p>
              <img :src="require(`~/assets/icon/right.png`)" class="icon">
            </div>
            <div class="d-flex justify-content-between align-items-center my-3">
              <p class="m-0">عدد مستخدمين غير محدود</p>
              <img :src="require(`~/assets/icon/right.png`)" class="icon">
            </div>
            <div class="d-flex justify-content-between align-items-center my-3">
              <p class="m-0">تفعيل خدمة البط البرمجي API</p>
              <img :src="require(`~/assets/icon/right.png`)" class="icon">
            </div>
            <div class="d-flex justify-content-between align-items-center my-3">
              <p class="m-0">دعم فني علي مدار الساعة</p>
              <img :src="require(`~/assets/icon/right.png`)" class="icon">
            </div>
          </div>

          <b-button size="sm" class="my-2 my-sm-2 mx-2 py-3 px-4 postion-custom secFont" type="button" pill  variant="success"> اشترك بالحزمة</b-button>
        </div>
      </b-col>
      <b-col cols="12" sm="10"  md="6" lg="5" class="px-5 my-4">
        <div class="postion-relative b-rounded shadow p-3 pb-5">
          <p class="mainFont my-2">اسم الحزمة</p>
          <div class="my-5 d-flex justify-content-around">
            <div class="rounded shadow p-2">
              <p class="DarkGrayColor mb-0 font-weight-bold">شهر</p>
              <p class="mainColor mb-0">المدة</p>
            </div>
            <div class="rounded shadow p-2">
              <p class="mainColor mb-0">الأسعار</p>
              <p class="DarkGrayColor mb-0 font-weight-bold">150 ريال</p>
            </div>
          </div>
          <div class="border-top pt-3">
            <div class="d-flex justify-content-between align-items-center my-3">
              <p class="m-0">تفعيل خدمة البط البرمجي API</p>
              <img :src="require(`~/assets/icon/wrong.png`)" class="icon">
            </div>
            <div class="d-flex justify-content-between align-items-center my-3">
              <p class="m-0">تفعيل خدمة المجيب الالي API</p>
              <img :src="require(`~/assets/icon/wrong.png`)" class="icon">
            </div>
            <div class="d-flex justify-content-between align-items-center my-3">
              <p class="m-0">تفعيل قسم التذاكر لخدمة العملاء</p>
              <img :src="require(`~/assets/icon/right.png`)" class="icon">
            </div>
            <div class="d-flex justify-content-between align-items-center my-3">
              <p class="m-0">تفعيل نظام الأقسام</p>
              <img :src="require(`~/assets/icon/right.png`)" class="icon">
            </div>
            <div class="d-flex justify-content-between align-items-center my-3">
              <p class="m-0">تفعيل ميزة الردود السريعة</p>
              <img :src="require(`~/assets/icon/right.png`)" class="icon">
            </div>
            <div class="d-flex justify-content-between align-items-center my-3">
              <p class="m-0">عدد مستخدمين غير محدود</p>
              <img :src="require(`~/assets/icon/right.png`)" class="icon">
            </div>
            <div class="d-flex justify-content-between align-items-center my-3">
              <p class="m-0">تفعيل خدمة البط البرمجي API</p>
              <img :src="require(`~/assets/icon/right.png`)" class="icon">
            </div>
            <div class="d-flex justify-content-between align-items-center my-3">
              <p class="m-0">دعم فني علي مدار الساعة</p>
              <img :src="require(`~/assets/icon/right.png`)" class="icon">
            </div>
          </div>
          <b-button size="sm" class="my-2 my-sm-2 mx-2 py-3 px-4 postion-custom secFont" type="button" pill  variant="success"> اشترك بالحزمة</b-button>
        </div>
      </b-col>
    </b-row>
  </b-container>
</template>


<style scoped>
 .icon{
   width: 25px;
   height: 25px;
 }
</style>

