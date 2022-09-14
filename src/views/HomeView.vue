<template>
  <div>
    <div>
      <AppHeader/>
      <div class="">
        <AboutUs class="my-5"/>
        <WhatWeDo/>
        <OurNumbers class="my-5"/>
        <BookNow/>
      </div>
    </div>
  </div>
</template>

<script>
import AppHeader from '@/components/appHeader.vue';
import AboutUs from '@/components/aboutUs.vue';
import WhatWeDo from '@/components/whatWeDo.vue';
import OurNumbers from '@/components/ourNumbers.vue';
import BookNow from '@/components/bookNow.vue';
export default {
    components: { AppHeader, AboutUs, WhatWeDo, OurNumbers, BookNow }
}
</script>
