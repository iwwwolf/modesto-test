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
    <div class="intro__flowers-block">
      <div class="intro__flower intro__flower_1">
        <img src="../assets/images/flower.png" alt="">
      </div>
      <div class="intro__flower intro__flower_2">
        <img src="../assets/images/flower.png" alt="">
      </div>
      <div class="intro__flower intro__flower_3">
        <img src="../assets/images/flower.png" alt="">
      </div>
      <div class="intro__flower intro__flower_4">
        <img src="../assets/images/flower.png" alt="">
      </div>
      <div class="intro__flower intro__flower_5">
        <img src="../assets/images/flower.png" alt="">
      </div>
      <div class="intro__flower intro__flower_6">
        <img src="../assets/images/flower.png" alt="">
      </div>
      <div class="intro__flower intro__flower_7">
        <img src="../assets/images/flower.png" alt="">
      </div>
      <div class="intro__flower intro__flower_8">
        <img src="../assets/images/flower.png" alt="">
      </div>
      <div class="intro__flower intro__flower_9">
        <img src="../assets/images/flower.png" alt="">
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
