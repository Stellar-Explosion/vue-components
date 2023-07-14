<template>
  <h5 class="card-title">
    <slot></slot>
  </h5>
</template>

<script>
import { h, defineComponent } from 'vue';

export default defineComponent({
  functional: true,
  render() {
    return h('h5', { class: 'card-title' }, this.$slots.default());
  }
});
</script>
