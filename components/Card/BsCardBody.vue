<template>
  <p class="card-text">
    <slot></slot>
  </p>
</template>

<script>
import { h, defineComponent } from 'vue';

export default defineComponent({
  functional: true,
  render() {
    return h('p', { class: 'card-text' }, this.$slots.default());
  }
});
</script>
