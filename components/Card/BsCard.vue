<template>
  <div class="card">
    <img :src="image" class="card-img-top" alt="...">
    <div class="card-body">
      <slot></slot>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    image: {
      type: String,
      required: true,
    },
  },
};
</script>