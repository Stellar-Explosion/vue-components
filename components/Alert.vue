<template>
  <div v-if="isOpen" class="alert" :class="`alert-${variant}`">
    {{ message }}
    <button type="button" class="close" @click="closeAlert">&times;</button>
  </div>
</template>

<script>
export default {
  props: {
    message: {
      type: String,
      required: true
    },
    variant: {
      type: String,
      default: "primary"
    }
  },
  data() {
    return {
      isOpen: true
    };
  },
  methods: {
    closeAlert() {
      this.isOpen = false;
    }
  }
};
</script>

<style>
.alert {
  padding: 10px;
  border-radius: 4px;
}

.alert-primary {
  background-color: #007bff;
  color: #fff;
}

.alert-danger {
  background-color: #dc3545;
  color: #fff;
}
</style>