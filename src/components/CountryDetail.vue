<template lang="html">
  <div>
    <p><b>Name:</b> {{country.name}}</p>
    <p><b>Capital:</b> {{country.capital}}</p>
    <p><b>Population:</b> {{country.population}}</p>
    <p><b>Languages Spoken:</b> {{country.languages[0].name}}</p>
    <img v-bind:src="country.flag" alt="">
  </div>
</template>

<script>

export default {
  "name": "country-detail",
  "props": ["country"]
}
</script>

<style lang="css" scoped>
div {
  background-color: darkslategrey;
  color: white;
  height: 330px;
  width: 400px;
  padding: 15px;
  border-radius: 1em;
  position: fixed;
  right: 20%;
}

img {
  max-width: 250px;
  height: auto;
}
</style>
