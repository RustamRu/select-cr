<script>
import StatList from '../StatList/StatList.vue';
import DistrictMap from "../../assets/image/cfd-map.svg";

export default {
  components: {
    StatList, DistrictMap
  }
}
</script>

<template>
  <main class="main">
    <h1 class="main__title">
      <span class="main__title-accent">Центральная россия —</span> 1/3 экономики страны
    </h1>
    <StatList />
    <DistrictMap class="main__map"/>
  </main>
</template>

<style lang="scss">
@import "./Main.scss";
</style>