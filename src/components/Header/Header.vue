<script>
import Logo from "../../assets/image/logo.svg";
import BurgerIco from "../../assets/icons/burger.svg";

export default {
  components: {
    Logo, BurgerIco
  }
};
</script>

<template>
  <header class="header">
    <Logo />
    <button class="header__btn burger-btn">
      <BurgerIco class="burger-btn__icon" />
    </button>
  </header>
</template>

<style lang="scss">
@import "./Header.scss";
</style>