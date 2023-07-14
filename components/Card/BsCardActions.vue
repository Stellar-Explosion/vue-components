<template>
  <a class="btn btn-primary" href="#">
    <slot></slot>
  </a>
</template>

<script>
import { h, defineComponent } from 'vue';

export default defineComponent({
  functional: true,
  render() {
    return h('a', { class: 'btn btn-primary', href: '#' }, this.$slots.default());
  }
});
</script>
