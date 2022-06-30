<template>
  <div class="page-wrapper page-main">
    <InviteBlock/>
    <AboutBlock/>
    <SwiperBlock/>
    <NewsBlock/>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
import InviteBlock from '@/components/main-page/_InviteBlock';
import AboutBlock from '@/components/main-page/_AboutBlock';
import SwiperBlock from '@/components/main-page/_SwiperBlock';
import NewsBlock from '@/components/main-page/_NewsBlock';

export default Vue.extend({
  name: 'IndexPage',
  components: {
    InviteBlock,
    AboutBlock,
    SwiperBlock,
    NewsBlock,
  },
})
</script>

<style lang="scss">
.page-main {
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
