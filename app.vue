<template>
  <Button variant="secondary"></Button>
  <Alert></Alert>
  <BsContainer>
    <BsRow>
      <BsCol>
        <BsCard image="/no-photo.jpg">
          <BsCardTitle>Заголовок</BsCardTitle>
          <BsCardBody>Текст текст</BsCardBody>
          <BsCardActions>Кнопка-ссылка</BsCardActions>
        </BsCard>
      </BsCol>
    </BsRow>
  </BsContainer>
</template>

<script>

import {defineComponent} from "vue";
import BsContainer from "~/components/Card/BsContainer.vue";
import BsRow from "~/components/Card/BsRow.vue";
import BsCol from "~/components/Card/BsCol.vue";
import BsCard from "~/components/Card/BsCard.vue";
import BsCardTitle from "~/components/Card/BsCardTitle.vue";
import BsCardBody from "~/components/Card/BsCardBody.vue";
import BsCardActions from "~/components/Card/BsCardActions.vue";

export default defineComponent({
  components: {BsCardActions, BsCardBody, BsCardTitle, BsCard, BsCol, BsRow, BsContainer}
})
</script>
