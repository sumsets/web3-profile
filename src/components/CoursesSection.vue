<template>
<div class="container">
  <div class="courses-section">
    <p class="section-head">Courses</p>
    <div class="buttons">
      <b-button class="c-buton col-4">Active</b-button>
      <b-button class="c-buton col-4">Previous</b-button>
      <b-button class="c-buton col-4">Upcoming</b-button>
    </div>
  </div>
  <div class="scroll-back">
    <div class="scroll-section">
      <p class="p-desc">Rapid Prod.</p>
      <p class="p-desc">second line</p>
    </div>
  </div>
</div>
</template>

<script>
</script>

<style scoped lang="scss">
.container{
  background-color:#F7F7FA;
}
.courses-section{
  background-color: white;
}
.section-head {
  color: #333333;
  text-align: left;
  padding: 20px 0px 0px 20px;
  font-weight: 600;
  font-size: 22px;
  line-height: 30px;
}
.buttons {
  padding-bottom: 6px;
}
.c-buton{
  background-color: white;
  color: #828282;
  border: none;
  font-weight: 400;
  font-size: 16px;
  line-height: 24px;
  margin-top: 8px;
}
.scroll-section{
  width: 270px;
  height: 155px;
  border-radius: 20px;
  background-color: #f7f7fa;
  color: #333333;
  padding-top: 16px;
  margin: 20px;
}
.scroll-back{
  background-color: white;
  padding: 5px;
  margin-top: 1px;
}
.p-desc{
  font-size: 18px;
  line-height: 24px;
  font-weight: 700;
  text-align: left;
  padding-left: 16px;
}
</style>
