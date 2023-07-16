<template>
  <div :class="['carousel-item', { 'active': active }]">
    <img :src="image" class="card-img-top" alt="...">
  </div>
</template>

<script>
export default {
  name: 'BsCarouselItem',
  props: {
    active: {
      type: Boolean,
      default: false,
    },
    image: {
      type: String,
      required: true,
    },
  },
};
</script>

