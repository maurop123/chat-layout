<template>
  <v-container fluid class="tallest">
    <v-layout column fill-height reverse>
      <v-flex class="child" v-for="word in words">
        <h1>{{word}}</h1>
      </v-flex>
    </v-layout>
  </v-container>
</template>

<script>
  export default {
    data() {
      return {
        words: ['test', 'toast', 'teeth', 'hair', 'bone', 'skin', 'teeth']
      }
    },
  }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
  font-weight: normal;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}

.tallest {
  height: 100%;
}

.child {
  /* height: 30px; */
}

.child h1 {
  font-size: 100px;
}
</style>
