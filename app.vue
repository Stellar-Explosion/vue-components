<template>
  <Button variant="secondary"></Button>
  <Alert></Alert>
  <BsContainer>
    <BsRow>
      <BsCol>
        <BsCard image="/no-photo.jpg" alt="...">
          <BsCardTitle>Заголовок</BsCardTitle>
          <BsCardBody>Текст текст</BsCardBody>
          <BsCardActions>Кнопка-ссылка</BsCardActions>
        </BsCard>
      </BsCol>
    </BsRow>
    <BsRow>
      <BsCol>
        <BsCarousel>
          <BsCarouselItem image="/no-photo.jpg" active></BsCarouselItem>
          <BsCarouselItem image="/no-photo-slide2.jpg"></BsCarouselItem>
          <BsCarouselItem image="/no-photo-slide3.jpg"></BsCarouselItem>
          <BsCarouselControlPrev target="carouselExample"></BsCarouselControlPrev>
          <BsCarouselControlNext target="carouselExample"></BsCarouselControlNext>
        </BsCarousel>
      </BsCol>
    </BsRow>
  </BsContainer>
</template>

<script>

import {defineComponent} from "vue";
import BsContainer from "~/components/BsContainer.vue";
import BsRow from "~/components/BsRow.vue";
import BsCol from "~/components/BsCol.vue";
import BsCard from "~/components/Card/BsCard.vue";
import BsCardTitle from "~/components/Card/BsCardTitle.vue";
import BsCardBody from "~/components/Card/BsCardBody.vue";
import BsCardActions from "~/components/Card/BsCardActions.vue";
import BsCarousel from "~/components/Carousel/BsCarousel.vue";
import BsCarouselInner from "~/components/Carousel/BsCarouselInner.vue";
import BsCarouselItem from "~/components/Carousel/BsCarouselItem.vue";
import BsCarouselControlPrev from "~/components/Carousel/BsCarouselControlPrev.vue";
import BsCarouselControlNext from "~/components/Carousel/BsCarouselControlNext.vue";

export default defineComponent({
  components: {
    BsCarouselControlNext,
    BsCarouselControlPrev,
    BsCarouselItem,
    BsCarouselInner, BsCarousel, BsCardActions, BsCardBody, BsCardTitle, BsCard, BsCol, BsRow, BsContainer}
})
</script>
