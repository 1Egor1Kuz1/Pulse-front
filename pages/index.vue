<template>
  <div class="page-wrapper page-main">
    <InviteBlock/>
    <AboutBlock/>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
import InviteBlock from '@/components/main-page/_InviteBlock';
import AboutBlock from '@/components/main-page/_AboutBlock';

export default Vue.extend({
  name: 'IndexPage',
  components:{
    InviteBlock,
    AboutBlock
  },
})
</script>

<style  lang="scss">
.page-main{
  &__section {
    position: relative;
    display: -ms-flexbox;
    display: flex;
    -ms-flex-align: center;
    align-items: center;
    min-height: 100vh;
  }
}


</style>
