<template>
  <div class="items">
    <div class="item" v-for="list in computers">
      <h2>Name: {{ list.name }}</h2>
      <h3>Price: ${{ list.price }}</h3>
      <img :src="list.image" class="imgs" alt="" />
    </div>
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
.items {
  display: flex;
  flex-wrap: wrap;
  flex-direction: row;
  justify-content: space-between;
}

.item {
  display: flex;
  flex-wrap: wrap;
  flex-direction: column;
  width: 20%;
  margin: 1rem;
  border: 2px black solid;
  align-items: center;
}

.imgs {
  width: 15rem;
}
</style>
