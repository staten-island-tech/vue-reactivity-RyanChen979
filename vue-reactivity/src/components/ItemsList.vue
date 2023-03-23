<template>
  <div class="everything">
    <div class="card" v-for="list in computers">
      <div class="card-inner">
        <div class="card-front">
          <h2>Name: {{ list.name }}</h2>
          <h3>Price: ${{ list.price }}</h3>
          <img :src="list.image" alt="" /><br />
          <button type="submit">Details</button>
        </div>
        <div class="card-back">
          <img :src="list.image" alt="" />
        </div>
      </div>
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
          details: {
            processor: "",
            software: "",
            memory: "",
          },
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
.everything {
  display: flex;
  flex-wrap: wrap;
  flex-direction: row;
  justify-content: space-between;
}

.card {
  background-color: transparent;
  width: 20%;
  height: 300px;
  perspective: 1000px;
  margin: 1.45rem;
}

.card-inner {
  display: flex;
  flex-wrap: wrap;
  flex-direction: column;

  margin: 1rem;
  border: 2px black solid;

  position: relative;
  width: 100%;
  height: 100%;
  text-align: center;
  transition: transform 0.6s;
  transform-style: preserve-3d;
}
.card:hover .card-inner {
  transform: rotateY(180deg);
}

.card-front,
.card-back {
  position: absolute;
  width: 100%;
  height: 100%;
  -webkit-backface-visibility: hidden;
  backface-visibility: hidden;
  border-radius: 16px;
}

.card-back {
  transform: rotateY(180deg);
}

.card-front img {
  object-fit: cover;
  border-radius: inherit;
  width: 15rem;
}
.card-front button {
}

.card-back img {
  width: 15rem;
}
</style>
