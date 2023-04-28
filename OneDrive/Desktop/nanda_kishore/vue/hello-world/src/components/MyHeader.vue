<template>
    
    <h3> {{ authorName }} {{ bookName }}</h3>
    <form>
    <div>
        <label :style="{padding :space + px}">Phone Number :</label>
        <input type="number" v-model="formValues.number">
        <label>NAME :</label>
 <input type="text" v-mode="formValues.name">
    </div>
    <div>
        <label> SELECT SIZE  :</label>
         <select v-model="formValues.size">
        <option> SELECT SIZE</option>
        <option> SMALL </option>
         <option>MEDIUM</option>
        <option>LARGE </option>
         <option> X LARGE</option>
        </SELECT>
    </div>
    </form>
</template>

 
<script>
export default {
    name : 'MyHeader',
    props:{
        bookName: String,
        authorName: String
    },
    data(){

        return{
            space :20,
            formValues : {
        name:"",
        size:"",
        number:""

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
label{
    margin-top: 20%;
}

</style>

