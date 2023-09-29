<script setup>
import { useRoute } from 'vue-router';
import coffeeblack from './coffeeblack.vue'
import coffeeblue from './coffeeblue.vue'
import coffeegreen from './coffeegreen.vue'
import coffeered from './coffeered.vue'
import coffeeyellow from './coffeeyellow.vue'

const route = useRoute()
const id = parseInt(route.params.id)


</script>

<template>
    <body>
        <div v-if="id==0">
            <coffeeblack />
        </div>
    </body>

    <body>
        <div v-if="id==1">
            <coffeeblue/>
    </div>
    </body>

    <body>
        <div v-if="id==2">
            <coffeegreen />
    </div>
    </body>

    <body>
        <div v-if="id==3">
            <coffeered/>
    </div>
    </body>

    <body>
        <div v-if="id==4">
            <coffeeyellow />
    </div>
    </body>

</template>

<style scoped>
body{
    text-align: center;
}
</style>