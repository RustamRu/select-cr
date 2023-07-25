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
    <a href="#">
      <Logo class="header__logo logo" />
    </a>
    <button class="header__btn icon-btn">
      <BurgerIco class="icon-btn__icon" />
    </button>
  </header>
</template>

<style lang="scss">
@import "./Header.scss";
</style>