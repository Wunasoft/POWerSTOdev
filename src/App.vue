<script setup lang="ts">
// import { RouterLink, RouterView } from 'vue-router'
import {RouterLink} from 'vue-router'

import HeaderLogo from './components/modules/HeaderLogo.vue';
import MainImage from './components/modules/MainImage.vue';
import ContentsTitle from './components/modules/ContentsTitle.vue';

</script>

<template>
  <HeaderLogo/>
  <MainImage/>
  <ContentsTitle msgCon="NPL 투자현황"  imgName0="subTitle1.png" imgName1="subTitle2.png" imgName2="subTItle3.png"/>
  <ContentsTitle msgCon="투자"  imgName0="subTitle1.png" imgName1="subTitle2.png" imgName2="subTItle3.png"/>
</template>

<style scoped>
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

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }

  nav {
    text-align: left;
    margin-left: -1rem;
    font-size: 1rem;

    padding: 1rem 0;
    margin-top: 1rem;
  }
}
</style>
