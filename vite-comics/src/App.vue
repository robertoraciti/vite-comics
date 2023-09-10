<script>
import AppHeader from "./components/AppHeader.vue";
import AppMain from "./components/AppMain.vue";
import AppFooter from "./components/AppFooter.vue";
import AzureSec from "./components/AzureSec.vue";

export default {
  data() {
    return {
      title: "",
    };
  },

  components: {
    AppHeader,
    AppMain,
    AppFooter,
    AzureSec,
  },
};
</script>

<template>
  <AppHeader />
  <AppMain />
  <AzureSec />
  <AppFooter />
</template>

<style lang="scss">
body {
  background-color: black;
}

.container {
  width: 70%;
  margin: auto;
}

.active {
  color: #0282f9;
  border-bottom: 5px solid #0282f9;
}
</style>
