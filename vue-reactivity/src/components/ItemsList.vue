<template>
  <div class="items">
    <h2 v-for="list in computers">
      Name: {{ list.name }} <br />
      Price: ${{ list.price }}
    </h2>
    <img v-for="list in computers" :src="list.image" class="image" alt="" />
  </div>
</template>

<script>
export default {
  data() {
    return {
      computers: [
        {
          name: "Dell XPS 13 Plus 9320",
          price: 1599,
          category: "",
          image:
            "https://www.notebookcheck.net/uploads/tx_nbc2/xps_13_plus_9320.jpg",
        },
        {
          name: "Lenovo Slim 7",
          price: 873.99,
          category: "",
          image:
            "https://p4-ofp.static.pub/ShareResource/na/subseries/gallery/lenovo-slim-7i-14inch-01.png",
        },
        {
          name: "",
          price: 0,
          category: "",
          image: "",
        },
        {
          name: "",
          price: 0,
          category: "",
          image: "",
        },
        {
          name: "",
          price: 0,
          category: "",
          image: "",
        },
        {
          name: " ",
          price: 0,
          category: "",
          image: "",
        },
        {
          name: "",
          price: 0,
          category: "",
          image: "",
        },
        {
          name: "",
          price: 0,
          category: "",
          image: "",
        },
        {
          name: "",
          price: 0,
          category: "",
          image: "",
        },
        {
          name: "",
          price: 0,
          category: "",
          image: "",
        },
        {
          name: "",
          price: 0,
          category: "",
          image: "",
        },
        {
          name: "",
          price: 0,
          category: "",
          image: "",
        },
        {
          name: "",
          price: 0,
          category: "electronics",
          image: "",
        },
        {
          name: " ",
          price: 0,
          category: "",
          image: "",
        },
        {
          name: "",
          price: 0,
          category: "",
          image: "",
        },
        {
          name: "",
          price: 0,
          category: "",
          image: "",
        },
        {
          name: "",
          price: 0,
          category: "",
          image: "",
        },
        {
          name: " ",
          price: 0,
          category: "",
          image: "",
        },
        {
          name: "",
          price: 0,
          category: "",
          image: "",
        },
        {
          name: "",
          price: 0,
          category: "",
          image: "",
        },
      ],
    };
  },
};
</script>

<style scoped>
image {
  height: 1rem;
  width: auto;
}
</style>
