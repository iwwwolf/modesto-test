<template>
  <component :is="href ? 'a' : 'button'" @click.prevent="scrollTo && scroll(scrollTo)" :class="[
              'button',
              (variant ? 'button_' + variant : false),
              (size ? 'button_' + size : false)
          ]">
    <slot />
    <span class="button__icon" v-if=$slots.icon>
      <slot name="icon" />
    </span>
  </component>
</template>

<script>
export default {
  name: "ButtonComponent",
  props: {
    variant: String,
    size: String,
    scrollTo: String,
    href: String
  },
  methods: {
    scroll(selector) {
      document.querySelector(selector)
          .scrollIntoView({ behavior: 'smooth' });
    }
  }
}
</script>
