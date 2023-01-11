<template>
  <button :class="[
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
    size: String
  }
}
</script>
