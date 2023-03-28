<template>
  <div class="everything">
    <div class="card" v-for="list in computers" data-aos="zoom-out-up">
      <h2>{{ list.name }}</h2>
      <h3>Price: ${{ list.price }}</h3>
      <img :src="list.image" :alt="list.name" /><br />

      <div class="details">
        <h4 id="details">Details:</h4>
        <p>Processor: {{ list.details.processor }}</p>
        <p>Ram: {{ list.details.memory }}</p>
        <p>Hard Drive: {{ list.details.harddrive }}</p>
        <p>Color: {{ list.details.color }}</p>
      </div>
      <button class="button" type="click">Add to Cart</button>
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
            processor: "Intel Core i7 1260P (12th Gen)",
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
            processor: "Intel Core i7-1065G7 (12th Gen)",
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
          name: "MacBook Air M2",
          price: 1599,
          image:
            "https://store.storeimages.cdn-apple.com/4982/as-images.apple.com/is/macbook-air-midnight-config-20220606?wid=410&hei=249&fmt=jpeg&qlt=95&.v=1654122880566",
          details: {
            processor: "Apple M2",
            memory: "16 GB",
            harddrive: "512 GB SSD",
            color: "Midnight",
          },
        },
        {
          name: "Lenovo IdeaPad Flex",
          price: 749.99,
          image:
            "https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSoVJM1nAhmCIcML6OTvNatlZSCxEup9qwEj8SaWG-BkDfI8wbFFSNWxqTNjmyXc6v452w&usqp=CAU",
          details: {
            processor: "AMD Ryzen 5 5500U",
            memory: "8 GB LPDDR4X",
            harddrive: "256 GB SSD",
            color: "Storm Grey",
          },
        },
        {
          name: "ASUS ROG Strix SCAR 16",
          price: 3699.99,
          image:
            "https://cdn.shopify.com/s/files/1/0228/7629/1136/products/02_SCAR_16_L_2afecb5b-839b-4b8a-8eba-235659e389be_2000x.png?v=1674747492",
          details: {
            processor: "Intel Core i9-13980HX",
            memory: "64 GB RAM",
            harddrive: "2 TB SSD",
            color: "Black",
          },
        },
        {
          name: "Acer Swift 5",
          price: 799.99,
          image:
            "https://images.acer.com/is/image/acer/Swift-5_SF514-55TA_Fp-Backliton_Misty-Green_01a-1?$Product-Cards-XL$",
          details: {
            processor: "Intel Core i7 1165G7 (11th Gen)",
            memory: "	16 GB",
            harddrive: "512 GB SSD",
            color: "Mist Green",
          },
        },
        {
          name: "Acer - Chromebook Spin 311",
          price: 249,
          image:
            "https://images.acer.com/is/image/acer/chromebook-spin-311_cp311-3h_01c-2",
          details: {
            processor: "MediaTek Kompanio 500 Series",
            memory: "4 GB LPDDR4X",
            harddrive: "64 GB",
            color: "Pure Silver",
          },
        },
        {
          name: "HP ENVY 13",
          price: 1169.99,
          image:
            "https://ssl-product-images.www8-hp.com/digmedialib/prodimg/lowres/c08226080.png?imdensity=1&imwidth=175",
          details: {
            processor: "Intel Core i7-1250U",
            memory: "8 GB",
            harddrive: "1 TB SSD",
            color: "Natural Silver",
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
  methods: {
    cartList: [],
    Cart: function () {
      document.button.addEventListener("click");
    },
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

.button {
  margin-top: 1rem;
  background-color: white;
  border-radius: 10px;
}
</style>
