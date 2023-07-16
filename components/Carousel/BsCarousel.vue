<template>
  <div class="carousel slide">
    <BsCarouselInner :items="items">
      <slot></slot>
    </BsCarouselInner>
    <BsCarouselControlPrev :target="targetId"></BsCarouselControlPrev>
    <BsCarouselControlNext :target="targetId"></BsCarouselControlNext>
  </div>
</template>

<script>
import BsCarouselInner from "~/components/Carousel/BsCarouselInner.vue";
import BsCarouselControlPrev from "~/components/Carousel/BsCarouselControlPrev.vue";
import BsCarouselControlNext from "~/components/Carousel/BsCarouselControlNext.vue";

export default {
  components: {
    BsCarouselInner,
    BsCarouselControlPrev,
    BsCarouselControlNext
  },
  props: {
    items: {
      type: Array,
      default: () => []
    }
  },
  computed: {
    targetId() {
      return `carousel-${this._uid}`;
    }
  }
}
</script>