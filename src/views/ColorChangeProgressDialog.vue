<template>
  <div class="outer">
    1/22
    <div class="inner">1/22</div>
  </div>
</template>

<script>
export default {
}
</script>

<style scoped>
@-webkit-keyframes move {
  0%{
    -webkit-clip-path:polygon(0% 0%,0% 100%,0% 100%,0% 0%);
  }
  100%{
    -webkit-clip-path:polygon(0% 0%,0% 100%,100% 100%,100% 0%);
  }
}
div{
  height: 50px;
  line-height: 50px;
  text-align: center;
  font-size: 2px;
}
.outer{
  position: relative;
}
.inner{
  position: absolute;
  left: 0;
  top: 0;
  right: 0;
  bottom: 0;
  color: red;
  background-color: blue;
  -webkit-clip-path:polygon(0% 0%,0% 100%,100% 100%,100% 0%);
  animation: move 1s linear 0s;
}
</style>
