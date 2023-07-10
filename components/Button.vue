<template>
  <button class="btn" :class="`btn-${variant}`">
    <slot></slot>
  </button>
</template>

<script>
import { ref } from 'vue';

export default {
  props: {
    variant: {
      type: String,
      default: "primary"
    }
  },
  setup(props) {
    const variant = ref(props.variant);

    return {
      variant
    };
  }
};
</script>