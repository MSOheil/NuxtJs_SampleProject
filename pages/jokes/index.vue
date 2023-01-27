<template>
  <div :v-for="joke in jokes">
    <Jokes :joke="joke.joke" :id="joke.id" />
  </div>
</template>

<script>

import axios from "axios"
import { ref } from 'vue';
export default {
  comments: {
    Jokes: Jokes,
  },
  async setup() {

    const jokes = ref([]);
    const config = {
      headers: {
        Accept: "application/json"
      }
    }
    var result = await axios.get('https://icanhazdadjoke.com/search', config);
    jokes.value = result.data.results;
    console.log(jokes.value);
  }

}
</script>

<style>

</style>