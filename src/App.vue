<template>
  <div id="app">
  {{ title }}

  <ul>
    <li v-for="entry in entries" :key="entry.id">
    {{ entry.description }}
    </li>
  </ul>
  </div>
</template>

<script>

export default {
  name: 'App',
  data() {
    return {
      title: "Welcome to Opportunity",
      entries: [
        {
          id: 1,
          description: "Basisbeschäftigung Besuch",
          daytime: "14.00 Uhr"
        },
        {
          id: 2,
          description: "Sozialamt Dietikon",
          daytime: "15.30 Uhr"
        }
      ]
    }
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
