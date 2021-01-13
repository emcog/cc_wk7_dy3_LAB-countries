<template lang="html">
  <div class="country-details" v-if="country">
    <h2>{{ country.name }}</h2>
    <span>{{ country.capital }}</span>
    <span>{{ country.population }}</span>
  </div>
</template>

<script>
export default {
  name: "country-detail",
  props:['country'] //?????????????????
}
</script>

<style>
  .country-detail {
    float: right;
  }
</style>