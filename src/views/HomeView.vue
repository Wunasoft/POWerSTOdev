<script setup lang="ts">

  import MainImage from '../components/modules/MainImage.vue';
  import ContentsTitle from '../components/modules/ContentsTitle.vue';

  var imgPath:string = "../../src/images/";
data(){
  const strParam0 = [
    {fname: imgPath+"notice2.png", hLink: "230822001", cname: "염창동주택", erate: "25"},
    {fname: imgPath+"subTitle1.png", hLink: "230822002", cname: "신사동상가", erate: "28"},
    {fname: imgPath+"subTitle2.png", hLink: "230822003", cname: "홍대앞주택", erate: "35"}
  ];
  const strParam1= [
    {fname: imgPath+"investment21.png",  hLink: "230822001",  cname: "염창동주택",  erate: "25"}, 
    {fname: imgPath+"investment22.png", hLink: "230822002", cname: "신사동상가", erate: "28"}, 
    {fname: imgPath+"investment23.png", hLink: "230822003", cname: "홍대앞주택", erate: "35"}
  ];
};
</script>

<template>
  <main>
    <MainImage/>
    <ContentsTitle strSubTitle="NPL 투자현황" :conParam = "strParam0"/>
    <ContentsTitle strSubTitle="투자상품" :conParam="strParam1"/>
  </main>
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
</style>