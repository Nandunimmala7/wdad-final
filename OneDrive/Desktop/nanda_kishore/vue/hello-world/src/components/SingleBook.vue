<template>
    <div>
 <label>{{ dessert }}  :</label>  
 <select>
    <option>select desserts</option>
    <option>C C COOKIE</option>
    <option>D C BROWNIE</option>
    <option>CNM PART</option>
 </select>
</div>
</template>
<script>
export default{
    name : "SingleBook",
    props:{
        dessert : String
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