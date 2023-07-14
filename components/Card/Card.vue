<template>
  <div class="col-4">
    <div class="card">
      <img :src="image" class="card-img-top" alt="...">
      <div class="card-body">
        <slot name="title"></slot>
        <slot name="text"></slot>
        <slot name="button"></slot>
      </div>
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
