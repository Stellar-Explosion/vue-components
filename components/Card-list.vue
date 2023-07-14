<template>
  <div class="container">
    <div class="row">
      <div class="col-4">
        <div class="card">
          <img :src="image" class="card-img-top" alt="...">
          <div class="card-body">
            <CardTitle>
              <slot name="title"></slot>
            </CardTitle>
            <CardBody>
              <slot name="text"></slot>
            </CardBody>
            <CardActions>
              <slot name="button"></slot>
            </CardActions>
          </div>
        </div>
      </div>
      <div class="col-4">
        <div class="card">
          <img :src="image" class="card-img-top" alt="...">
          <div class="card-body">
            <CardTitle>
              <slot name="title"></slot>
            </CardTitle>
            <CardBody>
              <slot name="text"></slot>
            </CardBody>
            <CardActions>
              <slot name="button"></slot>
            </CardActions>
          </div>
        </div>
      </div>
      <div class="col-4">
        <div class="card">
          <img :src="image" class="card-img-top" alt="...">
          <div class="card-body">
            <CardTitle>
              <slot name="title"></slot>
            </CardTitle>
            <CardBody>
              <slot name="text"></slot>
            </CardBody>
            <CardActions>
              <slot name="button"></slot>
            </CardActions>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import { h, defineComponent } from 'vue';

const CardTitle = defineComponent({
  functional: true,
  render() {
    return h('h5', { class: 'card-title' }, this.$slots.default());
  }
});

const CardBody = defineComponent({
  functional: true,
  render() {
    return h('p', { class: 'card-text' }, this.$slots.default());
  }
});

const CardActions = defineComponent({
  functional: true,
  render() {
    return h('a', { class: 'btn btn-primary', href: '#' }, this.$slots.default());
  }
});

export default defineComponent({
  props: {
    image: {
      type: String,
      required: true,
    },
  },
  components: {
    CardTitle,
    CardBody,
    CardActions,
  },
});
</script>