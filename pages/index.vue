<template>
 <div>
    <AppTop/>
    <Header/>
    <OurView/>
    <OurService/>
    <WhtsappLoopEx />
    <Info/>
    <EmailBox/>
    <InteractiveBot />
    <Cards/>
    <CallUs/>
    <AppBottom/>
 </div>
</template>

<script>
import AppTop from '@/components/Global/AppTop';
import Header from '@/components/local/Header';
import OurView from '@/components/local/OurView';
import OurService from '@/components/local/OurService';
import WhtsappLoopEx from '@/components/local/WhtsappLoopEx';
import InteractiveBot from '@/components/local/InteractiveBot';
import Info from '@/components/local/Info';
import EmailBox from '@/components/local/EmailBox';
import Cards from '@/components/local/Cards';
import CallUs from '@/components/local/CallUs';
import AppBottom from '@/components/Global/AppBottom';

export default {
  components:{
    AppTop,
    Header,
    OurView,
    OurService,
    WhtsappLoopEx,
    InteractiveBot,
    Info,
    EmailBox,
    Cards,
    CallUs,
    AppBottom
  },
}
</script>
