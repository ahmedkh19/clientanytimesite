<template>
 <div>
    <AppNav/>
    <Header/>
    <OurView/>
    <OurService/>
    <Cards/>
    <CallUs/>
    <AppFooter/>
 </div>
</template>

<script>
import AppNav from '@/components/Global/AppNav';
import Header from '@/components/local/Header';
import OurView from '@/components/local/OurView';
import OurService from '@/components/local/OurService';
import Cards from '@/components/local/Cards';
import CallUs from '@/components/local/CallUs';
import AppFooter from '@/components/Global/AppFooter';

export default {
  components:{
    AppNav,
    Header,
    OurView,
    OurService,
    Cards,
    CallUs,
    AppFooter
  },
}
</script>
