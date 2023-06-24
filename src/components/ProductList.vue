<template>
  <div>
    <section class="catalog">

      <ul class="catalog__list">
          <product-item :products="products"/>
      </ul>
      <ul class="catalog__pagination pagination">
        <li class="pagination__item">
          <a class="pagination__link pagination__link--arrow pagination__link--disabled"
             aria-label="Предыдущая страница">
            <svg width="8" height="14" fill="currentColor">
              <use xlink:href="#icon-arrow-left"></use>
            </svg>
          </a>
        </li>
        <li class="pagination__item">
          <a class="pagination__link pagination__link--current">
            1
          </a>
        </li>
        <li class="pagination__item">
          <a class="pagination__link" href="#">
            2
          </a>
        </li>
        <li class="pagination__item">
          <a class="pagination__link" href="#">
            3
          </a>
        </li>
        <li class="pagination__item">
          <a class="pagination__link" href="#">
            4
          </a>
        </li>
        <li class="pagination__item">
          <a class="pagination__link" href="#">
            ...
          </a>
        </li>
        <li class="pagination__item">
          <a class="pagination__link" href="#">
            10
          </a>
        </li>
        <li class="pagination__item">
          <a class="pagination__link pagination__link--arrow" href="#"
             aria-label="Следующая страница">
            <svg width="8" height="14" fill="currentColor">
              <use xlink:href="#icon-arrow-right"></use>
            </svg>
          </a>
        </li>
      </ul>
    </section>
  </div>
</template>

<script>
// eslint-disable-next-line import/extensions
import productItem from '@/components/ProductItem';

export default {
  name: 'product-list',
  components: { productItem },

  props: ['products'],
};
</script>

<style scoped>

</style>
