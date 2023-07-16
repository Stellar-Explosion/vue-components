<template>
  <button class="carousel-control-prev bg-dark" type="button" :data-bs-target="target" data-bs-slide="prev">
    <span class="carousel-control-prev-icon" aria-hidden="true"></span>
    <span class="visually-hidden">Previous</span>
  </button>
</template>

<script>
export default {
  name: 'BsCarouselControlPrev',
  props: {
    target: {
      type: String,
      required: true,
    },
  },
};
</script>