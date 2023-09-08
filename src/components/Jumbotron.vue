<script>
export default {
  data() {
    return {
      imageUrl: "avatar_2.jpg",
    };
  },

  methods: {
    getImageUrl(name) {
      return new URL(`../assets/img/${name}`, import.meta.url).href;
    },
  },
};
</script>

<template>
  <img :src="getImageUrl(imageUrl)" alt="" />
</template>

<style scoped></style>
