<template>
  <div id="app">

  </div>
</template>

<script>

export default {
  name: 'app',
  data() {
    return {
      countries: []
    };
  },
  mounted() {
    fetch('countries_data.json')
    .then(response => response.json())
    .then(countries => this.countries = countries);
  },
  components: {

  }
}
</script>

<style>
#app {

}
</style>
