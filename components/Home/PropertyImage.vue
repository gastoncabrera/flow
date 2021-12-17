<template>
  <div class="property">
    <div class="property__container custom_container custom_container--xxxl">
      <div class="property__wrap">
        <img
          src="Gray.jpg"
          alt=""
          class="property__image property__image--one"
        />

        <img
          src="Gray.jpg"
          alt=""
          class="property__image property__image--two"
        />

        <img
          src="Gray.jpg"
          alt=""
          class="property__image property__image--three"
        />

        <img
          src="Gray.jpg"
          alt=""
          class="property__image property__image--four"
        />

        <img
          src="Gray.jpg"
          alt=""
          class="property__image property__image--five"
        />

        <v-btn class="property__button">Mira la propiedad</v-btn>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.property {
  height: 100%;
  width: 100%;
}

.property__wrap {
  position: relative;
  width: 100%;
  height: 100%;
  display: grid;
  justify-content: center;
  grid-template-columns: repeat(3, 1fr);
  grid-template-areas: "one two three" "one four five ";
  gap: 10px;
  border-radius: 15px;
  overflow: hidden;
}

.property__image {
  width: 100%;
  height: 100%;
  object-fit: cover;
}

.property__image--one {
  grid-area: one;
}

.property__image--two {
  grid-area: two;
}

.property__image--three {
  grid-area: three;
}

.property__image--four {
  grid-area: four;
}

.property__image--five {
  grid-area: five;
}

.property__button.property__button.property__button {
  position: absolute;
  right: 29px;
  bottom: 22px;
}
</style>