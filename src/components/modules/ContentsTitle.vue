<template>
  <div class="containerIndex">
    <div class="subtitle">&nbsp;{{strDataProps.strTitle}}</div>
    <img class="contents" src="../../images/{{strDataProps.imgName0}}" />
    <img class="contents" src="../../images/{{strDataProps.imgName1}}" />
    <img class="contents" src="../../images/{{strDataProps.imgName2}}" />
  </div>
</template>

<script lang="ts">
  //import { ref } from "vue"
  //const strTitle:string[]
  
  export default {
    //setup() {
    props:
      ["strDataProps"]
      
    //} //= ref(["NPL 투자사례","investment11.png","investment12.png","notice.png"]);
  };
</script>
<style>
.containerIndex {
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
