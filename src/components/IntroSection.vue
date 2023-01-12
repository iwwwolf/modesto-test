<template>
  <section class="intro">
    <div class="main-container">
      <div class="intro__content">
        <h1>Мы будем рады сотрудничать с вами на платформе 'Международной цветочной онлайн-площадки'!</h1>
        <p>Присоединяйтесь к нам и начните получать доход с бизнеса в первый месяц регистрации! </p>
        <ButtonsBlock>
          <ButtonComponent variant="primary" size="large" scrollTo="#registrationSection">Начать покупать</ButtonComponent>
          <ButtonComponent variant="secondary" size="large" scrollTo="#registrationSection">Начать продавать</ButtonComponent>
        </ButtonsBlock>
      </div>
    </div>
  </section>
</template>

<script>
import ButtonsBlock from '@/components/elements/ButtonsBlock.vue';
import ButtonComponent from '@/components/elements/ButtonComponent.vue';

export default {
  name: "IntroSection",
  components: {
    ButtonsBlock,
    ButtonComponent,
  }
}
</script>
