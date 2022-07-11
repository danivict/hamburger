<template>
  <div>
    <first-component />
    <life-cycle />
    <pessoa />
  </div>
</template>

<script>
import FirstComponent from "./components/FirstComponent.vue";
import LifeCycle from "./components/LifeCycle.vue";
import Pessoa from "./components/Pessoa.vue";

export default {
  name: "App",
  components: {
    FirstComponent,
    LifeCycle,
    Pessoa,
  },
};
</script>