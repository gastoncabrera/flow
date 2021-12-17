<template>
  <li class="apartment__item">
    <div class="apartment__background_number">
      <span class="apartment__number">3</span>
    </div>

    <div class="apartment__item_wrap">
      <span class="apartment__item_title">Reserva tu cita</span>

      <span class="apartment__item_description">
        Completa tu reserva y prepárate para la mejor experiencia con un
        psicólogo online.
      </span>
    </div>
  </li>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
@import "@/assets/scss/utils";

.apartment__item {
  display: flex;
}

.apartment__background_number {
  height: 48px;
  min-width: 48px;
  border-radius: 50%;
  background-color: #d8d8d8;
  position: relative;
}

.apartment__number {
  position: absolute;
  left: 50%;
  top: 50%;
  transform: translate(-50%, -50%);
  font-size: 18px;
  line-height: 22px;
  font-weight: 600;
}

.apartment__item_wrap {
  display: flex;
  flex-direction: column;
  margin-left: 41px;
}

.apartment__item_title {
  font-size: 23px;
  line-height: 28px;
  font-weight: 600;
  margin-bottom: 15px;
}

.apartment__item_description {
  font-size: 18px;
  line-height: 27px;
  width: 352px;
}
</style>