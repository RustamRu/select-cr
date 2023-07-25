<script>
import CartIco from "../../assets/icons/cart.svg";
import GearIco from "../../assets/icons/gear.svg";
import RubleIco from "../../assets/icons/ruble.svg";
import RyeIco from "../../assets/icons/rye.svg";
import ThreeArrowsIco from "../../assets/icons/three-arrows.svg";

export default {
  components: {
    CartIco, GearIco, RubleIco, RyeIco, ThreeArrowsIco,
  },
  data() {
    return {
      sectors: [
        {
          name: 'Внешняя торговля',
          icon: ThreeArrowsIco,
          districtGrowth: '+19.0',
          totalGrowth: '+17.6',
        },
        {
          name: 'Инвестиции',
          icon: RubleIco,
          districtGrowth: '+8.9',
          totalGrowth: '+4.3',
        },
        {
          name: 'Промышленность',
          icon: GearIco,
          districtGrowth: '+7.5',
          totalGrowth: '+2.9',
        },
        {
          name: 'Розничная торговля',
          icon: CartIco,
          districtGrowth: '+4.0',
          totalGrowth: '+2.6',
        },
        {
          name: 'Сельское хозяйство',
          icon: RyeIco,
          districtGrowth: '+3.1',
          totalGrowth: '-0.6',
        },
      ]
    }
  }
};
</script>

<template>
  <aside class="aside">
    <table class="table">
      <thead>
        <tr>
          <th class="col-heading col-heading--main accent">Рост за 2019 год</th>
          <th class="col-heading accent">Центральная Россия</th>
          <th class="col-heading">Российская Федерация</th>
        </tr>
      </thead>
      <tbody>
        <tr v-for="sector in sectors" class="sector-entry">
          <td class="sector-entry__name">
            <span class="sector-entry__icon"><component :is="sector.icon"/></span> {{ sector.name }}
          </td>
          <td class="sector-entry__grouth-amount accent">{{ sector.districtGrowth }} %</td>
          <td class="sector-entry__grouth-amount">{{ sector.totalGrowth }} %</td>
        </tr>
      </tbody>
    </table>
  </aside>
</template>

<style lang="scss">
@import "./SideStat.scss";
</style>