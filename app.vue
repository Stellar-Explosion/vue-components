<template>
  <div>
    <Button label="Кнопка" variant="danger" />
    <Alert message="Это предупреждение" variant="warning" />
  </div>
</template>

<script>
import Button from "./components/Button.vue";
import Alert from "./components/Alert.vue";

export default {
  components: {
    Button,
    Alert,
  }
};
</script>