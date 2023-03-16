<template>
  <ol>
    <li v-for="items in items">{{ items.message }} {{ items.value }}</li>
  </ol>
</template>

<script>
export default {
  data() {
    return {
      items: [
        { message: "Foo", value: "whatever", id: 1, img: "cvs.com" },
        { message: "Bar", value: "hello", id: 2, img: "bestbuy.com" },
      ],
    };
  },
};
</script>
