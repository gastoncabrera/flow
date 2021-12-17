<template>
  <div class="hero">
    <div class="hero__container custom_container custom_container--xl">
      <h1 class="hero__title">Gánate un apartamento en Miami</h1>

      <p class="hero__info">
        Aplica al sorteo con 0,034 ETH.
        <br />
        Sortearemos el 31 de Diciembre de 2021.
      </p>

      <div class="tickets_bar">
        <div class="tickets_bar__sold"></div>

        <div class="tickets_bar__total"></div>
      </div>

      <span class="hero__tickets">
        Faltan 593 / 1,200 participantes para cerrar el sorteo
      </span>

      <div class="hero__buttom">
        <v-btn class="hero__buttom_wallet"> Connect wallet </v-btn>

        <div class="hero__buttom_info">Descubre cómo funciona</div>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
@import "@/assets/scss/utils";

.hero__container {
  margin-top: 164px;
  margin-bottom: 132px;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}

.hero__title {
  font-size: 56px;
  line-height: 67px;
  font-weight: 400;
}

.hero__info {
  margin-top: 29px;
  margin-bottom: 36px;
  font-size: 16px;
  line-height: 19px;
  font-weight: 400;
  text-align: center;
}

.tickets_bar {
  position: relative;
  width: 410px;
  height: 17px;
  border-radius: 8.5px;
  overflow: hidden;
}

.tickets_bar__sold {
  position: absolute;
  left: 0;
  top: 0;
  width: 50%;
  height: 100%;
  background-color: #d8d8d8;
  border-radius: 8.5px;
  z-index: 10;
}

.tickets_bar__total {
  position: absolute;
  left: 0;
  top: 0;
  width: 100%;
  height: 100%;
  background-color: #d8d8d8;
  opacity: 0.2000000029802322;
}

.hero__tickets {
  margin-top: 20px;
}

.hero__buttom {
  display: flex;
  padding-top: 40px;
  align-items: center;
}

.hero__buttom_wallet.hero__buttom_wallet.hero__buttom_wallet {
  margin-right: 24px;
  font-size: 16px;
  line-height: 19px;
  text-transform: none;
  font-weight: 400;
  background-color: #d8d8d8;
  border: 1px solid #979797;
  border-radius: 22.5px;
  padding: 20px 40px;
}

.hero__buttom_info {
  font-size: 16px;
  line-height: 19px;
  font-weight: 400;
}
</style>