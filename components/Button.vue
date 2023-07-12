<template>
  <button class="btn" :class="`btn-${variant}`">
    <slot>Кнопка</slot>
  </button>
</template>

<script>

export default {
  props: {
    variant: {
      type: String,
      default: "primary"
    }
  },
  setup(props) {
    const variant = props.variant;

    return {
      variant
    };
  }
};
</script>