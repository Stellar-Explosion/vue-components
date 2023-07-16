<template>
  <div class="row">
    <slot></slot>
  </div>
</template>

<script>
export default {
  props: {
    rowClass: {
      type: String,
      default: 'row',
    },
  },
};
</script>