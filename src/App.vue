<template>
  <PageHeader/>
  <IntroSection />
</template>

<script>
import "./assets/style/main.scss";

import PageHeader from './components/PageHeader.vue';
import IntroSection from './components/IntroSection.vue';

export default {
  name: 'App',
  components: {
    PageHeader,
    IntroSection
  }
}
</script>