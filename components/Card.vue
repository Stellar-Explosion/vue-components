<template>
  <div class="container text-center">
    <div class="row">
      <div class="col-4">
        <div class="card">
          <img :src="image" class="card-img-top" alt="...">
          <div class="card-body">
            <h5 class="card-title">
              <slot>Заголовок</slot>
            </h5>
            <p class="card-text">
              <slot>Текст</slot>
            </p>
            <a href="#" class="btn" :class="`btn-${variant} btn-${size}`">
              <slot>Кнопка-ссылка</slot>
            </a>
          </div>
        </div>
      </div>
      <div class="col-4">
        <div class="card">
          <img :src="image" class="card-img-top" alt="...">
          <div class="card-body">
            <h5 class="card-title">
              <slot>Заголовок</slot>
            </h5>
            <p class="card-text">
              <slot>Текст</slot>
            </p>
            <a href="#" class="btn" :class="`btn-${variant} btn-${size}`">
              <slot>Кнопка-ссылка</slot>
            </a>
          </div>
        </div>
      </div>
      <div class="col-4">
        <div class="card">
          <img :src="image" class="card-img-top" alt="...">
          <div class="card-body">
            <h5 class="card-title">
              <slot>Заголовок</slot>
            </h5>
            <p class="card-text">
              <slot>Текст</slot>
            </p>
            <a href="#" class="btn" :class="`btn-${variant} btn-${size}`">
              <slot>Кнопка-ссылка</slot>
            </a>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    image: {
      type: String,
      required: true,
    },
    variant: {
      type: String,
      default: "primary"
    },
    size: {
      type: String,
      default: "lg"
    },
    disabled: {
      type: Boolean,
      default: false
    }
  },

  setup(props) {
    return {
      image: props.image,
      variant: props.variant,
      disabled: props.disabled
    };
  },
};
</script>