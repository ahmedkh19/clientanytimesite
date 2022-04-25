<template>
 <div>
    <AppNav/>
    <Header/>
    <OurView/>
    <OurService/>
    <WhtsappLoopEx />
    <InteractiveBot />
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
import WhtsappLoopEx from '@/components/local/WhtsappLoopEx';
import InteractiveBot from '@/components/local/InteractiveBot';
import Cards from '@/components/local/Cards';
import CallUs from '@/components/local/CallUs';
import AppFooter from '@/components/Global/AppFooter';

export default {
  components:{
    AppNav,
    Header,
    OurView,
    OurService,
    WhtsappLoopEx,
    InteractiveBot,
    Cards,
    CallUs,
    AppFooter
  },
}
</script>
