<template>
  <div class="list-item">
    <div class="image">
      <img :src="images[idx]" />
    </div>
    <div class="content">
      <p class="tagline">{{ tagline }}</p>
      <h3 class="heading">{{ heading }}</h3>
    </div>
  </div>
</template>

<script>
import Img1 from "@/assets/items/item_1.jpg";
import Img2 from "@/assets/items/item_2.jpg";
import Img3 from "@/assets/items/item_3.jpg";

export default {
  name: "Thumbnail",
  props: {
    idx: String,
    tagline: String,
    heading: String
  },
  data() {
    return {
      images: [Img1, Img2, Img3]
    };
  }
};
</script>

<style scoped lang="less">
.list-item {
  max-height: 27rem;
  max-width: 80rem;
  margin: 0 auto;
  padding: 2rem 0;
  display: flex;

    &:nth-child(2) {
    flex-direction: row-reverse;

    .content {
     margin-right: 5rem;
  }
  }
}

.image {
  max-width: 48rem;
  max-height: 27rem;

  img {
    width: 100%;
    height: 100%;
  }
}

.content {
  display: flex;
  flex-direction: column;
  justify-content: center;
  max-width: 27rem;
  max-height: 13.5rem;
  margin-top: auto;
  margin-bottom: auto;
  margin-left: -5rem;
  text-align: left;



}

.tagline {
  color: #fff;
  text-transform: uppercase;
  font-weight: 700;
}

.heading {
  color: #fff;
  font-size: 4rem;
  font-weight: 700;
  letter-spacing: -0.25rem;
}
</style>
