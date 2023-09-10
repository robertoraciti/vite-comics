<script>
export default {
  data() {
    return {
      links: [
        "characters",
        "comics",
        "movies",
        "tv",
        "games",
        "collectibles",
        "fans",
        "news",
        "shop",
      ],
    };
  },
};
</script>

<template>
  <header class="header">
    <div class="header-contents container">
      <div class="logo">
        <img src="../../public/img/dc-logo.png" alt="" srcset="" width="70" />
      </div>
      <ul>
        <li v-for="link in links">{{ link.toUpperCase(link) }}</li>
      </ul>
    </div>
  </header>
</template>

<style lang="scss" scoped>
header {
  background-color: white;
}

.header-contents {
  height: 120px;
  display: flex;
  justify-content: space-between;
  align-items: center;
  ul {
    list-style-type: none;
    li {
      display: inline-block;
      margin-left: 1rem;
      font-size: 0.8rem;
      color: rgb(49, 49, 49);
    }
  }
}
</style>
