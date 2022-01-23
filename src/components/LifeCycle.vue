<template>
  <div>
    <h1>Meu nome eh: {{ nome }}</h1>
  </div>
</template>

<script>
export default {
  name: "LifeCycle",
  data() {
    return {
      nome: "Nu stiu",
    };
  },
  created() { // usado para criar o loader
    //ao carregar pagina troca data
    setTimeout(() => {
      this.nome = "Luciius";
    }, 1000);
  },
  mounted() {
    // troca valor
    setTimeout(() => {
      this.nome = "Petris";
    }, 2000);
  },
};
</script>