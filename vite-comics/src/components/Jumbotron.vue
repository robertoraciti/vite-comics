<script></script>
<template>
  <div>
    <img src="../../public/img/jumbotron.jpg" alt="" />
    <label>CURRENT SERIES</label>
  </div>
</template>
<style lang="scss" scoped>
div {
  position: relative;
  img {
    width: 100%;
    height: 300px;
    object-fit: cover;
    object-position: top;
  }

  label {
    color: white;
    background-color: #0282f9;
    padding: 10px;
    // height: 30px;
    position: absolute;
    left: 15%;
    bottom: -5%;
  }
}
</style>
