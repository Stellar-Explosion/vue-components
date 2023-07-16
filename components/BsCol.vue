<template>
  <div class="col-sm-3 col-md-6 col-lg-12">
    <slot></slot>
  </div>
</template>

<script>
export default {
  props: {
    colClass: {
      type: String,
      default: 'col',
    },
  },
};
</script>