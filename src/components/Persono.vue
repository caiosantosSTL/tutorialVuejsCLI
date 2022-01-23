<template>
  <div>
    <h2>Desc da pessoa: {{ nome }}</h2>
    <Infos />
  </div>
</template>

<script>
import Infos from "./Infos.vue"; //import Infos component
export default {
  components: { Infos }, //import Infos component
  name: "Pessoa",
  data() {
    return {
      nome: "Matias",
    };
  },
};
</script>