<template>
  <div class="buttons-block">
    <slot>
      <ButtonComponent variant="link">Войти</ButtonComponent>
      <ButtonComponent class="buttons-block__registration-button">Создать аккаунт</ButtonComponent>
    </slot>
  </div>
</template>

<script>
import ButtonComponent from '@/components/ButtonComponent.vue';

export default {
  name: "ButtonsBlock",
  components: {
    ButtonComponent,
  }
}
</script>