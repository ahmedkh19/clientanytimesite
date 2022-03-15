<template>
  <div>
    <p class="wraper">
      <span class="mainFont my-5 line">الدفع</span>
      <!-- <div class="line"></div> -->
    </p>

    <b-container class="my-5">
      <div class="rounded border shadow p-5 my-5">
        <h4 class="text-center font-weight-bold">الدفع</h4>
        <div class="d-flex flex-wrap justify-content-center">
           <img :src="require(`~/assets/icon/paypal.svg`)" class="paypal">
           <img :src="require(`~/assets/icon/paypal.svg`)" class="paypal">
           <img :src="require(`~/assets/icon/paypal.svg`)" class="paypal">
        </div>
        <b-form @submit="onSubmit" @reset="onReset" v-if="show">

          <div class="d-flex flex-wrap w-100">
            <b-form-group class="w-50 px-3" id="input-group-3" label="رقم البطاقة" label-for="input-3">
            <b-form-input
              id="input-3"
              placeholder="رقم البطاقة"
              v-model="form.visaNumber"
              :options="resons"
              required

            ></b-form-input>
            </b-form-group>

            <b-form-group class="w-50 px-3" id="input-group-2" label="تاريخ الأنتهاء" label-for="input-2">
              <b-form-input
                id="input-2"
                v-model="form.visaData"
                placeholder="تاريخ الأنتهاء"
                required
              ></b-form-input>
            </b-form-group>
          </div>

          <div class="d-flex flex-wrap w-100">
            <b-form-group
            id="input-group-1"
            label=" رمز التحقق"
            label-for="input-1"
            class="w-50 px-3"
          >
            <b-form-input
              id="input-1"
              v-model="form.visaCode"
              placeholder="   رمز التحقق"
              required
            ></b-form-input>
            </b-form-group>

            <b-form-group
              id="input-group-4"
              label="  اسم حامل البطاقة"
              label-for="input-4"
              class="w-50 px-3"
            >
              <b-form-input
                id="input-4"
                v-model="form.visaName"
                placeholder="  اسم حامل البطاقة "
                required
              ></b-form-input>
            </b-form-group>

          </div>
          <div class="d-flex justify-content-center">
            <b-button size="sm" class="my-2 mx-auto py-2 px-5 thrFont w-25" type="button" variant="success"> تأكيد الدفع </b-button>
          </div>

        </b-form>
      </div>
    </b-container>
  </div>
</template>

<script>
  export default {
    data() {
      return {
        form: {
          visaName: '',
          visaCode: '',
          visaData: '',
          visaNumber: ''
        },
        show: true
      }
    },
    methods: {
      onSubmit(event) {
        event.preventDefault()
        alert(JSON.stringify(this.form))
      },
      onReset(event) {
        event.preventDefault()
        // Reset our form values
        this.form.visaName = ''
        this.form.visaCode = ''
        this.form.visaData = ''
        this.form.visaNumber = ''
        // Trick to reset/clear native browser form validation state
        this.show = false
        this.$nextTick(() => {
          this.show = true
        })
      }
    }
  }
</script>

<style scoped>
.wraper::after{
  content: '';
  position: absolute;
  top: 20px;
  bottom: 0;
  right: 0;
  left: 0;
  display: inline-block;
  height: .3em;
  width: 100%;
  padding: 0 30px 30px 30px;
  border-top:2px solid var(--mainColor);
    z-index: -1;

}
.wraper{
  position: relative;
  text-align: center;
  margin: 60px 0;

}
.line{
  padding: 0 40px;
   background-color: #fff;
  /* z-index: 1000000000; */
}
.paypal{
  width: 50px;
  height: 50px;
  background-color: #f0f0f0;
  padding: 8px;
  border-radius: 5px;
  margin: 20px;
}
</style>
