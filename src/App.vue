<template>
  <div>
    <Header />
    <div class="bet-body">
      <SportTabs />
    </div>
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import SportTabs from "./components/SportTabs.vue";

export default {
  name: "App",
  components: {
    Header,
    SportTabs
  }
};
</script>
