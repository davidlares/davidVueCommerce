<template>
  <div :key="product.id" class="col-xs-12 col-sm-10 col-md-4">
    <div class="card">
        <header class="bg-primary padding white-font">Product #{{product.id}}</header>
        <div class="card-body">
          <h2 class="card-title">
            <a :href="'/products/' + product.id">{{product.title}}</a>
          </h2>
          <h4 class="card-subtitle">{{product.humanPrice}}</h4>
          <p class="card-text">{{product.description}}</p>
        </div>
    </div>
  </div>
</template>
<script>
export default {
  name: "product-card",
  props: {
    product: {
      type: Object
    }
  },
  data() {
    return {

    }
  }
}
</script>
<style lang="scss" scoped>
</style>
