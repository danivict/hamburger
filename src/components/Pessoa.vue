<template>
  <div>
    <h2>Esta é a descrição da pessoa {{ nome }}</h2>
    <Info />
    <Picture />
  </div>
</template>

<script>
import Info from "./Info.vue";
import Picture from "./Picture.vue";

export default {
  name: "Pessoa",
  components: {
    Info,
    Picture,
  },
  data() {
    return {
      nome: "Daniel",
    };
  },
};
</script>