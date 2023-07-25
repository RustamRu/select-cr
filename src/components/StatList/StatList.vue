<script>
export default {
  data() {
    return {
      categories: [
        {
          name: 'Деньги',
          subcategories: [
            { amount: '73%', name: 'финансовых влияний' },
            { amount: '53%', name: 'накопленных прямых иностранных инвестиций' },
            { amount: '29%', name: 'инвестиций в основной капитал' },
          ]
        },
        {
          name: 'Производство',
          subcategories: [
            { amount: '35%', name: 'валового регионального продукта' },
            { amount: '35%', name: 'обрабатывающей промышленности' },
            { amount: '28%', name: 'продукци сельского хозяйства' },
          ]
        },
        {
          name: 'Рынок',
          subcategories: [
            { amount: '54%', name: 'внешней торговли' },
            { amount: '35%', name: 'розничной торговли' },
          ]
        },
      ]
    }
  }
};
</script>

<template>
  <div class="categories-block">
    <article class="categories-block__col category" v-for="category in categories">
      <h2 class="category__title">{{ category.name }}</h2>
      <ul v-for="subcategory in category.subcategories" class="category__subcategories">
        <li class="subcategory">
          <span class="subcategory__amount">{{ subcategory.amount }}</span> {{ subcategory.name }}
        </li>
      </ul>
    </article>
  </div>
</template>

<style lang="scss">
@import "./StatList.scss";
</style>


