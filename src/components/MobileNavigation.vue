<template>
  <div class="mobile-navigation" :class="{ 'is-active': navigationIsOpen}">
    <div class="mobile-navigation__content">
      <NavigationMenu class="mobile-navigation__navigation"/>
      <ButtonsBlock class="mobile-navigation__buttons" />
    </div>
  </div>
</template>

<script>
import NavigationMenu from '@/components/NavigationMenu.vue';
import ButtonsBlock from '@/components/elements/ButtonsBlock.vue';

export default {
  name: "MobileNavigation",
  props: ["navigationIsOpen"],
  components: {
    NavigationMenu,
    ButtonsBlock
  }
}

</script>