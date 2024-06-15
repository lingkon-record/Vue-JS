<template>
  <div id="app">
    <AAppHeader />
    <BannerAdd/>
    <ProductGrid />
    <BlogPage />
  </div>
</template>

<script>
import AAppHeader from "./components/AAppHeader.vue";
import ProductGrid from "./components/ProductGrid";
import BlogPage from "./components/BlogPage";
import BannerAdd from "./components/BannerAdd";

export default {
  name: "App",
  components: {
    AAppHeader,
    BannerAdd,
    ProductGrid,
    BlogPage
  },
};
</script>
