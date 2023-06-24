<template>
  <div>
    <product-list :products="products"/>
  </div>
</template>

<script>
import products from '@/data/products';
// eslint-disable-next-line import/extensions
import productList from '@/components/ProductList';

export default {
  name: 'App',
  components: { productList },

  data() {
    return {
      products,
    };
  },
};
</script>
