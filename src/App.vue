// sr/App.vue
<script>
import Header from './components/Header/Header.vue';
import StatList from './components/StatList/StatList.vue';
import SideStat from './components/SideStat/SideStat.vue';
import DistrictMap from "./assets/image/cfd-map.svg";

export default {
  components: {
    Header, StatList, SideStat, DistrictMap
  }
}
</script>

<template>
  <Header />
  <h1 class="page-title">
    <span class="accent">Центральная россия —</span> 1/3 экономики страны
  </h1>
  <StatList />
  <SideStat />
  <DistrictMap />
</template>

<style lang="scss">
@import "./styles.scss";
</style>