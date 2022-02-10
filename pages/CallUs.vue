<template>
 <div>
    <AppNav/>
    <CallUs/>
    <AppFooter/>
 </div>
</template>

<script>
import AppNav from '@/components/Global/AppNav';
import CallUs from '@/components/local/CallUs';
import AppFooter from '@/components/Global/AppFooter';

export default {
  components:{
    AppNav,
    CallUs,
    AppFooter
  },
}
</script>
