<template>
  <div>
    <Button variant="secondary"></Button>
    <Alert></Alert>
    <Card-list image="/no-photo.jpg">
      <template v-slot:title>Заголовок</template>
      <template v-slot:text>Текст</template>
      <template v-slot:button>Кнопка-ссылка</template>
    </Card-list>
  </div>
</template>

<script>

</script>
