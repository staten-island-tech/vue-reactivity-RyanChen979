<template>
  <ol>
    <li v-for="items in items">
      Name: {{ items.name }}; Value: {{ items.value }}
    </li>
  </ol>
</template>

<script>
export default {
  data() {
    return {
      items: [
        { name: "1", value: "hgj", id: 1, img: "" },
        { name: "2", value: "ehgfwr", id: 2, img: "" },
        { name: "3", value: "tehgfw", id: 2, img: "" },
        { name: "5", value: "dsdsff", id: 2, img: "" },
        { name: "4", value: "qdsfw", id: 2, img: "" },
        { name: "6", value: "ddsfsf", id: 2, img: "" },
        { name: "7", value: "dsf", id: 2, img: "" },
        { name: "8", value: "ewr", id: 2, img: "" },
        { name: "9", value: "tysf", id: 2, img: "" },
        { name: "10", value: "svcbdf", id: 2, img: "" },
        { name: "11", value: "edfwr", id: 2, img: "" },
      ],
    };
  },
};
</script>
