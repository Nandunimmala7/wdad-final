<template>
  <div>
    <h1>Pizza Menu</h1>
    <ul>
      <li v-for="pizza in pizzas" :key="pizza.id">
        <h2>{{ pizza.name }}</h2>
        <p>Size: {{ pizza.size }}</p>
        <p>Price: ${{ pizza.price }}</p>
        <p>Toppings: {{ pizza.toppings.join(", ") }}</p>
        <p>Average Review: {{ pizza.avgReview }}/5</p>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: "MyHome",
  data() {
    return {
      pizzas: [],
    };
  },
  mounted() {
    this.fetchPizzas();
  },
  methods: {
    fetchPizzas() {
      fetch("http://localhost:3000/api/getPizzas")
        .then((response) => response.json())
        .then((data) => {
          this.pizzas = data;
        })
        .catch((error) => {
          console.log(error);
        });
    },
  },
};
</script>
