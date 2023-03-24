<template>
  <div class="everything">
    <div class="card" v-for="list in computers" data-aos="zoom-out-up">
      <h2>Name: {{ list.name }}</h2>
      <h3>Price: ${{ list.price }}</h3>
      <img :src="list.image" :alt="list.name" /><br />
      <!-- <button type="submit">Details</button> -->
      <div>
        <h4 class="details">Details:</h4>
        <p>Processor: {{ list.details.processor }}</p>
        <p>Ram: {{ list.details.memory }}</p>
        <p>Hard Drive: {{ list.details.harddrive }}</p>
        <p>Color: {{ list.details.color }}</p>
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
          price: 1499.0,
          image:
            "https://www.notebookcheck.net/uploads/tx_nbc2/xps_13_plus_9320.jpg",
          details: {
            processor:
              "12th Gen Intel Core i7 1260P (16 threads, 4.70 GHz Turbo)",
            memory: "16GB LPDDR5, 5200 MHz, integrated, dual channel",
            harddrive: "1TB, M.2, Gen 4 PCle NVMe, SSD",
            color: "platinum",
          },
        },
        {
          name: "Lenovo Slim 7",
          price: 873.99,
          image:
            "https://p4-ofp.static.pub/ShareResource/na/subseries/gallery/lenovo-slim-7i-14inch-01.png",
          details: {
            processor: "",
            memory: "",
            harddrive: "",
            color: "",
          },
        },
        {
          name: "Dell G15",
          price: 1099.99,
          image:
            "https://i.dell.com/is/image/DellContent/content/dam/ss2/product-images/dell-client-products/notebooks/g-series/g15-5525/pdp/laptop-g-series-15-5525-pdp-hero-bk-coralkb.psd?qlt=95&fit=constrain,1&hei=349&wid=504&fmt=jpg&wid=570&hei=400",
          details: {
            processor: "",
            memory: "",
            harddrive: "",
            color: "",
          },
        },
        {
          name: "HP Victus 15 (2022)",
          price: 549.99,
          image:
            "https://m.media-amazon.com/images/W/IMAGERENDERING_521856-T1/images/I/61ZRgmj+NqL.jpg",
          details: {
            processor: "",
            memory: "",
            harddrive: "",
            color: "",
          },
        },
        {
          name: "MacBook Air",
          price: 1199.0,
          image:
            "https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTo1ZAKTLP5A_guGxt05oUjilK8VzSk4z-UQQ&usqp=CAU",
          details: {
            processor: "",
            memory: "",
            harddrive: "",
            color: "",
          },
        },
        {
          name: "",
          price: 0,
          image: "",
          details: {
            processor: "",
            memory: "",
            harddrive: "",
            color: "",
          },
        },
        {
          name: "",
          price: 0,
          image: "",
          details: {
            processor: "",
            memory: "",
            harddrive: "",
            color: "",
          },
        },
        {
          name: "",
          price: 0,
          image: "",
          details: {
            processor: "",
            memory: "",
            harddrive: "",
            color: "",
          },
        },
        {
          name: "",
          price: 0,
          image: "",
          details: {
            processor: "",
            memory: "",
            harddrive: "",
            color: "",
          },
        },
        {
          name: "",
          price: 0,
          image: "",
          details: {
            processor: "",
            memory: "",
            harddrive: "",
            color: "",
          },
        },
        {
          name: "",
          price: 0,
          image: "",
          details: {
            processor: "",
            memory: "",
            harddrive: "",
            color: "",
          },
        },
        {
          name: "",
          price: 0,
          image: "",
          details: {
            processor: "",
            memory: "",
            harddrive: "",
            color: "",
          },
        },
        {
          name: "",
          price: 0,
          category: "electronics",
          image: "",
          details: {
            processor: "",
            memory: "",
            harddrive: "",
            color: "",
          },
        },
        {
          name: " ",
          price: 0,
          image: "",
          details: {
            processor: "",
            memory: "",
            harddrive: "",
            color: "",
          },
        },
        {
          name: "",
          price: 0,
          image: "",
          details: {
            processor: "",
            memory: "",
            harddrive: "",
            color: "",
          },
        },
        {
          name: "",
          price: 0,
          image: "",
          details: {
            processor: "",
            memory: "",
            harddrive: "",
            color: "",
          },
        },
        {
          name: "",
          price: 0,
          image: "",
          details: {
            processor: "",
            memory: "",
            harddrive: "",
            color: "",
          },
        },
        {
          name: " ",
          price: 0,
          image: "",
          details: {
            processor: "",
            memory: "",
            harddrive: "",
            color: "",
          },
        },
        {
          name: "",
          price: 0,
          image: "",
          details: {
            processor: "",
            memory: "",
            harddrive: "",
            color: "",
          },
        },
        {
          name: "",
          price: 0,
          image: "",
          details: {
            processor: "",
            memory: "",
            harddrive: "",
            color: "",
          },
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
  display: flex;
  flex-wrap: wrap;
  flex-direction: column;
  justify-content: flex-start;
  width: 20%;
  height: auto;
  margin: 1.45rem;
  border: 2px black solid;
  text-align: center;
  align-items: center;
}

img {
  object-fit: cover;
  border-radius: inherit;
  width: 15rem;
}

.details {
  text-decoration: underline;
}

ul {
  width: 80%;
}
</style>
