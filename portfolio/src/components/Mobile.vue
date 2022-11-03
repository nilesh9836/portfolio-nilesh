<template>
  <v-container class="justify-content-end" >
  <div class="center">
  <div class="mobile">
    <div class="screen active"></div>
    <div class="home"></div>
    <div class="inner"></div>
  </div>
</div>
</v-container>
</template>

<script>
export default {

}
</script>

<style>
/* body
{
  margin: 0;
  padding: 0;
} */
/* .center
{
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%,-50%);
} */
.mobile
{
  width: 276px;
  height: 555px;
  background: #fff;
  border-radius: 30px;
  border: 2px solid rgba(0,0,0,.3);
  box-sizing: border-box;
  box-shadow: inset 0 0 8px rgba(0,0,0,.3);
}
.screen
{
  background: #262626;
  width: 256px;
  height: 430px;
  margin: 58px auto;
  overflow: hidden;
}
.screen
{
  background-size: cover;
  background-color:hsla(50, 33%, 25%, 0.75);

}
.home
{
  transform: translate(112px,-45px);
  width: 40px;
  height: 40px;
  border-radius: 50%;
  background: #fff;
  border: 2px solid #cecece;
  box-sizing: border-box;
  cursor: pointer;
  box-shadow: inset 0 0 7px rgba(0,0,0,.1);
}
.inner
{
  width: 40px;
  height: 4px;
  border-radius: 2px;
  background: #262626;
  box-sizing: border-box;
}
.inner:before
{
  content: '';
  background: #262626;
  width: 8px;
  height: 8px;
  border-radius: 50%;
}
.inner:after
{
  content: '';
  background: #262626;
  width: 6px;
  height: 6px;
  border-radius: 50%;
}
</style>