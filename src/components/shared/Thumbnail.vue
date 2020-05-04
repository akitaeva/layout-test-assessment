<template>
  <div class="list-item">
    <div class="image">
      <img :src="images[idx]" alt="artcilePic" />
    </div>
    <div class="content">
      <p class="tagline">{{ tagline }}</p>
      <h3 class="heading">{{ heading }}</h3>
      <a href="/">
        See more
        <img :src="forward" />
      </a>
    </div>
  </div>
</template>

<script>
import Img1 from "@/assets/items/item_1.jpg";
import Img2 from "@/assets/items/item_2.jpg";
import Img3 from "@/assets/items/item_3.jpg";
import Forward from "@/assets/icons/forward.svg";

export default {
  name: "Thumbnail",
  props: {
    idx: String,
    tagline: String,
    heading: String
  },
  data() {
    return {
      images: [Img1, Img2, Img3],
      forward: Forward
    };
  }
};
</script>

<style scoped lang="less">
.list-item {
  max-height: 27rem;
  width: 80rem;
  max-width: 80vw;
  margin: 0 auto;
  padding: 2rem 0;
  display: flex;

  @media screen and (min-width: 1024px) {
    &:nth-child(2) {
      flex-direction: row-reverse;
    }
  }

  @media screen and (max-width: 1024px) {
    margin: 0 5%;
  }
}

.image {
  max-width: 65%;
  max-height: 100%;

  img {
    width: 100%;
    height: 100%;
    object-fit: cover;
  }

  @media screen and (max-width: 834px) {
    max-width: 45%;
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

  @media screen and (max-width: 834px) {
    margin-left: 1rem;
  }
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

  @media screen and (max-width: 1024px) {
    font-size: 3rem;
  }

  @media screen and (max-width: 834px) {
    font-size: 2rem;
    max-width: 85%;
    letter-spacing: -0.1rem;
  }
}

a {
  color: #fff;
  text-decoration: none;
  text-transform: uppercase;
}
</style>
