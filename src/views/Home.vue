<template>
  <div id="body" >
      <HomeMain1 />
      <HomeMain2 />
      <HomeMain3 />
      <HomeFooter />

  </div>
</template>

<script>
import HomeMain1 from "@/components/homeMain1"
import HomeMain2 from "@/components/homeMain2"
import HomeMain3 from "@/components/homeMain3"
import HomeFooter from "@/components/HomeFooter"

export default {
  components :{
      HomeMain1,
      HomeMain2,
      HomeMain3,
      HomeFooter,

  }
}

</script>

<style>
  .main1 {
    height: 600px;
    width: 50%;
    background-image: url("../assets/mainbody1.png");
    background-repeat: no-repeat;
    background-size: 100% 100%;
    float: left;
  }
  .main2 {
    border-style: ridge;
    height: 600px;
    margin-left: 30px;
    width: 23%;
    float: left;
    background-color: #F0FFFF;
  }
  .main3 {
    border-style: ridge;
    height: 600px;
    margin-left: 41px;
    width: 23%;
    float: left;
    background-color: #F0FFFF;
  }

  #body {
  height: 800px;
  padding: 30px;
  margin-left:30px;
  margin-right:30px;
  width: 97%;
  float: left;
  background-color: #F0F8FF;
}
</style>