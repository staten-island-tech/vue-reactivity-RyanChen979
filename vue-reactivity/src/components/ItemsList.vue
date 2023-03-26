<template>
  <div class="everything">
    <div class="card" v-for="list in computers" data-aos="zoom-out-up">
      <h2>{{ list.name }}</h2>
      <h3>Price: ${{ list.price }}</h3>
      <img :src="list.image" :alt="list.name" /><br />
      <!-- <button type="submit">Details</button> -->
      <div class="details">
        <h4 id="details">Details:</h4>
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
            "https://i.dell.com/is/image/DellContent/content/dam/ss2/product-images/dell-client-products/notebooks/xps-notebooks/xps-13-9320/media-gallery/xs9320t-cnb-00005ff090-sl-oled.psd?fmt=png-alpha&pscan=auto&scl=1&hei=402&wid=628&qlt=100,1&resMode=sharp2&size=628,402&chrss=full",
          details: {
            processor: "12th Gen Intel Core i7 1260P",
            memory: "16GB LPDDR5",
            harddrive: "1 TB SSD",
            color: "Platinum",
          },
        },
        {
          name: "Lenovo Slim 7i",
          price: 1639.99,
          image:
            "https://p1-ofp.static.pub/medias/24268996282_82VA_202205301038021660044262642.png",
          details: {
            processor: "12th Gen Intel Core i7-1065G7",
            memory: "16 GB LPDDR5",
            harddrive: "1 TB SSD",
            color: "Light Silver",
          },
        },
        {
          name: "Dell G15",
          price: 1399.99,
          image:
            "https://i.dell.com/is/image/DellContent/content/dam/ss2/product-images/dell-client-products/notebooks/g-series/g15-5525/media-gallery/g15-5525-bk-coralkb/notebook-g-15-5525-black-coralkb-gallery-1.psd?fmt=png-alpha&pscan=auto&scl=1&hei=402&wid=457&qlt=100,1&resMode=sharp2&size=457,402&chrss=full",
          details: {
            processor: "AMD Ryzen 7 6800H",
            memory: "16 GB DDR4",
            harddrive: "1 TB SSD",
            color: "Dark Shadow Grey",
          },
        },
        {
          name: "HP Victus 15 (2022)",
          price: 799.99,
          image:
            "https://ssl-product-images.www8-hp.com/digmedialib/prodimg/lowres/c08186082.png",
          details: {
            processor: "Intel Core i5",
            memory: "8 GB DDR4",
            harddrive: "256 GB SSD",
            color: "Mica Silver",
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
  padding: 0.5rem;
  border: 2px black solid;
  text-align: center;
  align-items: center;
}

img {
  object-fit: cover;
  border-radius: inherit;
  height: 10rem;
  width: auto;
}

#details {
  text-decoration: underline;
}

ul {
  width: 80%;
}
</style>
