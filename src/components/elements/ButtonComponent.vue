<template>
  <button @click.prevent="scrollTo && scroll(scrollTo)" :class="[
              'button',
              (variant ? 'button_' + variant : false),
              (size ? 'button_' + size : false)
          ]">
    <slot></slot>
  </button>
</template>

<script>
export default {
  name: "ButtonComponent",
  props: {
    variant: String,
    size: String,
    scrollTo: String
  },
  methods: {
    scroll(selector) {
      document.querySelector(selector)
          .scrollIntoView({ behavior: 'smooth' });
    }
  }
}
</script>
