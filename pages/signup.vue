<template>
  <div class="px-4">
     <b-row  align-h="center">
      <b-col cols="10" sm="10"  md="6" lg="6" class="">
        <div class="nave">
          <NuxtLink  to="/" >
           <img :src="require(`~/assets/logo/logo.png`)" class="logo"/>
          </NuxtLink>
        </div>
        <div class="my-5">
           <p class="Toptext">
          اهلاً بكم من جديد في
          <sapn class="mainColor">clientanytime</sapn>
        </p>
        <p class="mainColor fs">تسجيل الدخول</p>
        </div>

        <b-row align-h="center">
          <b-col cols="10" sm="10"  md="8" lg="8" class="p-3">
            <b-form @submit="onSubmit" @reset="onReset" v-if="show">

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

          <b-form-group id="input-group-2" label="كلمة المرور" label-for="input-2">
            <b-form-input
              id="input-2"
              v-model="form.number"
              placeholder="كلمة المرور"
              type="number"
              required
            ></b-form-input>
          </b-form-group>

          <b-button size="sm" class="my-2 my-sm-2 mx-2 py-1 px-2 secFont w-100" type="button" variant="success">  تسجيل الدخول</b-button>
            </b-form>
          </b-col>
        </b-row>

      </b-col>
      <b-col cols="10" sm="10"  md="6" lg="6" class="">
        <div class="w-100 d-flex justify-content-center align-items-center">
          <img :src="require(`~/assets/img/WhatsApp3.jpeg`)" class="imgSignUp">
        </div>
      </b-col>
    </b-row>
  </div>

</template>


<script>
  export default {
    data() {
      return {
        form: {
          email: '',
          number: '',
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
        this.form.email = ''
        this.form.number = ''
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
 .nave{
   border-bottom: 2px solid var(--GrayColor);
  padding: 10px;
 }
 .logo{
  width: 120px;
  height: 40px;
 }
 .imgSignUp{
   height: 99vh;
   width: 99%;
 }
 .Toptext{
  font-size: 22px;
  font-weight: bolder;
 }
 .fs{
   font-size: 30px;
   font-weight: 600;
 }

</style>
