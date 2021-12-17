<template>
  <div class="questions">
    <div class="questions__container custom_container custom_container--xl">
      <div class="questions__title">Preguntas frecuentes</div>
      <div class="questions__wrap">
        <div class="questions__item">
          <span class="questions__item_title"
            >Titulo de una primera pregunta frecuente</span
          >
          <p class="questions__item_description">
            Esta es una respuesta Esta es una respuesta Esta es una respuesta
            Esta es una respuesta Esta es una respuesta Esta es una respuesta
            Esta es una respuesta
          </p>
        </div>
        <div class="line"></div>
        <div class="questions__item">
          <span class="questions__item_title"
            >Titulo de una primera pregunta frecuente</span
          >
          <p class="questions__item_description">
            Esta es una respuesta Esta es una respuesta Esta es una respuesta
            Esta es una respuesta Esta es una respuesta Esta es una respuesta
            Esta es una respuesta
          </p>
        </div>
        <div class="line"></div>
        <div class="questions__item">
          <span class="questions__item_title"
            >Titulo de una primera pregunta frecuente</span
          >
          <p class="questions__item_description">
            Esta es una respuesta Esta es una respuesta Esta es una respuesta
            Esta es una respuesta Esta es una respuesta Esta es una respuesta
            Esta es una respuesta
          </p>
        </div>
        <div class="line"></div>
        <div class="questions__item">
          <span class="questions__item_title"
            >Titulo de una primera pregunta frecuente</span
          >
          <p class="questions__item_description">
            Esta es una respuesta Esta es una respuesta Esta es una respuesta
            Esta es una respuesta Esta es una respuesta Esta es una respuesta
            Esta es una respuesta
          </p>
        </div>
        <div class="line"></div>
      </div>
      <div class="questions__more">Ver más preguntas frecuentes</div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
@import "@/assets/scss/utils";

.questions__container {
  margin-top: 95px;
}

.questions__title {
  font-size: 26px;
  line-height: 31px;
  font-weight: 400;
  margin-bottom: 70px;
}

.questions__item {
  display: flex;
  margin-top: 38px;
}

.questions__item_title {
  font-size: 20px;
  line-height: 24px;
  font-weight: 600;
  width: 100%;
  max-width: 364px;
  margin-right: 117px;
}

.questions__item_description {
  font-size: 16px;
  line-height: 25px;
  font-weight: 400;
  width: 100%;
  max-width: 469px;
}

.line {
  border: 1px solid #f2f3f6;
}
.questions__more {
  margin-top: 46px;
  font-size: 16px;
  line-height: 19px;
  font-weight: 400;
}
</style>