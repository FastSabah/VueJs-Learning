<template>
<h1>This is Home.vue Code</h1>
<ul>
    <li v-for="item in users" :key="item.name">
<UserF :data = "item" :getData="getData" />
</li>
</ul>
</template>

<script>
import UserF from './User.vue'
export default {
    name: "HomeF",
    components: {
        UserF
    },data() {

return {
    users: [{
            name: "urwa",
            email: "urwa@test.com"
        },
        {
            name: "usman",
            email: "usman@test.com"
        },
        {
            name: "sabah",
            email: "sabah@test.com"
        },
        {
            name: "farah",
            email: "farah@test.com"
        },
    ]
}
},
methods:{

    getData(item){

alert(item);
    }
}

}
</script>
<style scoped>
ul {
    text-align: left;
    margin-left: 20px;
    list-style: none;
}

</style>