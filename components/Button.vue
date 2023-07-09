<template>
  <button class="btn" :class="`btn-${variant}`">{{ label }}</button>
</template>

<script>
export default {
  props: {
    label: {
      type: String,
      required: true
    },
    variant: {
      type: String,
      default: "primary"
    }
  }
};
</script>

<style>
.btn {
  padding: 10px 20px;
  border-radius: 4px;
  color: #fff;
  cursor: pointer;
}

.btn-primary {
  background-color: #007bff;
}

.btn-danger {
  background-color: #dc3545;
}
</style>