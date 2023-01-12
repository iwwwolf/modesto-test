<template>
  <PageHeader/>
  <IntroSection />
  <FormSection />
</template>

<script>
import "./assets/style/main.scss";

import PageHeader from './components/PageHeader.vue';
import IntroSection from './components/IntroSection.vue';
import FormSection from './components/FormSection.vue';

export default {
  name: 'App',
  components: {
    PageHeader,
    IntroSection,
    FormSection
  }
}
</script>