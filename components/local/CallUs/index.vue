<template>
  <b-container id="CallUs">
    <p class="mainFont">اتصل بنا</p>
    <b-row align-h="center">
      <b-col cols="11" sm="11"  md="10" lg="9" class="px-5 py-2 my-4 b-rounded shadow">
        <b-row align-h="center">
          <!-- <b-col cols="10" sm="10"  md="6" lg="6" class="p-3">
             <b-form @submit="onSubmit" @reset="onReset" v-if="show">

               <b-form-group id="input-group-3" label="سبب التواصل" label-for="input-3">
                <b-form-select
                  id="input-3"
                  v-model="form.contactReason"
                  :options="resons"
                  required
                ></b-form-select>
              </b-form-group>

               <b-form-group id="input-group-2" label="رقم الجوال" label-for="input-2">
                <b-form-input
                  id="input-2"
                  v-model="form.phoneNumber"
                  placeholder="ادخل رقم الجوال"
                  type="number"
                  required
                ></b-form-input>
              </b-form-group>

              <b-form-group
                id="input-group-1"
                label="البريد الألكتروني"
                label-for="input-1"
              >
                <b-form-input
                  id="input-1"
                  v-model="form.email"
                  type="email"
                  placeholder="ادخل البريد الألكتروني"
                  required
                ></b-form-input>
              </b-form-group>

              <b-form-group
                id="input-group-4"
                label="نص الرسالة"
                label-for="input-4"
              >
                <b-form-textarea
                  id="input-4"
                  v-model="form.message"
                  placeholder="نص الرسالة"
                  required
                ></b-form-textarea>
              </b-form-group>

              <b-button size="sm" class="my-2 my-sm-2 mx-2 py-1 px-2 secFont w-100" type="button" variant="success" v-on:click="onSubmit">ارسال طلب اتصال</b-button>
            </b-form>

          </b-col> -->
          <b-col cols="11" sm="11"  md="6" lg="6" class="p-3">
            <p class="text-center secFont">وسائل التواصل</p>
            <div class="d-flex flex-column justify-content-start align-items-center w-100">
              <div class="d-flex justify-content-center align-items-center my-2">
              <img :src="require(`~/assets/icon/phone.png`)" class="img">
              <p class="font-weight-bold my-0 mr-4">3564654677575894564+</p>
              </div>
              <div class="d-flex justify-content-center align-items-center my-2">
                <img :src="require(`~/assets/icon/email.png`)" class="img">
                <p class="font-weight-bold my-0 mr-4">yasser000@gmail.com</p>
              </div>
            </div>
            <div class="d-flex justify-content-center w-100">
                <img :src="require(`~/assets/img/WhatsApp1.jpeg`)" class="poster">
            </div>
          </b-col>
        </b-row>
      </b-col>
    </b-row>
  </b-container>
</template>


<script>
import axios from "axios";
  export default {
    data() {
      return {
        form: {
          email: '',
          phoneNumber: '',
          contactReason: null,
          message: ''
        },
        resons: [{ text: 'التواصل مع إدارة الموقع', value: null }, 'سبب 1', 'سبب 2', 'سبب 4', 'سبب 3'],
        show: true
      }
    },
    methods: {
      onSubmit(event) {
        event.preventDefault()
        console.log(JSON.stringify(this.form))
        axios
          .post(`${process.env.apiURL}/contactus`, JSON.stringify(this.form))
          .then((res) => {
            console.log(res);
            console.log(res.status);
            this.resCase = res.status;
            this.warning = "";
          })
          .catch((error) => {
            console.log(error);
            this.resErorr = error;
          });
      },
      onReset(event) {
        event.preventDefault()
        // Reset our form values
        this.form.email = ''
        this.form.phoneNumber = ''
        this.form.contactReason = null
        this.form.message = ''
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
 .icon{
   width: 25px;
   height: 25px;
 }
 .img{
   width: 50px;
 }
 .poster{
   height: 250px;
 }
</style>

