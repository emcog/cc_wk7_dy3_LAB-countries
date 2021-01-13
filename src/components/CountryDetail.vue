<template lang="html">
  <div v-if="country">
    <span>Bananas</span>
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

</style>