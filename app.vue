<template>
  <div>
    <Button variant="secondary"></Button>
    <Alert></Alert>
    <Card image="/no-photo.jpg">
      <template v-slot:title>
        <CardTitle>Заголовок</CardTitle>
      </template>
      <template v-slot:text>
        <CardBody>Текст</CardBody>
      </template>
      <template v-slot:button>
        <CardActions>Кнопка</CardActions>
      </template>
    </Card>
  </div>
</template>

<script>

</script>
