<template>

<div>
    <AppTop/>
    <Pay/>
    <br>
    <AppBottom/>
 </div>
</template>

<script>
import AppTop from '@/components/Global/AppTop';
import Pay from '@/components/local/Pay';
import AppBottom from '@/components/Global/AppBottom';

export default {
  components:{
    AppTop,
    Pay,
    AppBottom
  },
}
</script>
