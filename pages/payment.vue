<template>

<div>
    <AppNav/>
    <Pay/>
    <br>
    <AppFooter/>
 </div>
</template>

<script>
import AppNav from '@/components/Global/AppNav';
import Pay from '@/components/local/Pay';
import AppFooter from '@/components/Global/AppFooter';

export default {
  components:{
    AppNav,
    Pay,
    AppFooter
  },
}
</script>
