<template>
  <div v-if="isOpen" class="alert" :class="`alert-${variant}`">
    <slot>Это предупреждение</slot>
    <button type="button" class="close" @click="closeAlert">&times;</button>
  </div>
</template>

<script>
import { ref } from 'vue';

export default {
  props: {
    variant: {
      type: String,
      default: "primary"
    }
  },
  setup() {
    const isOpen = ref(true);

    const closeAlert = () => {
      isOpen.value = false;
    };

    return {
      isOpen,
      closeAlert
    };
  }
};
</script>