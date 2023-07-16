<template>
  <button class="carousel-control-next bg-dark" type="button" :data-bs-target="target" data-bs-slide="next">
    <span class="carousel-control-next-icon" aria-hidden="true"></span>
    <span class="visually-hidden">Next</span>
  </button>
</template>


<script>
export default {
  name: 'BsCarouselControlNext',
  props: {
    target: {
      type: String,
      required: true,
    },
  },
};
</script>

