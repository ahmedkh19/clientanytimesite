<template>
  <b-container class="my-5" id="OurService">
    <p class="mainFont"> بناء بوت تفاعلي </p>

    <b-row align-h="center">
      <b-col cols="10" sm="10"  md="10" lg="3" class="px-4 my-3 text-center ">
        <img :src="require(`~/assets/img/chatPhone.png`)" class="p-2 mb-2 border-bottom">
      </b-col>
      <b-col cols="10" sm="10"  md="10" lg="6" class="px-4 my-3 ">
        <h5 class="text-center mb-4">
          تتميز بتقديم خدمتك علي مدار الساعو مع بوت واتس لووب من خلال تطبيق المراسلة المفضلة WhatsApp من خلال ممثل خدمة العملاء الألي و المبني علي خدمة الذكاء الاصطناعي
        </h5>
       <div class="accordion" role="tablist">
          <b-card no-body class="mb-2">
            <b-card-header header-tag="header" class="p-1" role="tab">
              <b-button block v-b-toggle.accordion-1 variant="success">هل يمكنني إنشاء بوت بدون معرفة برمجية ؟</b-button>
            </b-card-header>
            <b-collapse id="accordion-1" visible accordion="my-accordion" role="tabpanel">
              <b-card-body>
                <b-card-text>
                  نعم يمكنك بسهولة إنشاء بوت تفاعلي بدون اي خبرة برمجية مع نظام (السحب والافلات) بتصميم بسيط، كما نوفر المساعدة في انشاء البوت لفترة محدودة
                </b-card-text>
              </b-card-body>
            </b-collapse>
          </b-card>

          <b-card no-body class="mb-2">
            <b-card-header header-tag="header" class="p-1" role="tab">
              <b-button block v-b-toggle.accordion-2 variant="success">هل البوت يعمل مع واتس اب مباشرة ؟</b-button>
            </b-card-header>
            <b-collapse id="accordion-2" accordion="my-accordion" role="tabpanel">
              <b-card-body>
                <b-card-text>نعم </b-card-text>
              </b-card-body>
            </b-collapse>
          </b-card>

          <b-card no-body class="mb-2">
            <b-card-header header-tag="header" class="p-1" role="tab">
              <b-button block v-b-toggle.accordion-3 variant="success">هل يمكن إرسال صور و فيديوهات علي ردود العملاء ؟</b-button>
            </b-card-header>
            <b-collapse id="accordion-3" accordion="my-accordion" role="tabpanel">
              <b-card-body>
                <b-card-text>نعم , يمكن ارسال الوسائط من تسجيل صوتي وصور ومقاطع فيديو الي اي شخص علي الواتساب</b-card-text>
              </b-card-body>
            </b-collapse>
          </b-card>

            <b-card no-body class="mb-2">
            <b-card-header header-tag="header" class="p-1" role="tab">
              <b-button block v-b-toggle.accordion-3 variant="success">كم عدد المحادثات التي يستطيع البوت الرد عليها؟</b-button>
            </b-card-header>
            <b-collapse id="accordion-4" accordion="my-accordion" role="tabpanel">
              <b-card-body>
                <b-card-text>يستطيع البوت التعامل مع عدد لا محدود من المحادثات بسرعة فائقة ومع نظام حماية من قوي يحميك من الحظر</b-card-text>
              </b-card-body>
            </b-collapse>
          </b-card>
        </div>
      </b-col>
     <b-col cols="10" sm="10"  md="10" lg="3" class="px-4 my-3 text-center">
        <img :src="require(`~/assets/img/chatPhone2.png`)" class="p-2 mb-2 border-bottom">
      </b-col>
    </b-row>
  </b-container>
</template>

<style scoped>
 .h{
   height: 250px;
 }
</style>

