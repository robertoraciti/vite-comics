<script>
export default {
  data() {
    return {
      links: [
        "Characters",
        "Comics",
        "Movies",
        "Tv",
        "Games",
        "Collectibles",
        "Fans",
        "News",
      ],

      shops: ["Shop DC", "Shop DC Collectibles"],

      helpOptions: [
        "Terms Of Use",
        "Privacy policy (new)",
        "Ad Choices",
        "Advertising",
        "Jobs",
        "Subscriptions",
        "Talent Workshops",
        "CPSC Certificates",
        "Ratings",
        "Shop Help",
        "Contact Us",
      ],

      sites: ["DC", "MAD Magazine", "DC Kids", "DC Universe", "DC Power Visa"],

      icons: [
        {
          path: "../../public/img/footer-facebook.png",
        },
        {
          path: "../../public/img/footer-twitter.png",
        },
        {
          path: "../../public/img/footer-youtube.png",
        },
        {
          path: "../../public/img/footer-pinterest.png",
        },
        {
          path: "../../public/img/footer-periscope.png",
        },
      ],
    };
  },
};
</script>

<template>
  <footer class="footer">
    <div class="upper-footer container">
      <div>
        <h3>DC COMICS</h3>
        <ul>
          <li v-for="link in links">{{ link }}</li>
        </ul>
        <h3>SHOP</h3>
        <ul>
          <li v-for="shop in shops">{{ shop }}</li>
        </ul>
      </div>
      <div>
        <h3>DC</h3>
        <ul>
          <li v-for="helpOption in helpOptions">{{ helpOption }}</li>
        </ul>
      </div>
      <div>
        <h3>SITES</h3>
        <ul>
          <li v-for="site in sites">{{ site }}</li>
        </ul>
      </div>
      <div id="bg-logo">
        <!-- <img src="../../public/img/dc-logo-bg.png" alt="" /> -->
      </div>
    </div>
    <section class="lower-footer">
      <div class="footer-contents container">
        <button>SIGN-UP NOW!</button>
        <div id="follow-us">
          <p>FOLLOW US</p>
          <img
            v-for="icon in icons"
            :src="icon.path"
            alt=""
            srcset=""
            width="35"
          />
        </div>
      </div>
    </section>
  </footer>
</template>

<style lang="scss" scoped>
.footer {
  background-image: url(../../public/img/footer-bg.jpg);
  background-size: cover;
  position: relative;

  .upper-footer {
    display: flex;
    color: white;
    padding: 30px 0;

    div {
      width: 150px;
    }
    ul {
      list-style-type: none;
      margin: 0;
      padding: 0;
      line-height: 20px;
    }
    li {
      color: gray;
    }
  }
  #bg-logo {
    height: 460px;
    width: 500px;
    background-image: url(../../public/img/dc-logo-bg.png);
    background-size: cover;
    position: absolute;
    left: 55%;
    bottom: 20%;
    overflow: hidden;
  }

  .lower-footer {
    background-color: #303030;

    height: 95px;

    .footer-contents {
      height: 100%;
      display: flex;
      justify-content: space-between;
      align-items: center;

      #follow-us {
        display: flex;
        align-items: center;
        color: #0282f9;
      }

      #follow-us * {
        margin-right: 1rem;
      }
    }
    button {
      border: 2px solid #0282f9;
      background-color: #303030;
      color: white;
      padding: 1rem;
    }
  }
}
</style>
