<script setup>
import axios from "axios";
import { ref } from "vue";

const response = ref();

const getValue = async () => {
  try {
    response.value = await axios.get("/api/test-me");
  } catch (error) {
    // Do something with the error
    console.log(error);
  }
};
</script>

<template>
  <div>
    <h1>
      Hi, I'm Amber. <br />
      I create.
    </h1>
    <router-link to="/test"> Take me to Test page </router-link>
    <button @click.prevent="tiggerEndpoint">Trigger Endpoint</button>
    <p v-if="response">{{ response.data }}</p>
  </div>
</template>
