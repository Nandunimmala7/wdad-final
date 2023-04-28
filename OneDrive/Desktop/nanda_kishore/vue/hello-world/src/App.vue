<template>
  <MyHome />
  <!-- <div class="tittle">
    <h1 v-bind:style="{color:Acolor}">{{ name }}</h1>
    <p v-bind:style="{color:Bcolor, font: Afont}">{{ caption }}</p>
  </div>
  <HelloWorld />
  <MyHeader bookName="ORDER" authorName="START YOUR"/>
  <BookBox :books= "books"/>
  <SingleBook dessert="desserts"/> -->
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
// import MyHeader from './components/MyHeader.vue'
// import BookBox from './components/BookBox.vue'
// import SingleBook from './components/SingleBook.vue'
import MyHome from "./components/MyHome.vue";

export default {
  name: "App",
  components: {
    MyHome,
  },
  data() {
    return {
      // books : [],
      // name : "M.D.PIZZAS",
      // caption : "fresh&hot",
      // Acolor : "green",
      // Bcolor : "red",
      // Afont : "italic"
    };
  },
  methods: {
    // async fetchBooks(){
    //   const res = await fetch("https://upadhayay.github.io/db.jso")
    //   const data = await res.json()
    //   console.log(data)
    //   return data
    // }
  },
  // async created(){
  //   this.books =await this.fetchBooks()
  // }
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
.tittle {
  border: 3px solid blue;
  margin-top: 0px;
  padding: 20px;
}
</style>
