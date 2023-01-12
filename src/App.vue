<template>
  <main>
    <PageHeader/>
    <IntroSection />
    <FormSection />
    <PageFooter />
  </main>
</template>

<script>
import "./assets/style/main.scss";

import PageHeader from './components/PageHeader.vue';
import IntroSection from './components/IntroSection.vue';
import FormSection from './components/FormSection.vue';
import PageFooter from "@/components/PageFooter";

export default {
  name: 'App',
  components: {
    PageFooter,
    PageHeader,
    IntroSection,
    FormSection
  }
}
</script>