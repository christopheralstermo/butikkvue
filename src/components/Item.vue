


<script setup lang="ts">
import {ref, onMounted} from "vue";

const itemList = ref([]);


async function getAll(){
  const response = await fetch("http://localhost:5170/ItemApi");
  let result = response.json();
  console.log(result)
}

</script>

<template>
<button @click="getAll">klikk</button>
</template>

<style scoped>

</style>