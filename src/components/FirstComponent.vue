<template>
  <div>
    <h1>Olá Vue</h1>
    <p>Meu nome é {{ nome }} e minha profissão é {{ profissao }}</p>
  </div>
</template>

<script>
export default {
  name: "FirstComponent",
  data() {
    return {
      nome: "Daniel",
      profissao: "Dev",
    };
  },
};
</script>