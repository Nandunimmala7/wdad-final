<template>

   <div v-for="book of books.books" :key="book.id">
    {{ book.title }} 
  </div>
  <form>
  <div>
    <label> TOPPINGS  :</label>
 <select  v-model="formValues.toppings">
 <option> CHOOSE TOPPINGS</option>
 <option> PEPPERORNI </option>
 <option>CHICKEN</option>
 <option>VEG </option>
 <option> MEATS </option>
 </SELECT>
  </div>
  </form>  
</template>
<script>



export default{
  
     name :'BookBox',
     props: {
        books : Array
     },
     data(){
        return{
            formValues:{
                toppings : []
            }
        }
     }
     
}
</script>
<style scoped>
div{
    text-align: center;
    padding :30px;
    border:1px solid black;
}

</style>
