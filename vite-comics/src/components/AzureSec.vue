<script>
export default {
  data() {
    return {
      images: [
        {
          path: "../../public/img/buy-comics-digital-comics.png",
          description: "Digital Comics",
        },
        {
          path: "../../public/img/buy-comics-merchandise.png",
          description: "DC Merchandise",
        },
        {
          path: "../../public/img/buy-comics-subscriptions.png",
          description: "Subscriptions",
        },
        {
          path: "../../public/img/buy-comics-shop-locator.png",
          description: "Comic Shop Locator",
        },
        {
          path: "../../public/img/buy-dc-power-visa.svg",
          description: "DC Power Visa",
        },
      ],
    };
  },
};
</script>

<template>
  <section class="azure-sec">
    <div class="container">
      <div v-for="image in images">
        <img :src="image.path" alt="" srcset="" width="45" />
        <span>{{ image.description }}</span>
      </div>
    </div>
  </section>
</template>

<style lang="scss" scoped>
.azure-sec {
  background-color: #0282f9;
  height: 150px;
  div {
    z-index: 1;
    height: 100%;
    display: flex;
    justify-content: space-around;
    align-items: center;
    color: white;

    img {
      margin-right: 1rem;
      width: 50px;
      height: 60px;
    }
  }
}
</style>
