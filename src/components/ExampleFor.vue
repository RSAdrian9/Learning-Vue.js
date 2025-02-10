<template>
    <ul>
        <li v-for="country in countries" :key="country.code">{{ country.name }}</li>
        <!-- Lo hemos abreviado, pero se podría no omitir la propiedad v-bind -->
        <!-- <li v-for="country in countries" v-bind:key="country">{{ country }}</li> -->
        <!-- Otra forma de ponerlo -->
        <!--<li v-for="(country, index) in countries" v-bind:key="index">{{ country }}</li>-->
    </ul>
</template>

<script lang="ts" setup>
import {Ref, ref } from 'vue'

interface ICountry {
    code: string,
    name: string
}
let countries:Ref<Array<ICountry>> = ref([
    {
        code: 'es',
        name: 'España'
    },
    {
        code: 'fr',
        name: 'Francia'
    },
    {
        code: 'it',
        name: 'Italia'
    },
    {
        code: 'pt',
        name: 'Portugal'
    }

])
</script>

<style scoped>

</style>