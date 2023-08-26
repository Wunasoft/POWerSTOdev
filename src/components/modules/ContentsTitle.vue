<script setup lang="ts">
  defineProps<{
    strSubTitle: string,
    conParam : string[][]
  }>()
</script>
<template>
  <div class="containerCon">
    <div class="subtitle">&nbsp;{{strSubTitle}}</div>
    <img v-for="conParam in conParam" class="contents" :src=conParam.fname :key="conParam.index">
  </div>
</template>

<style scoped>
.containerCon {
  display: grid;
  grid-template-rows: 5em, 23.75em;
  grid-template-columns: 25em 25em 25em;
  justify-content: center;
  margin-top: 1.9em;
  height: 27.25em;
  background-size: cover;
}

.subtitle {
  grid-column: 1/4;
  grid-row: 1/2;
  vertical-align: bottom;
  height: 1.8em;
  font-size: 1.3em;
  font-family: "Segoe UI";
  font-weight: bold;
  padding-right: 0.6em;
}

.contents {
  height: 23.75em;
  text-align: center;
  width: 23.75em;
  align-self: center;
  justify-content: center;
  flex-grow: 0em;
  padding-right: 4em; 
}
</style>
