<template>
  <div class="container">
    <slot></slot>
  </div>
</template>

<script>
export default {
  props: {
    containerClass: {
      type: String,
      default: 'container',
    },
  },
};
</script>