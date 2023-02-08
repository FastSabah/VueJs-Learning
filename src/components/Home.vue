<template>
<h1>This is Home.vue Code</h1>
<ul>
    <li v-for="item in users" :key="item.name">
<UserF :data = "item" :getData="getData" />
</li>
</ul>
<h1>{{ text }}</h1>
<div v-html="tag">

</div>
<div v-html="tag2">

</div>
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
    ],
    text:"This is simple Text",
    tag:"<h1>This is my first Heading</h1>",
    tag2:"<h3>This is my second Heading</h3>"
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