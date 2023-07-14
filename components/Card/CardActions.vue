<template>
  <a href="#" class="btn" :class="`btn-${variant} btn-${size}`">
    <slot></slot>
  </a>
</template>

<script>
export default {
  props: {
    variant: {
      type: String,
      default: "primary"
    },
    size: {
      type: String,
      default: "lg"
    },
    disabled: {
      type: Boolean,
      default: false
    }
  },
};
</script>