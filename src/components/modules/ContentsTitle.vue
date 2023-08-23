<script setup lang="ts">
  defineProps<{
    msgCon: string,
    imgName0: string,
    imgName1: string,
    imgName2: string
    // imgNames:string[3]
  }>()
</script>

<template>
  <div class="containerCon">
    <div class="subtitle">&nbsp;{{msgCon}}</div>
    <img class="contents" src="../../images/{{imgName0}}" />
    <img class="contents" src="../../images/{{imgName1}}" />
    <img class="contents" src="../../images/{{imgName2}}" />
    <!-- <img v-for="imgName in imgNames" class="contents" src="../../imgaes/{{ imgName}}" :key="imgName"> -->
  </div>
</template>

<style scoped>
.containerCon {
  display: grid;
  grid-template-rows: 80px, 380px;
  grid-template-columns: 400px 400px 400px;
  justify-content: center;
  margin-top: 30px;
  height: 440px;
  background-size: cover;
}

.subtitle {
  grid-column: 1/4;
  grid-row: 1/2;
  vertical-align: bottom;
  height: 36px;
  font-size: 25px;
  font-family: "Segoe UI";
  font-weight: bold;
  padding-right: 10px;
}

.contents {
  height: 380px;
  text-align: center;
  width: 380px;
  align-self: center;
  justify-content: center;
  flex-grow: 0;
  padding-right: 4em;
}
</style>
