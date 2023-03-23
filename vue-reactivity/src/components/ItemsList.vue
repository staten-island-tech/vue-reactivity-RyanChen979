<template>
  <div class="items">
    <div class="item" v-for="list in computers">
      <h2>Name: {{ list.name }}</h2>
      <h3>Price: ${{ list.price }}</h3>
      <img :src="list.image" alt="" />
      <button type="submit">Details</button>
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
          price: 1149.0,
          category: "laptops",
          image:
            "https://www.notebookcheck.net/uploads/tx_nbc2/xps_13_plus_9320.jpg",
        },
        {
          name: "Lenovo Slim 7",
          price: 873.99,
          category: "laptops",
          image:
            "https://p4-ofp.static.pub/ShareResource/na/subseries/gallery/lenovo-slim-7i-14inch-01.png",
        },
        {
          name: "Dell G15",
          price: 1099.99,
          category: "laptops",
          image:
            "https://i.dell.com/is/image/DellContent/content/dam/ss2/product-images/dell-client-products/notebooks/g-series/g15-5525/pdp/laptop-g-series-15-5525-pdp-hero-bk-coralkb.psd?qlt=95&fit=constrain,1&hei=349&wid=504&fmt=jpg&wid=570&hei=400",
        },
        {
          name: "HP Victus 15 (2022)",
          price: 0,
          category: "laptops",
          image:
            "https://m.media-amazon.com/images/W/IMAGERENDERING_521856-T1/images/I/61ZRgmj+NqL.jpg",
        },
        {
          name: "MacBook Air",
          price: 0,
          category: "laptops",
          image:
            "https://i.pcmag.com/imagery/reviews/02pPlSC851BxRP4BFdufSBJ-3.fit_lim.size_1050x.jpg",
        },
        {
          name: " ",
          price: 0,
          category: "laptops",
          image: "",
        },
        {
          name: "",
          price: 0,
          category: "laptops",
          image: "",
        },
        {
          name: "",
          price: 0,
          category: "laptops",
          image: "",
        },
        {
          name: "",
          price: 0,
          category: "laptops",
          image: "",
        },
        {
          name: "",
          price: 0,
          category: "laptops",
          image: "",
        },
        {
          name: "",
          price: 0,
          category: "laptops",
          image: "",
        },
        {
          name: "",
          price: 0,
          category: "laptops",
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
          category: "laptops",
          image: "",
        },
        {
          name: "",
          price: 0,
          category: "laptops",
          image: "",
        },
        {
          name: "",
          price: 0,
          category: "laptops",
          image: "",
        },
        {
          name: "",
          price: 0,
          category: "laptops",
          image: "",
        },
        {
          name: " ",
          price: 0,
          category: "laptops",
          image: "",
        },
        {
          name: "",
          price: 0,
          category: "laptops",
          image: "",
        },
        {
          name: "",
          price: 0,
          category: "laptops",
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
  justify-items: center;
  align-items: center;
}

.item img {
  object-fit: cover;
  border-radius: inherit;
  width: 15rem;
}

.item button {
}
</style>
