<script>
import Header from './components/Header/Header.vue';
import Main from './components/Main/Main.vue';
import SideStat from './components/SideStat/SideStat.vue';

export default {
  components: {
    Header, Main, SideStat
  }
}
</script>

<template>
  <Header />
  <Main />
  <SideStat />
</template>

<style lang="scss">
@import "./styles.scss";
</style>