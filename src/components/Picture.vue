<template>
  <img :src="source" :alt="desc" />
  <button v-on:click="changeImg">Change Image</button>
</template>

<script>
export default {
  name: "Picture",
  data() {
    return {
      count: 0,
      source:
        "https://upload.wikimedia.org/wikipedia/commons/thumb/d/d8/Emblem-person-blue.svg/1200px-Emblem-person-blue.svg.png",
      desc: "imagem aleatória",
      images: [
        "https://icons-for-free.com/download-icon-person-1324760545186718018_512.png",
        "https://eitrawmaterials.eu/wp-content/uploads/2016/09/person-icon.png",
        "https://img.freepik.com/free-icon/important-person_318-10744.jpg?w=2000",
      ],
    };
  },
  methods: {
    changeImg() {
      this.source = this.images[this.count];
      this.count++;
      if (this.count > 2) this.count = 0;
    },
  },
};
</script>