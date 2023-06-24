<template>
    <li class="catalog__item" v-for="(product, index) in products" :key="index">
      <a class="catalog__pic" href="#">
        <img :src="product.image"  :alt="product.title">
      </a>

      <h3 class="catalog__title">
        <a href="#">
          {{ product.title }}
        </a>
      </h3>

      <span class="catalog__price">
              {{ product.price }} руб.
            </span>

      <ul class="colors colors--black">
        <li class="colors__item">
          <label for="color-1" class="colors__label">
            <input
              id="color-1"
              class="colors__radio sr-only"
              type="radio"
              name="color-1"
              value="#73B6EA"
              checked=""
            />
            <span class="colors__value" style="background-color: #73B6EA;">
                  </span>
          </label>
        </li>
        <li class="colors__item">
          <label for="color-1" class="colors__label">
            <input class="colors__radio sr-only" type="radio" name="color-1" value="#8BE000">
            <span class="colors__value" style="background-color: #8BE000;">
                  </span>
          </label>
        </li>
        <li class="colors__item">
          <label  for="color-1" class="colors__label">
            <input class="colors__radio sr-only" type="radio" name="color-1" value="#222">
            <span class="colors__value" style="background-color: #222;">
                  </span>
          </label>
        </li>
      </ul>
    </li>
</template>

<script>
export default {
  name: 'product-item',
  props: ['products'],
};
</script>

<style scoped>

</style>
