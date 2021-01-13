<template lang="html">
  <div>
    <select id="country" v-model="selectedCountry" >
            <option disabled value ="Choose your country">Choose your country</option>
            <option v-for="(country, index) in countries" v-bind:value=country>{{ country.name }}</option>
    </select>
  </div>
</template>

<script>
import ListItem from './ListItem.vue';

export default {
    name:'countries-list',
    props: ['countries'],
    components: {
        "list-item": ListItem
    }
}
</script>

<style lang="css" scoped>

</style>

 <!-- 
    <ul>
        <list-item v-for="(country, index) in countries" :country="country" :key="index"></list-item>
    </ul>
-->

<!-- 
    <select id="currency" v-model="exchangeRate">
        <option disabled value ="this is a val">Choose your currency</option>
        <option v-for="(rate, currency) in currencies" v-bind:value=rate>{{ currency }}</option>
    </select>
-->