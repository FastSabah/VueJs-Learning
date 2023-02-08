<template>


        <div class="user">
    {{ data.name }}
    <button v-on:click="getData(data.name)">Check Name</button>
</div>
  
</template>

    
<script>


export default {
    name: "UserF",
    props:{
        data:Object,
        getData:Function
    }

}
</script>

<style scoped>
ul {
    
    text-align: left;
    margin-left: 20px;
    list-style: none;
}
.user{
    background-color: rgb(0, 64, 255);
    padding:10px;
    margin-bottom:10px;
    color:#fafafa;
    text-transform: uppercase;

}
</style>

