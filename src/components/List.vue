<template>
  <div class="landing">
    <Thumbnail
      idx="0"
      tagline="Lorem ipsum"
      heading="Lorem ipsum dolor sit amet"
    />
    <Thumbnail
      idx="1"
      tagline="Lorem ipsum"
      heading="Lorem ipsum dolor sit amet"
    />
    <Thumbnail
      idx="2"
      tagline="Lorem ipsum"
      heading="Lorem ipsum dolor sit amet"
    />
  </div>
</template>

<script>
import Thumbnail from "./shared/Thumbnail.vue";

export default {
  name: "List",
  data() {
    return {
      images: [
        "@/assets/items/item_1.jpg",
        "@/assets/items/item_2.jpg",
        "@/assets/items/item_3.jpg"
      ]
    };
  },
  components: {
    Thumbnail
  },
  props: {
    msg: String
  }
};
</script>

<!-- "scoped" attribute limits CSS to this component only -->
<style scoped lang="less">
.landing {
  height: 100%;
  width: 100%;
  background-color: #000;
  margin-bottom: 5rem;
}  
</style>
