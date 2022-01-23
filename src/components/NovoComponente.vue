<template>
  <div>
    <h1>Ola ----</h1>
    <p>O nome eh {{ nome }}</p>
  </div>
</template>

<script>
export default {
  name: "NovoComponente",
  data() {
    return {
      nome: "Tuva",
    };
  },
};
</script>