<script>
export default {
  props: {
    thumb: String,
    series: String,
  },
};
</script>
<template>
  <div class="card">
    <img :src="thumb" alt="" />
    <p>{{ series }}</p>
  </div>
</template>
<style lang="scss">
.card {
  width: 16%;
  height: 200px;
  margin-top: 30px;

  img {
    width: 100%;
    height: 150px;
    object-fit: cover;
    object-position: top;
  }
  p {
    margin: 10px 0;
    padding: 0;
    color: white;
  }
}
</style>
