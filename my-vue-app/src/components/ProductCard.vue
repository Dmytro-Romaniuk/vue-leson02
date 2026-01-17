<template>
  <div class="product-card">
    <img :src="image" :alt="name" class="product-img" />
    <h2>{{ name }}</h2>
    <p>{{ description }}</p>
    <p class="price">{{price}}</p>
    <button class="buy-button">Купить</button>
  </div>
</template>

<script>
export default {
  props: {
    name: String,
    description: String,
    price: Number,
    image: String,
  },
};
</script>

<style scoped>
.product-card {
  max-width: 300px;
  border: 1рх solid #e0e0e0;
  border-radius: 12px;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
  text-align: center;
}
.product-img {
  width: 100%;
  height: 200px;
}
.price {
  font-size: 18px;
  font-weight: bold;
  color: #28a745;
}
.buy-button {
  background-color: #007bff;
  color: #fff;
  font-weight: bold;
  border: none;
  border-radius: 6px;
  padding: 10px 20px;
  cursor: pointer;
  margin-bottom: 20px;
}
button:hover {
  background: #0056b3;
}
</style>
